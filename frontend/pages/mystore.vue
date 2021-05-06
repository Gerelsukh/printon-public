<template>
  <div>
      <Header/>

      <div class="mycontainer">
                <div class="search-bar mt-3">
                    <v-container>
                    <v-row>
                        <v-col>
                            <div class="store-title"><h2>Миний Дэлгүүр</h2> <v-icon class="mt-2">mdi-home</v-icon></div>                            
                        </v-col>
                        <v-col wider>
                        </v-col>
                    </v-row>
                </v-container>
            </div>
      </div>

      <div class="mycontainer">
                <div class="search-bar mt-3">
                    <v-container>
                    <v-row>
                        <v-col wider>
                            <v-card>                                
                                <v-text-field
                                    class="rounded-pill mx-5 pt-5"
                                    prepend-inner-icon="mdi-magnify"
                                    placeholder="Бараа, бүтээгдэхүүн, төрлөөр хайх"
                                    outlined
                                    dense
                                    color="#25BC3D"
                                    background-color="#F5F5F5"
                            ></v-text-field>
                            <div class="myorder">                            
                            <img class="product" src="~/assets/print/mystore.png">
                            <div>
                            <v-card-title>T-Shirt</v-card-title>
                             <v-card-text>
                                <div>Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
                                </v-card-text></div>
                                <v-btn>Захиалах</v-btn>
                                <v-btn>Өөрчлөх</v-btn>
                                </div>
                            </v-card>             
                        </v-col>
                    </v-row>
                </v-container>
            </div>
      </div>
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
.myorder {
    display: flex;
    flex-direction: row;
    justify-content: center;
}
.product {
    width: 100px;
    height: 100px;
    border: 1px solid #F7F7F7;
}
.store-title {
    display: flex;
    flex-direction: row;
    justify-content: left;
    align-items: flex-start;
    height: 100%;
}
.mycontainer {
    width: 100%;
    height: auto;
}
</style>