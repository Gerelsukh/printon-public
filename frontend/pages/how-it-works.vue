<template>
    <div>
        <Header/>

        <v-container class="container">
            <v-row justify="center" class="mt-16"><h1>Хэрхэн ажилладаг вэ</h1></v-row>
            <v-row justify="center" class="mt-16"><p style="text-align: center;"><span style="color: black;">Манай платформ нь хувийн бренд үүсгэх хүсэлтэй хүн болгоны ажлыг хөнгөвчлөх зорилготой <br>бренд үүсгэх, захиалах, хэвлэх, хүргэлт гэсэн ажлуудыг агуулсан систем юм.</span></p></v-row>
            <v-row justify="center" class="mt-16"><v-btn color="#25BC3D" x-large width="200" href="/products"><span style="color:white; font-fmily: 'Roboto'">Эхлэх</span></v-btn></v-row>
            <v-row justify="center" style="margin-top: 150px"><h2>Бидний санал болгох 5 үйлчилгээ</h2></v-row>
            <v-row
                no-gutters
                style="margin-top: 100px"
                class="mx-16"
                >
                <v-col>
                    <div class="gifdiv"><img class="gif" src="~/assets/how-work/pick.gif"></div>
                </v-col>
                <v-col>
                    <div class="desc">
                        <div class="innerdesc">
                            <div class="mb-10"><h1>Сонгох</h1></div>
                            <div class="mt-16"><p><span class="text">Манайд байгаа нийт 300 гаруй бүтээгдэхүүнээс хүссэн бүтээгдэхүүнээ сонгох боломжтой. Өөрт тохирох, өөрт таалагдсан, өөрийн нэрийн бүтээгдэхүүнд хамгийн ойр чанартай бүтээгдэхүүнээс сонголтоо хийгээрэй.</span></p></div>
                        </div>
                    </div>
                </v-col>
                </v-row>
                <v-row
                no-gutters
                style="margin-top: 100px"
                class="mx-16"
                >
                <v-col>
                    <div class="desc">
                        <div class="innerdesc-right">
                            <div class="mb-10"><h1>Бренд үүсгэх</h1></div>
                            <div class="mt-16"><p><span class="text">Та хүссэн бараагаа хүссэнээр өөрчилж загвараа гаргах боломжтой юм. Та үүсгэсэн бүтээгдэхүүнээ урьдчилаад харах боломжтой бөгөөд бид танд хамгийн чанартай, шинэлэг бүтээгдэхүүн санал болгож таны брендийг бий болгоход туслах болно.</span></p></div>
                        </div>
                    </div>
                </v-col>
                <v-col>
                    <div class="gifdiv"><img class="gif" src="~/assets/how-work/customize.gif"></div>
                </v-col>
                </v-row>
                <v-row
                no-gutters
                style="margin-top: 100px"
                class="mx-16"
                >
                <v-col>
                    <div class="gifdiv"><img class="gif" src="~/assets/how-work/mystore.gif"></div>
                </v-col>
                <v-col>
                    <div class="desc">
                        <div class="innerdesc">
                            <div class="mb-10"><h1>Миний дэлгүүр</h1></div>
                            <div class="mt-16"><p><span class="text">Миний дэлгүүр хэсэгт таны үүсгэсэн бүтээгдэхүүн таныг устгах хүртэл хадгалагдах болно. Тоо ширхэг өөрчлөх, өнгө солих, загвараа шинээр хийх боломж танд өгөх болно.</span></p></div>
                        </div>
                    </div>
                </v-col>
                </v-row>
                <v-row
                no-gutters
                style="margin-top: 100px"
                class="mx-16"
                >
                <v-col>
                    <div class="desc">
                        <div class="innerdesc-right">
                            <div class="mb-10"><h1>Хүргэлт</h1></div>
                            <div class="mt-16"><p><span class="text">Таны захиалсан бараа бүтээгдэхүүнийг маш болгоомжтой таны гар дээр түргэн шуурхай 100% сэтгэл ханамжтай хүргэж өгөх болно.</span></p></div>
                        </div>
                    </div>
                </v-col>
                <v-col>
                    <div class="gifdiv"><img class="gif" src="~/assets/how-work/fullfill.gif"></div>
                </v-col>
                </v-row>
        </v-container>

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
  margin-top: 100px;
}
.gif {
    height: 350px;
    width: 350px;
}
.gifdiv {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
}
.innerdesc-right{
    padding: 0  30px 20px 20px;
}
.innerdesc {
    padding: 20px  30px 20px 0;
}
.text {
    font-size: 18px;
}
</style>