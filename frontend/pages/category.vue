<template>
  <div>
      <Headerdef/>

      <v-container class="mt-8">
              <v-row>
                  <v-col>
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/man-tshirt')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p class="category-title">Подволк</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="category" src="~/assets/category/tshirt.png">
                                </v-list-item>
                      </v-card>
                  </v-col>

                  <v-col>
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/man-tshirt')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p class="category-title">Малгайтай <br>цамц</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="category" src="~/assets/category/hoodie.png">
                                </v-list-item>
                      </v-card>
                  </v-col>

                  <v-col>
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/man-tshirt')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p class="category-title">Цамц</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="category" src="~/assets/category/shirt.png">
                                </v-list-item>
                      </v-card>
                  </v-col>
              </v-row>

              <v-row>
                  <v-col class="mx-auto">
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/man-tshirt')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p class="category-title">Майк</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="category" src="~/assets/category/tanktop.png">
                                </v-list-item>
                      </v-card>
                  </v-col>
                  <v-col class="mx-auto">
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/man-tshirt')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p class="category-title">Jersey</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="category" src="~/assets/category/jersey.png">
                                </v-list-item>
                      </v-card>
                  </v-col>
                  <v-col class="mx-auto">
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/man-tshirt')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p class="category-title">Оймс</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="category" src="~/assets/category/socks.png">
                                </v-list-item>
                      </v-card>
                  </v-col>
              </v-row>
          </v-container>
  </div>
</template>

<script>
import  Headerdef  from "~/components/default-header.vue";
export default {
    components :{
        Headerdef 
    }
}
</script>

<style scoped>
.category {
    width: 150px;
    height: 150px;
}
.category-title {
    font-weight: 700;
    font-family: 'Roboto';
    font-size: 20px;
}
.v-card {
    cursor: pointer;
}
</style>