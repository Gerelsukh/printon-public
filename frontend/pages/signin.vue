<template>
        <div class="signin-section">
            <div class="form">
                <div class="">
                  <v-icon size="40" @click="$router.push('/products')">mdi-close</v-icon>
                    <div class="img"><img src="../assets/logo/printon.png"></div>
                    <div class="headline">
                        <p>Тавтай морил</p>
                    </div>
                    <div class="text">
                    <v-text-field
                    label="Email" 
                    type="email"
                    dense
                    outlined
                    color="#25BC3D"></v-text-field>
                    <v-text-field
                    label="Password"
                    :append-icon="show ? 'mdi-eye-off' : 'mdi-eye'"
                    :type="show ? 'text' : 'password'"
                    hint="At least 8 characters"
                    @click:append="show = !show"
                    dense
                    outlined
                    color="#25BC3D"></v-text-field>
                    <div class="forgot-pass"><a>Нууц үгээ мартсан уу?</a></div>
                    <v-checkbox
                    class="nopadding"
                    color="#25BC3D"
                    v-model="checkbox"
                    label="Сануулах уу?"></v-checkbox>
                    </div>
                  </div>
                    <div class="signin-btn">
                        <v-btn class="signin-btn-item" color="#25BC3D">Sign in</v-btn>
                    </div>
                    <div class="subline center"> Шинэ хэрэглэгч үү? &nbsp;<a class="signup" href="/signup">Sign Up</a></div>
              </div>
            <div class="image">     
            </div>
        </div>
</template>

<script>
  export default {
    data () {
      return {
        show: false,
        password: 'Password',
        
      }
    },
  }
</script>

<style lang="scss" scoped>
    .form {
        padding: 40px;
    }
    .signup {
        color: #25BC3D;
    }
    .forgot-pass a {
      color: #25BC3D;
      font-weight: 500;
      text-decoration: none;
      font-size: 13px;
    }
    a {
        text-decoration: none;
        color: #25BC3D;
        font-weight: 700;
    }
    .center {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        padding-top: 10px;
        padding-bottom: 10px;
    }
    .headline p {
        text-transform: uppercase;
        font-weight: 700;
        font-size: 20px;
        color: black;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
    }
    .subline {
        color: black;
    }
    .signin-btn {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
    }
    .signin-btn-item {
        width: 50%;
        color: white;
        text-transform: capitalize;
    }
    .image {
        background-position: center;
        background-size: cover;
        background-image: url("../assets/signin/signin.png");
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
       
    }
    .signin-section{
      background-color: white;
    }
    img {
        width: 204px;
        height: 52px;
    }
    .img {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
    } 
    .v-text-field{
      width: 300px;
    }
    .v-btn {
      width: 300px;
    }
    .text{
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
    i {
      cursor: pointer;
    }
  @media only screen and (min-width:961px){
    .signin-section{
      height: 100%;
      display: grid;
      grid-template-columns: 1fr 1fr;
      border-radius: 5px;
      overflow: hidden;

    }
    .image{
      padding-bottom: 60px;
    }
    .form{
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
  }
    @media only screen and (min-width: 601px) and (max-width:960px) {
      .signin-section{
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
      .signin-section{
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