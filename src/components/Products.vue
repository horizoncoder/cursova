<template>
    <product>
        <div class="cards">
             <v-card
    class="mx-auto"
    max-width="344"
    padding="34px"
  >
    <v-img
      src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
      height="200px"
    ></v-img>

    <v-card-title>
      Top western road trips
    </v-card-title>

    <v-card-subtitle>
      1,000 miles of wonder
    </v-card-subtitle>

    <v-card-actions>
      <v-btn text>В корзину</v-btn>

      <v-btn
        color="purple"
        text
      >
        Подробние
      </v-btn>

      <v-spacer></v-spacer>

      <v-btn
        icon
        @click="show = !show"
      >
        <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <div v-show="show">
        <v-divider></v-divider>

        <v-card-text>
         Описание товара
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>
        </div>
    </product>
</template>

<script>
  export default {
    data: () => ({
      show: false,
    }),
  }
</script>