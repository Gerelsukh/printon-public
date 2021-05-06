<template>
  <div>
      <Headerdef/>

      <div class="man-tshirt-container">
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

          <v-container class="">
                <v-row no-gutters>
                <v-col
                    cols="5"
                >
                    <nav class="nav"><a class="links" @click="$router.push('/products')">Төрөл/</a><a class="links" @click="$router.push('/category')">&nbsp;Эрэгтэй Xувцас/</a><a class="links"><span class="current-link">&nbsp;Подволк</span></a></nav>
                </v-col>
                </v-row>
            </v-container>

            <v-container class="">
                <v-row
                no-gutters
                >
                <v-col class="">
                    <h3>T-Shirt</h3>
                </v-col>
                <v-col>
                    <v-select
                    :items="items"
                    placeholder="Ангилах"
                    outlined
                    dense
                    color="#25BC3D"
                    class="d-flex justify-end"
                    ></v-select>
                </v-col>
                </v-row>
            </v-container>

          <v-container class="">
                <v-row no-gutters>
                <v-col
                    cols="5"                    
                    md="3"
                >
                <v-expansion-panels
                    v-model="panel"
                    :disabled="disabled"
                    multiple
                    >
                    <v-expansion-panel>
                        <v-expansion-panel-header>Размер</v-expansion-panel-header>
                        <v-expansion-panel-content>
                        <v-list dense>
                                    <v-header>Размер</v-header>
                                    <v-list-item-group
                                        v-model="selectedItem"
                                        color="primary"
                                    >
                                            <v-checkbox
                                            label="2XS"
                                            color="#25BC3D"
                                            value="2XS"
                                            hide-details
                                            ></v-checkbox>
                                            <v-checkbox
                                            label="XS"
                                            color="#25BC3D"
                                            value="XS"
                                            hide-details
                                            ></v-checkbox>
                                            <v-checkbox
                                            label="S"
                                            color="#25BC3D"
                                            value="S"
                                            hide-details
                                            ></v-checkbox>
                                            <v-checkbox
                                            label="M"
                                            color="#25BC3D"
                                            value="M"
                                            hide-details
                                            ></v-checkbox>
                                            <v-checkbox
                                            label="L"
                                            color="#25BC3D"
                                            value="L"
                                            hide-details
                                            ></v-checkbox>
                                            <v-checkbox
                                            label="XL"
                                            color="#25BC3D"
                                            value="XL"
                                            hide-details
                                            ></v-checkbox>
                                            <v-checkbox
                                            label="2XL"
                                            color="#25BC3D"
                                            value="2XL"
                                            hide-details
                                            ></v-checkbox>
                                    </v-list-item-group>                    
                                </v-list>
                        </v-expansion-panel-content>
                    </v-expansion-panel>
                    <v-expansion-panel>
                        <v-expansion-panel-header>Хэвлэх хэсэг</v-expansion-panel-header>
                        <v-expansion-panel-content>
                         <v-list dense>
                    <v-header>Хэвлэх хэсэг</v-header>
                    <v-list-item-group
                        v-model="selectedItem"
                        color="primary"
                    >
                            <v-checkbox
                            label="Бүх хэсэг"
                            color="#25BC3D"
                            value="all"
                            hide-details
                            ></v-checkbox>
                            <v-checkbox
                            label="Урд хэсэг"
                            color="#25BC3D"
                            value="front"
                            hide-details
                            ></v-checkbox>
                            <v-checkbox
                            label="Ард хэсэг"
                            color="#25BC3D"
                            value="back"
                            hide-details
                            ></v-checkbox>
                            <v-checkbox
                            label="Баруун ханцуй"
                            color="#25BC3D"
                            value="right-sleeve"
                            hide-details
                            ></v-checkbox>
                            <v-checkbox
                            label="Зүүн ханцуй"
                            color="#25BC3D"
                            value="left-sleeve"
                            hide-details
                            ></v-checkbox>
                            <v-checkbox
                            label="Дотор шошго"
                            color="#25BC3D"
                            value="inner-label"
                            hide-details
                            ></v-checkbox>
                            <v-checkbox
                            label="Гадна шошго"
                            color="#25BC3D"
                            value="outer-label"
                            hide-details
                            ></v-checkbox>
                    </v-list-item-group>                    
                </v-list>
                        </v-expansion-panel-content>
                    </v-expansion-panel>

                    <v-expansion-panel>
                        <v-expansion-panel-header>Panel 3</v-expansion-panel-header>
                        <v-expansion-panel-content>
                        Some content
                        </v-expansion-panel-content>
                    </v-expansion-panel>
                    </v-expansion-panels>
                </v-col>
                <v-col
                    cols="13"
                    sm="7"
                    md="9"
                >
                <v-container>
              <v-row>
                  <v-col>
                      <v-card
                            tile
                            class="mx-auto"
                            max-width="260"
                            height="400"
                            @click="$router.push('/product-tshirt')"
                            >
                                <v-chip
                                class="ma-2 chip"
                                label
                                outlined
                                text-color="black"
                                >
                                Шинэ
                                </v-chip>
                        <img class="recommend"
                            src="~/assets/recommend/hoodie.png"
                        >
                        <v-card-title>Hoodie</v-card-title>
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
                            @click="$router.push('/product-tshirt')"
                            >
                                <v-chip
                                class="ma-2 chip"
                                label
                                outlined
                                text-color="black"
                                >
                                Шинэ
                                </v-chip>
                        <img class="recommend"
                            src="~/assets/recommend/hoodie.png"
                        >
                        <v-card-title>Hoodie</v-card-title>
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
                            @click="$router.push('/product-tshirt')"
                            >
                                <v-chip
                                class="ma-2 chip"
                                label
                                outlined
                                text-color="black"
                                >
                                Шинэ
                                </v-chip>
                        <img class="recommend"
                            src="~/assets/recommend/hoodie.png"
                        >
                        <v-card-title>Hoodie</v-card-title>
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
                </v-col>
                </v-row>
            </v-container>
      </div>
  </div>
</template>

<script>
import  Headerdef  from "~/components/default-header.vue";
export default {
    components :{
        Headerdef
    },
    data: () => ({
      items: ['Шинэ', 'Их үнэ', 'Бага үнэ'],
      panel: [0, 1, 2],
      disabled: false,
      readonly: false,

    }),
}
</script>

<style scoped>
.v-select {
    width: 250px;
}
.nav .links {
    font-weight: 500;
    font-family: 'Roboto';
    font-size: 14px;
    color: #25BC3D;
    text-decoration: none;
}
.current-link {
    color: #C7C7C7;
}
.recommend {
        width: 260px;
        height: 250px;
    }
.v-chip {
    position: absolute;
    top: 5px;
}
.v-card {
    cursor: pointer;
}
</style>