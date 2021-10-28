<template>
  <div id="app">
    <HomeIcon class="icon1"/>
    <div class="header">
      <router-link to="/"><img src="logo.jpg" class="logo"></router-link>
      <!-- <router-link to="/aboutGoods" class="pages">Інформація про товар</router-link> -->
      <router-link to="/myAccount" class="pages myOffice">Мій кабінет</router-link>
      <router-link to="/registration" class="pages myRegistration">Реєстрація</router-link>
      <router-link to="/enter" class="pages mySignIn">Увійти</router-link>
      <br>
      <br>
    </div>
    <div class="content">
      <router-view></router-view>
    </div>
    <div class="footer">
        <div class='followUs'>
          <GlobeAltIcon class="icon8"/>
          <GlobeIcon class="icon9"/>
      <h3 style="color:#FFFFFF" >FOLLOW US</h3>
      <p> <a href="">Facebook</a></p>
      <p> <a href="">Instagram</a></p>
        </div>
        <div class='contacts'>
      <h3 style="color:#FFFFFF">CONTACTS</h3>
      <PhoneIcon class="icon6"/>
      <MailIcon class="icon7"/>
      <p>Call us now: 0123-456-789</p>
      <p>Email:<a href=""> forstudents-admin@gmail.com</a></p>
        </div>
    </div>
  </div>
</template>

<script>
import { HomeIcon } from '@iconicicons/vue'
import { PhoneIcon } from "@vue-hero-icons/solid"
import { MailIcon } from "@vue-hero-icons/solid"
import { GlobeAltIcon } from "@vue-hero-icons/outline"
import { GlobeIcon } from "@vue-hero-icons/outline"
export default {
  name: 'App',
  components: {  HomeIcon,PhoneIcon,MailIcon,GlobeAltIcon,GlobeIcon
  }
}
</script>

<style>
#app {
  background-image: url(https://images.wallpaperscraft.ru/image/single/chernyj_temnyj_fraktal_149686_300x168.jpg) ;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: Gold	;
  margin: -8px;
}
.logo{
  margin-left: -1300px;
  padding: -150px;
  height: 35px;
  width: 100px;
}
.pages {
  border-radius: 4px;
  background-color: Gold;
  margin-left: 20px;
  padding: 10px;
  color: Black;
  text-decoration: none;
}
.pages:hover {
  background-color: DarkOrange; 
  color: white;
}
.header, .content, .footer {
  padding: 10px;
}
.header, .footer {
  border:2px Gold  solid;
  background: Black;
}
.home {
  position: absolute;
  left: 0;
  margin-left: 10%;
}
.myOffice {
  position: absolute;
  right: 0;
  margin-right: 15%;
}
.myRegistration {
  position: absolute;
  right: 0; 
  margin-right: 7%;
}
.mySignIn {
  position: absolute;
  right: 0; 
  margin-right: 20px;
}
.header {
  padding-bottom: 0%;
  padding-top: 1%;
}
a {
    text-decoration: none;
    color: Gold; /* Цвет обычной ссылки */
    padding: 2px; /* Поля вокруг текста */
   }
   a:hover {
    text-decoration: none; /* Убираем подчеркивание */
    color: #fff; /* Цвет ссылки при наведении на нее курсора мыши */  
    background: Goldenrod; /* Цвет фона */
   }
/* .content {
}*/
.footer {
flex: 0 0 auto;
} 
.followUs{
  margin: 10px;
  border:3px Gold  solid; 
  width: 150px; 
  position: absolute;
  left: 0; 
  margin-left: 550px;
}
.contacts{
  border:3px Gold  solid; 
  width: 250px; 
  left: 0; 
  margin-left: 810px;
}
.icon1{
  position: absolute;
  color: gold;
  margin-top: 18px;
  margin-left: -730px;
}
.icon6{
  position: absolute;
  color: gold;
  margin-top: -5px;
  margin-left: -120px;
}
.icon7{
  position: absolute;
  color: gold;
  margin-top: 35px;
  margin-left: -100px;
}
.icon8{
  position: absolute;
  color: gold;
  margin-top: 55px;
  margin-left: -65px;
}
.icon9{
  position: absolute;
  color: gold;
  margin-top: 90px;
  margin-left: -65px;
}
</style>
