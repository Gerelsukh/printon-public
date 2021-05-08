<template>
  <div>
    <Header/>
    <div class="container"></div>
    <div class="lcontainer1">
        <div class="form">
                <div class="">
                    <div class="headline">
                        <p>Онлайнаар өөрийнхөө хүссэн бараа бүтээгдэхүүнийг <br>бүтээцгээе</p>
                    </div>
                    <div class="sub-headline">
                        <p>Шинэлэг загвар, түргэн үйлчилгээ</p>
                    </div>                    
                    <!-- href="http://localhost:3000/products" -->
                    <div class="signin-btn">
                        <v-btn class="signup-btn-item" color="#25BC3D" href="/products">Бренд үүсгэх</v-btn>
                    </div>
                    <div class="subline"> &nbsp; Үнэгүй - Хялбар - 100+ Бүтээгдэхүүн</div>
              </div>
         </div>
         <div class="image"><img class="land-image" src="~/assets/Landing-page/LAND.png"></div>
      </div>

      <div class="lcontainer2">
        <div class="title"><h2>Та PrintOn ашиглан юу хийж чадах вэ?</h2></div>

        <v-container class="">
        <v-row class="mb-1">
        <v-col
          cols="12"
          sm="4"
        >
        <v-card
        class="mx-auto"
        max-width="344"
        height="320"
        >
      <img class="whatchucan"
        src="~/assets/Landing-page/create.jpg"
        height="200px"
      >

      <v-card-title>
        Бренд үүсгэ
      </v-card-title>

      <v-card-subtitle>
        Манайд байршсан бүх бүтээгдэхүүнээс та хүссэн бараагаа сонгож захиалгаа өгөх боломжтой.
      </v-card-subtitle>
        </v-card>
      </v-col>
      <v-col
          cols="12"
          sm="4"
        >
        <v-card
        class="mx-auto"
        max-width="344"
        height="320"
        >
      <img class="whatchucan"
        src="~/assets/Landing-page/sell.jpg"
        height="200px"
      >

      <v-card-title>
        Борлуулах
      </v-card-title>

      <v-card-subtitle>
       Та захиалгаа гар дээрээ авснаар борлуулах боломжтой.
      </v-card-subtitle>
        </v-card>
      </v-col>
      <v-col
          cols="12"
          sm="4"
        >
        <v-card
        class="mx-auto"
        max-width="344"
        height="320"
        >
      <img class="whatchucan"
        src="~/assets/Landing-page/house.png"
        height="200px"
      >

      <v-card-title>
        Хүргэлтийн үйлчилгээ
      </v-card-title>

      <v-card-subtitle>
        Түргэн шуурхай тань гарт бүтээгдэхүүн хүргэгдэх болно.
      </v-card-subtitle>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
      </div>

      <div class="lcontainer3">
        <div class="title"><h2>Загварлаг бүтээгдэхүүн, хүссэнээрээ өөрчил</h2></div>

        <v-container class="">
          <v-row
            class="mb-6"
          >
            <v-col>
              <v-card
                tile
                class="mx-auto"
                max-width="208"
                height="280"
                >
              <img class="product"
                src="~/assets/Landing-page/t-shirt.png"
              >
              <v-card-title>Подволк</v-card-title>
              </v-card>
            </v-col>
            <v-col>
              <v-card
                tile
                class="mx-auto"
                max-width="208"
                height="280"
                >
              <img class="product"
                src="~/assets/Landing-page/hoodie.png"
              >
              <v-card-title>Малгайтай цамц</v-card-title>
              </v-card>
            </v-col>
            <v-col>
              <v-card
                tile
                class="mx-auto"
                max-width="208"
                height="280"
                >
              <img class="product"
                src="~/assets/Landing-page/mugs.png"
              >
              <v-card-title>Аяга</v-card-title>
              </v-card>
            </v-col>
            <v-col>
              <v-card
                tile
                class="mx-auto"
                max-width="208"
                height="280"
                >
              <img class="product"
                src="~/assets/Landing-page/caps.png"
              >
              <v-card-title>Малгай</v-card-title>
              </v-card>
            </v-col>
            <v-col>
              <v-card
                tile
                class="mx-auto"
                max-width="208"
                height="280"
                >
              <img class="product"
                src="~/assets/Landing-page/case.png"
              >
              <v-card-title>Утасны кейс</v-card-title>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      <div class="all-product-btn">
      <v-btn outlined color="black" href="/products">Бүх бүтээгдэхүүн</v-btn>
      </div>
    </div>

    <div class="lcontainer4">
      <div class="title"><h2>Хэрхэн өөрийн бренд үүсгэх вэ?</h2></div>
      <p class="tutorial">Хүссэн бүтээгдэхүүн ээ сонгоод хүссэн бренд ээ үүсгэ</p>
      <div class="youtube">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/gtriTzmghgg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>

      <div class="step">
            <v-container>
              <v-row class="mt-10" no-gutters>
                <v-col>
                  <img class="howto" src="~/assets/Landing-page/step1.png">
                  <v-btn class="ml-8 ma-4" outlined fab>1</v-btn>
                  <p>Бүтээгдэхүүн сонгох</p>
                </v-col>
                <v-col>
                  <img class="howto" src="~/assets/Landing-page/step2.png">
                  <v-btn class="ml-8 ma-4" outlined fab>2</v-btn>
                  <p>Өөрийн бренд үүсгэх</p>
                </v-col>
                <v-col>
                  <img class="howto" src="~/assets/Landing-page/step3.png">
                  <v-btn class="ml-9 ma-4" outlined fab>3</v-btn>
                  <p class="ml-5">Захиалга өгөх</p>
                </v-col>
                <v-col>
                  <img class="howto" src="~/assets/Landing-page/step4.png">
                  <v-btn class="ml-9 ma-4" outlined fab>4</v-btn>
                  <p>Гар дээрээ хүргүүлэх</p>
                </v-col>
              </v-row>
            </v-container>
      </div>
    </div>

    <div class="lcontainer5">
      <div class="title"><h2>PrintOn онцлог</h2></div>
        <v-container class="">
          <v-row no-gutters class="ml-11">
            <v-col>
              <div class="feature">
                <img class="featured" src="~/assets/Landing-page/feature1.png">
                <p class="feature-desc">100+ онцгой бүтээгдэхүүн</p>
                <p>Цамц, юүдэн, гутал, цүнх, оймс, малгай, утасны хайрцаг, аяга, наалт...</p>
              </div>
            </v-col>
            <v-col>
              <div class="feature">
                <img class="featured" src="~/assets/Landing-page/feature2.png">
                <p class="feature-desc">Ашиглахад үнэгүй</p>
                <p>Урьдчилгаа төлбөр шаардагдахгүй бөгөөд захиалга өгөхдөө л төлбөр төлөх шаардлагатай</p>
              </div>
            </v-col>
            <v-col>
              <div class="feature">
                <img class="featured" src="~/assets/Landing-page/feature3.png">
                <p class="feature-desc">Тоо ширхэг харгалзахгүй</p>
                <p>Бараа бүтээгдэхүүний тоо ширхэг заахгүй бөгөөд хүссэн хэмжээгээр захиалгаа өгөөрэй</p>
              </div>
            </v-col>
            <v-col>
              <div class="feature">
                <img class="featured" src="~/assets/Landing-page/feature4.png">
                <p class="feature-desc">Захиалгат брэнд</p>
                <p>Хүссэн лого, зургаа бидэнд өгснөөр зөвхөн өөрийн нэрийн бүтээгдэхүүнтэй болоорой</p>
              </div>
            </v-col>
            <v-col>
              <div class="feature">
                <img class="featured" src="~/assets/Landing-page/feature5.png">
                <p class="feature-desc">Тусламж</p>
                <p>Цамц, юүдэн, гутал, цүнх, оймс, малгай, утасны хайрцаг, аяга, наалт...</p>
              </div>
            </v-col>
            <v-col>
              <div class="feature">
                <img class="featured" src="~/assets/Landing-page/feature6.png">
                <p class="feature-desc">Хүргэлт үйлчилгээ</p>
                <p>Таны захилгат бараа бүтээгдэхүүнийг түргэн шуурхай хүргэж өгөх болно</p>
              </div>
            </v-col>
          </v-row>
        </v-container>      
    </div>

    <div class="lcontainer6">
      <div class="title"><h2>Үйлчлүүлэгчдийн бүтээсэн Бренд</h2></div>
          
    </div>
    <Footer/>
  </div>

