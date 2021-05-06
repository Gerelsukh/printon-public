<template>
  <div>
      <Headerdef/>

    <v-container class="container">
        <v-row no-gutters>
            <v-col>
                <div class="title-div">
                <p class="mt-10 ml-10">Үйлчилгээний 3 төрлөөс өөрт тохирох нөхцөлөө сонгоорой</p>
                </div>
            </v-col>
            <v-col>
                <div>
                    <img class="cover" src="~/assets/price/cover1.png">
                </div>
            </v-col>
        </v-row>
    </v-container>
        <v-container
        class="my-10"
        >
        <div class="service-title mb-5"><span class="pricing">Business Plan</span></div>
        <v-row
            no-gutters
            class="mx-5"
            >
            <v-col>
            <v-card
                class="pa-2 mx-auto mb-3"
                width="360"
                outlined
                color="#F7F7F7"
            >
            <v-list-item three-line>
        <v-list-item-content>
            <v-list-item-title class="headline mb-5">
                <span class="Title">Эрх чөлөө</span>
            </v-list-item-title>
            <v-list-item-subtitle class="mb-5"><span class="subtitle">Бренд үүсгэж бизнес ээ эхлүүлэх</span></v-list-item-subtitle>
            <div class="mb-5"><span class="text" >MNT 0 / сар</span></div>
            <div class="mb-10"><span class="detail">Хязгааргүй Brand үүсгэх</span></div>
            <v-btn
            depressed
            color="#25BC3D"
            >
            <span class="btn">Эхлүүлэх</span>
            </v-btn>
        </v-list-item-content>
        </v-list-item>
            </v-card>
            </v-col>
            <v-col>
            <v-card
                class="pa-2 mx-auto mb-3"
                width="360"
                outlined
                color="#F7F7F7"
            >
            <v-list-item three-line>
        <v-list-item-content>
            <v-list-item-title class="headline mb-5">
                <span class="Title">Premium</span>
            </v-list-item-title>
            <v-list-item-subtitle class="mb-5"><span class="subtitle">Бренд үүсгэж бизнес ээ өргөжүүлэх</span></v-list-item-subtitle>
            <div class="mb-5"><span class="text" >MNT 50.000 / сар</span></div>
            <div class="mb-10"><span class="detail">Хязгааргүй Brand үүсгэх</span></div>
            <v-btn
            depressed
            color="#25BC3D"
            >
            <span class="btn">Эхлүүлэх</span>
            </v-btn>
        </v-list-item-content>
        </v-list-item>
            </v-card>
            </v-col>
            <v-col>
            <v-card
                class="pa-2 mx-auto mb-3"
                width="360"
                outlined
                color="#F7F7F7"
            >
            <v-list-item three-line>
        <v-list-item-content>
            <v-list-item-title class="headline mb-5">
                <span class="Title">Enterprise</span>
            </v-list-item-title>
            <v-list-item-subtitle class="mb-5"><span class="subtitle">Бренд үүсгэж борлуулалт нэмэх</span></v-list-item-subtitle>
            <div class="mb-5"><span class="text" >MNT ~ / сар</span></div>
            <div class="mb-10"><span class="detail">Хязгааргүй Brand үүсгэх</span></div>
            <v-btn
            depressed
            color="#25BC3D"
            >
            <span class="btn">Эхлүүлэх</span>
            </v-btn>
        </v-list-item-content>
        </v-list-item>
            </v-card>
            </v-col>
        </v-row>
        </v-container>
    
            <v-container
            class="my-10"
            >
            <div class="service-title mb-5 mt-n5"><span class="price-feature">Багц болгоны гол онцлог</span></div>
            <v-row
                no-gutters
                class="mx-5"
                >
                <v-col>
                    <ul>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Бренд үүсгэх</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Захиалга үүсгэх</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">24/7 дэмжлэг</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Мэдлэгийн сан</span></div></li>
                    </ul>
                </v-col>
                <v-col>
                    <ul>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Бренд үүсгэх</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Захиалга үүсгэх</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">24/7 дэмжлэг</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Мэдлэгийн сан</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Бүх бүтээгдэхүүнд 20% хямдрал</span></div></li>
                    </ul>
                </v-col>
                <v-col>
                    <ul>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Бренд үүсгэх</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Захиалга үүсгэх</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">24/7 дэмжлэг</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Мэдлэгийн сан</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Бүх бүтээгдэхүүнд 20% хямдрал</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Өөрийн веб үүсгэх</span></div></li>
                        <li><div class="mt-2"><v-icon size="30" color="black">mdi-check-circle-outline</v-icon><span class="feature-text pl-2">Брэнд хэрэглэгчийн дэмжлэг</span></div></li>
                    </ul>
                </v-col>
            </v-row>
            </v-container>

            <v-container
            class="my-10"
            >
            <div class="d-flex flex-row mb-5 ml-4 mt-n8"><span class="pricing">Түгээмэл асуултууд</span></div>
            <v-row
                no-gutters
                class="mx-5"
                >
                <v-col>
                    <div class="mt-3"><span class="question">Lorem ipsum</span></div>
                    <div class="mt-3"><span class="answer">Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.</span></div>
                </v-col>
                <v-col>
                    <div class="mt-3"><span class="question">Lorem ipsum</span></div>
                    <div class="mt-3"><span class="answer">Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.</span></div>
                </v-col>
            </v-row>
            <v-row
                no-gutters
                class="mx-5 mt-2"
                >
                <v-col>
                    <div class="mt-3"><span class="question">Lorem ipsum</span></div>
                    <div class="mt-3"><span class="answer">Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.</span></div>
                </v-col>
                <v-col>
                    <div class="mt-3"><span class="question">Lorem ipsum</span></div>
                    <div class="mt-3"><span class="answer">Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.</span></div>
                </v-col>
            </v-row>
            <v-row
                no-gutters
                class="mx-5"
                >
                <v-col>
                    <div class="mt-3"><span class="question">Lorem ipsum</span></div>
                    <div class="mt-3"><span class="answer">Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.</span></div>
                </v-col>
                <v-col>
                    
                </v-col>
            </v-row>
            </v-container>

      <Footer/>

  </div>
</template>

<script>
import  Headerdef  from "~/components/default-header.vue";
import  Footer  from "~/components/footer.vue";
export default {
    components: {
        Headerdef,
        Footer
    },
}
</script>

<style scoped>
.header + .container {
    margin-top: 100px;
}
.question{
    font-family: 'Roboto';
    font-size: 25px;
    font-weight: 700;
}
.answer{

}
li{
    list-style: none;
}
.feature-text{
    color: black;
}
.price-feature{
    font-family: 'Roboto';
    font-size: 20px;
    font-weight: 600;
}
.pricing{
    font-family: 'Roboto';
    font-size: 40px;
    font-weight: 600;
}
.service-title{
    width: auto;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
}
.cover {
    width: 450px;
    height: 350px;
}
.title-div p{
    font-weight: 700;
    font-size: 40px;
    font-family: 'Roboto';
    color: black;
    line-height: 1.2;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
}
.Title{
    font-family: 'Roboto';
    font-size: 30px;
    font-weight: 700;
}
.text{
    font-family: 'Roboto';
    font-size: 25px;
    font-weight: 600;
}
.subtitle{
    font-family: 'Roboto';
    color: black;
}
.detail{
    font-family: 'Roboto';
    color: black;
}
.btn{
    font-family: 'Roboto';
    color: white;
}
.v-card{
    border-color: black;
}
</style>