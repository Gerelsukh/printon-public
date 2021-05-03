<template>
  <div>
      <Headerdef/>

      <div class="product-container">
          <div class="search-bar mt-3">
              <v-container>
              <v-row>
                  <v-col wider>
                      <v-text-field
                    class="rounded-pill"
                    prepend-inner-icon="mdi-magnify"
                    placeholder="Бараа, бүтээгдэхүүн, төрлөөр хайх"
                    outlined
                    color="#25BC3D"
                    background-color="#F5F5F5"
               ></v-text-field>
                  </v-col>
              </v-row>
          </v-container>
              
          </div>
      </div>
      
      <div class="product-container">
          <div class="sub-container-title"><h2>Бестселлер</h2></div>

          <v-container>
              <v-row>
                  <v-col>
                      <v-card
                            tile
                            class="mx-auto"
                            max-width="260"
                            height="400"
                            >
                                <v-chip
                                class="ma-2 chip"
                                label
                                outlined
                                text-color="black"
                                >
                                Бестселлер
                                </v-chip>
                        <img class="bestseller"
                            src="~/assets/products/bestseller1.png"
                        >
                        <v-card-title>T-Shirt</v-card-title>
                        <v-card-text>
                            <v-row
                                align="center"
                                class="mx-0"
                            >
                                <v-rating
                                :value="4.5"
                                color="amber"
                                dense
                                half-increments
                                readonly
                                size="14"
                                ></v-rating>

                                <div class="grey--text ml-4">
                                4.5 (413)
                                </div>
                            </v-row>

                            <div class="mt-2">Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
                            </v-card-text>
                        </v-card>
                  </v-col>

                  <v-col>
                      <v-card
                            tile
                            class="mx-auto"
                            max-width="260"
                            height="400"
                            >
                                <v-chip
                                class="ma-2 chip"
                                label
                                outlined
                                text-color="black"
                                >
                                Бестселлер
                                </v-chip>
                        <img class="bestseller"
                            src="~/assets/products/bestseller2.png"
                        >
                        <v-card-title>Eco Bag</v-card-title>
                        <v-card-text>
                            <v-row
                                align="center"
                                class="mx-0"
                            >
                                <v-rating
                                :value="4.5"
                                color="amber"
                                dense
                                half-increments
                                readonly
                                size="14"
                                ></v-rating>

                                <div class="grey--text ml-4">
                                4.5 (413)
                                </div>
                            </v-row>

                            <div class="mt-2">Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
                            </v-card-text>
                        </v-card>
                  </v-col>

                  <v-col>
                      <v-card
                            tile
                            class="mx-auto"
                            max-width="260"
                            height="400"
                            >
                                <v-chip
                                class="ma-2 chip"
                                label
                                outlined
                                text-color="black"
                                >
                                Бестселлер
                                </v-chip>
                        <img class="bestseller"
                            src="~/assets/products/bestseller3.png"
                        >
                        <v-card-title>T-Shirt</v-card-title>
                        <v-card-text>
                            <v-row
                                align="center"
                                class="mx-0"
                            >
                                <v-rating
                                :value="4.5"
                                color="amber"
                                dense
                                half-increments
                                readonly
                                size="14"
                                ></v-rating>

                                <div class="grey--text ml-4">
                                4.5 (413)
                                </div>
                            </v-row>

                            <div class="mt-2">Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
                            </v-card-text>
                        </v-card>
                  </v-col>

                  <v-col>
                      <v-card
                            tile
                            class="mx-auto"
                            max-width="260"
                            height="400"
                            >
                                <v-chip
                                class="ma-2 chip"
                                label
                                outlined
                                text-color="black"
                                >
                                Бестселлер
                                </v-chip>
                        <img class="bestseller"
                            src="~/assets/products/bestseller4.png"
                        >
                        <v-card-title>T-Shirt</v-card-title>
                        <v-card-text>
                            <v-row
                                align="center"
                                class="mx-0"
                            >
                                <v-rating
                                :value="4.5"
                                color="amber"
                                dense
                                half-increments
                                readonly
                                size="14"
                                ></v-rating>

                                <div class="grey--text ml-4">
                                4.5 (413)
                                </div>
                            </v-row>

                            <div class="mt-2">Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
                            </v-card-text>
                        </v-card>
                  </v-col>
              </v-row>
          </v-container>
      </div>

      <div class="product-container">
          <v-container class="">
              <v-row>
                  <v-col>
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/category')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p>Эрэгтэй <br>Хувцас</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="hi" src="~/assets/products/category1.png">
                                </v-list-item>
                      </v-card>
                  </v-col>

                  <v-col>
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/category')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p>Эмэгтэй <br>Хувцас</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="hi" src="~/assets/products/category2.png">
                                </v-list-item>
                      </v-card>
                  </v-col>

                  <v-col>
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/category')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p>Хүүхдийн <br>Хувцас</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="hi" src="~/assets/products/category3.png">
                                </v-list-item>
                      </v-card>
                  </v-col>
              </v-row>

              <v-row>
                  <v-col class="mr-n16">
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/category')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p>Дагалдах <br>Хэрэгсэл</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="hi" src="~/assets/products/category4.png">
                                </v-list-item>
                      </v-card>
                  </v-col>
                  <v-col class="">
                          <v-card
                                class="mx-auto"
                                max-width="344"
                                outlined
                                @click="$router.push('/category')"
                                color="#F7F7F7"
                            >
                                <v-list-item three-line>
                                <v-list-item-content>
                                    <v-list-item-title class="headline mb-1">
                                    <p>Бэлэг <br>Дурсгал</p>
                                    </v-list-item-title>
                                </v-list-item-content>

                                <img class="hi" src="~/assets/products/category5.png">
                                </v-list-item>
                      </v-card>
                  </v-col>
              </v-row>
          </v-container>
      </div>

      <div class="product-container">
          <Recommend/>
      </div>
      <div class="product-container">
          <Newproduct/>
      </div>
  </div>
</template>

<script>
import  Headerdef  from "~/components/default-header.vue";
import  Recommend  from "~/components/recommend.vue";
import  Newproduct  from "~/components/new-arrival.vue";
export default {
    components :{
        Headerdef,
        Recommend,
        Newproduct
    }
}
</script>

<style>
.v-chip.complete {
    background: rgb(255,215,0)!important;
}
.hi {
    width: 150px;
    height: 150px;
}
.chip {
    background-color: rgb(255,215,0)!important;
}
.v-chip {
    position: absolute;
    top: 5px;
}
.bestseller {
    width: 260px;
    height: 250px;
}
.v-text-field {
    width: 1200px;
}
.sub-container-title {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    margin: 30px 50px 20px 50px;
}
.product-container{
    width: 100%;
    height: auto;
}   
</style>