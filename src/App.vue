<template>
  <div id="app">
    <div class="header">
      <router-link to="/"  ><img src="logo.jpg" class="logo"></router-link>
      <!-- <router-link to="/aboutGoods" class="pages">Інформація про товар</router-link> -->
      <!-- <router-link to="/addGoods" class="pages">Додати товар</router-link> -->
      <router-link to="/myAccount" class="pages myOffice">Мій кабінет</router-link>
      <router-link to="/registration" class="pages myRegistration">Реєстрація</router-link>
      <router-link to="/registration" class="pages mySignIn">Увійти</router-link>
      <br>
      <br>
    </div>
    <div class="content">
      <router-view></router-view>
    </div>
    <div class="footer">
        <div class='followUs'>
      <h3 style="color:#FFFFFF" >FOLLOW US</h3>
      <p> <a href="">Facebook</a></p>
      <p> <a href="">Instagram</a></p>
        </div>
        <div class='contacts'>
      <h3 style="color:#FFFFFF">CONTACTS</h3>
      <p>Call us now: 0123-456-789</p>
      <p>Email:<a href=""> forstudents-admin@gmail.com</a></p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: Gold	;
  margin-top: 10px;
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
</style>
