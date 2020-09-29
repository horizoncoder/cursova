<template>
<v-conteiner>
  <div class="CaruselBlock">
      <v-carousel :show-arrows="true" cycle>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
  </div>
</v-conteiner>
   
</template>

<script>
  export default{
    name: 'Carusel',
  data () {
        return {
          items: [
            {
              src: require("../img/alienware.jpg"),
            },
            {
               src: require("../img/msi.jpg"),
            },
            {
              src: require("../img/asus.jpg"),
            },
            {
              src: require("../img/omen.png"),
            },
          ],
        }
      },
    }
</script>