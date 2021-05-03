<template>
  <div>
      <Headerdef/>

    <v-container>
        <v-row no-gutters>
            <v-col>
                <div class="title-div">
                <p class="mt-10 ml-10">Үйлчилгээний 3 төрлөөс өөрт тохирох нөхцөлөө сонгоорой</p>
                </div>
            </v-col>
            <v-col>
                <div>
                    <img class="cover" src="~/assets/price/cover.png">
                </div>
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
    }
}
</script>

<style scoped>
.cover {
    width: 350px;
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
</style>