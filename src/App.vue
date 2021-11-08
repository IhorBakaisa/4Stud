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

<style lang='scss'>
@import './assets/styles';
</style>