</template>

<script>
import  Header  from "~/components/header.vue";
import  Footer  from "~/components/footer.vue";
export default {
  components :{
    Header,
    Footer
  }
}
</script>

<style scoped>
 .header + .container{
  margin-top: 80px;
}
.customer {
  border: 1px solid #c7c7c7 !important;
}
.feature-desc {
  font-weight: 700;
  font-size: 20px;
}
.featured {
  width: 48px;
  height: 45px;
  margin-bottom: 15px;
}
.feature {
  width: 365px;
  height: 240px;
}
.step {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  margin-left: 150px;
}
.howto {
  height: 118px;
  width: 121px;
}
.youtube {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  margin: 20px;
}
.tutorial {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  font-family: 'Roboto';
}
.all-product-btn {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
}
.lcontainer6 {
  width: 100%;
  height: auto;
}
.lcontainer5 {
  width: 100%;
  height: auto;
  border-bottom: 1px solid#9C9C9C;
}
.lcontainer4 {
  width: 100%;
  height: auto;
  border-bottom: 1px solid#9C9C9C;
}
.lcontainer3 {
  width: 100%;
  height: auto;
  border-bottom: 1px solid#9C9C9C;
}
.lcontainer2 {
  width: 100%;
  height: auto;
  border-bottom: 1px solid#9C9C9C;
}
.whatchucan {
  width: 344px;
  height: 200px;
}
.product {
  width: 208px;
  height: 200px;
  background-color: #F7F7F7;
}
.title {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  margin: 50px 50px 20px 50px;
}
.land-image {
  width: 552px;
  height: 500px;
}
.headline p{
    font-weight: 700;
    font-family: 'Roboto';
    font-size: 35px;
    color: black;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    margin-right: 100px;
    line-height: 1.2;
}
.sub-headline p{
    font-weight: 500;
    font-family: 'Roboto';
    font-size: 15px;
    color: #312F2F;
}
.subline {
    font-weight: 500;
    font-family: 'Roboto';
    font-size: 15px;
    color: #9C9C9C;
    margin-top: 20px;
}
.form{
  margin-left: 100px;
}
.form {
  width: 100%;
  height: 100%;
}
.lcontainer1 {
  width: 100%;
  height: 300px;
  border-bottom: 1px solid#9C9C9C;
}
 @media only screen and (min-width:961px){
    .lcontainer1 {
      height: 100%;
      display: grid;
      grid-template-columns: 1fr 1fr;
      overflow: hidden;
    }
    .form{
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
    .image{
      padding-bottom: 60px;
    }
  }
    @media only screen and (min-width: 601px) and (max-width:960px) {
      .lcontainer1 {
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
      }
      .image {
        display: none;
      }
    }
    @media only screen and (max-width: 600px) {
      .lcontainer1 {
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
      }
      .image{
        display: none;
      }
    }
</style>