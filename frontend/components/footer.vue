<template>
  <div class="footer">
    <div class="inner-footer">
      <div class="footer-logo">
          <img src="~/assets/logo/printon.png" alt="printon-logo">
      </div>
      <div class="footer-column">
      <v-container>
          <v-row>
              <v-col>
                <h3>Website</h3>
                  <ul class="footer-bar">
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Бүтээгдэхүүн</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Хэрхэн ажилладаг</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Үйлчилгээ</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Блог</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Мэдлэгийн сан</span></div></a></li>
                </ul>
              </v-col>
              <v-col>
                <h3>Бүтээгдэхүүн</h3>
                  <ul class="footer-bar">
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Подволк</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Малгайтай цамц</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Цамц</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Аяга</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Усны сав</span></div></a></li>
                </ul>
              </v-col>
              <v-col>
                <h3>PrintOn</h3>
                  <ul class="footer-bar">
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Бидний тухай</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Холбоо барих</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Биднийг дагах</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Ажлын байр</span></div></a></li>
                    <li class="footer-item"><a class="footer-link" href="#"><div class="footer-link-item"><span>Мерчандайз</span></div></a></li>
                </ul>
              </v-col>
          </v-row>
      </v-container>
        </div>
        <div class="footer-end">
            <p class="copy">&copy; 2021 PrintiOn, Inc. All rights reserved.</p>
        </div>
      </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.copy {
    padding-top: 5px;
    padding-left: 5px;
    font-size: 12px;
}
.footer-end {
    width: 100%;
    height: 30px;
    background-color: #C4C4C4;
}
h3 {
    margin-left: 20px;
}
.footer-item .footer-link {
    font-weight: 500;
    font-family: 'Roboto';
    font-size: 15px;
    color: #696969;
    line-height: 2;
    transition: color 0.5s ease;
    height: 100%;
}
.footer-item .footer-link:hover {
    color: #25BC3D;
}
.footer-link {
    text-decoration: none;
}
.footer-bar {
    list-style: none;
    width: 100%;
    height: 100%;
}
.footer-column {
    margin-top: 30px;
}
.inner-footer {
    width: 1000px;
}
.footer {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    margin-top: 50px;
}
img {
  height: 52px;
  width: 204px;
}
</style>