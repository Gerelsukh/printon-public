<template>
  <div>
      <Headerdef/>

      <v-container class="mt-4">
        <v-row no-gutters>
              <v-col 
                cols="12"
                sm="6"
                md="8"
                > 
                <div class="product-img">
                <div class="img-detail ml-12">
                    <v-card
                        tile
                        outlined
                        class="mx-auto mb-2"
                        width="60"
                        height="60"
                        >
                    <img class="detailimg" src="~/assets/recommend/hoodie.png">
                    </v-card>

                    <v-card
                        tile
                        outlined
                        class="mx-auto mb-2"
                        width="60"
                        height="60"
                        >
                    <img class="detailimg" src="~/assets/recommend/hoodie.png">
                    </v-card>

                    <v-card
                        tile
                        outlined
                        class="mx-auto mb-2"
                        width="60"
                        height="60"
                        >
                    <img class="detailimg" src="~/assets/recommend/hoodie.png">
                    </v-card>

                    <v-card
                        tile
                        outlined
                        class="mx-auto mb-2"
                        width="60"
                        height="60"
                        >
                    <img class="detailimg" src="~/assets/recommend/hoodie.png">
                    </v-card>

                </div>
                <div class="main-img ml-n16">
                    <v-card
                        tile
                        outlined
                        class="mb-2"
                        width="400"
                        height="400"
                        >
                    <img class="mainimg" src="~/assets/recommend/hoodie.png">
                    </v-card>
                </div>
                </div>
              </v-col>

              <v-col
                cols="6"                    
                md="4"
                >
                <v-list
                subheader
                three-line
                >
                <v-subheader>T-Shirt</v-subheader>

                <v-list-item>
                    <v-list-item-content>
                    <v-list-item-title><b>Богино ханцуйтай V хүзүүтэй цамц</b></v-list-item-title>
                        100% хөвөн
                        <br>Хөнгөн даавуу
                        <br>Жижиглэн худалдаа
                        <br>Шошгон дээр оёсон
                        <br>Хэмжээ алдахгүй
                    </v-list-item-content>                    
                </v-list-item>
                <v-btn class="ml-5" color="#25BC3D" @click="$router.push('/print')">Customise</v-btn>
                </v-list>
              </v-col>
          </v-row>
      </v-container>
      <div class="product-info">
          <v-container>
              <v-row>
                  <v-col class="ml-16"><h2>Бүтээгдэхүүний Тухай</h2></v-col>
              </v-row>
          </v-container>
          <v-container>
              <v-row>
                  <v-col 
                    cols="6"                    
                    md="4"
                    class="ml-12"
                ><h3>Дэлгэрэнгүй</h3></v-col>
                  <v-col 
                    cols="10"
                    sm="4"
                    md="6">Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.</v-col>
              </v-row>
          </v-container>
          <v-divider width="1000" class="divider"></v-divider>
          
          <v-container>
              <v-row>
                  <v-col 
                    cols="6"                    
                    md="4"
                    class="ml-12"
                ><h3>Онцлог</h3></v-col>
                  <v-col 
                    cols="10"
                    sm="4"
                    md="6">
                    <v-row>
                    <v-col>
                    <div class="feature">
                        <img class="featured" src="~/assets/Landing-page/feature1.png">
                        <p class="feature-desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore</p>
                    </div>
                    </v-col>
                    <v-col>
                    <div class="feature">
                        <img class="featured" src="~/assets/Landing-page/feature1.png">
                        <p class="feature-desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore</p>
                    </div>
                    </v-col>
                    <v-col>
                    <div class="feature">
                        <img class="featured" src="~/assets/Landing-page/feature1.png">
                        <p class="feature-desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore</p>
                    </div>
                    </v-col>
                    <v-col>
                    <div class="feature">
                        <img class="featured" src="~/assets/Landing-page/feature1.png">
                        <p class="feature-desc">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore</p>
                    </div>
                    </v-col>
                    </v-row>
                </v-col>
              </v-row>
          </v-container>
          <v-divider width="1000" class="divider"></v-divider>

          <v-container>
              <v-row>
                  <v-col 
                    cols="6"                    
                    md="4"
                    class="ml-12"
                ><h3>Тусламж үйлчилгээний заавар</h3></v-col>
                  <v-col 
                    cols="10"
                    sm="4"
                    md="6">
                    <v-row>
                    <v-col>
                    <div class="feature1">
                        <div class="float-icon">
                        <img class="instructed" src="~/assets/Landing-page/feature1.png">
                        <img class="instructed" src="~/assets/Landing-page/feature1.png">
                        <img class="instructed" src="~/assets/Landing-page/feature1.png">
                        <img class="instructed" src="~/assets/Landing-page/feature1.png">
                        </div>
                        
                    </div>
                    
                    </v-col>
                    <div>
                            <p class="instruction">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore</p>
                        </div>
                    </v-row>
                </v-col>
              </v-row>
          </v-container>
          <v-divider width="1000" class="divider"></v-divider>

          <v-container>
              <v-row>
                  <v-col 
                    cols="6"                    
                    md="4"
                    class="ml-12"
                ><h3>Хэмжээ</h3></v-col>
                  <v-col 
                    cols="10"
                    sm="4"
                    md="6">
                    <img class="size" src="~/assets/products-detail/size.png">
                    </v-col>
              </v-row>
          </v-container>
          <v-divider width="1000" class="divider"></v-divider>
      </div>

      <Recommend/>
  </div>
</template>

<script>
import  Headerdef  from "~/components/default-header.vue";
import  Recommend  from "~/components/recommend.vue";
export default {
    components :{
        Headerdef,
        Recommend
    }
}
</script>

<style>
.size {
    width: 650px;
    height: 250px;
}
.float-icon .instructed{
    float: left;
    margin-right: 5px;
}
.instructed {
    width: 30px;
    height: 30px;
    margin-bottom: 5px;
}
.divider {
    margin-left: 150px;
}
.feature-desc {
  font-weight: 400;
  font-size: 13px;
}
.featured {
  width: 48px;
  height: 45px;
  margin-bottom: 15px;
}
.feature {
  width: 237px;
  height: 150px;
}
.mainimg {
    width: 400px;
    height: 400px;
}
.v-card {
    border-color: #25BC3D !important;
}
.detailimg {
    width: 60px;
    height: 60px;
}
.product-img {
    height: 100%;
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr;
    overflow: hidden;
}
.img-detail {
    width: 250px;
    height: auto;
    margin-top: 100px;
}
.main-img {
    width: 525px;
    height: auto;
}
</style>