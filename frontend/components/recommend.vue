<template>
<div>
  <div class="container-title"><h2>Санал болгох</h2></div>
  
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
                            src="~/assets/recommend/bottle.png"
                        >
                        <v-card-title>Water Bottle</v-card-title>
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
                                Шинэ
                                </v-chip>
                        <img class="recommend"
                            src="~/assets/recommend/jersey.png"
                        >
                        <v-card-title>Jersey</v-card-title>
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
                                Шинэ
                                </v-chip>
                        <img class="recommend"
                            src="~/assets/recommend/sweetshirt-woman.png"
                        >
                        <v-card-title>Sweetshirt</v-card-title>
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
</template>

<script>
export default {

}
</script>

<style>
    .v-chip {
        position: absolute;
        top: 5px;
    }
    .container-title {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        margin: 30px 50px 20px 50px;
    }
    .recommend {
        width: 260px;
        height: 250px;
    }
</style>