<template>
  <div id="app">
    <div class="header">
      <br>
      <router-link to="/" class="pages">Головна</router-link>
      <router-link to="/aboutGoods" class="pages">Інформація про товар</router-link>
      <router-link to="/addGoods" class="pages">Додати товар</router-link>
      <router-link to="/myAccount" class="pages">Мій кабінет</router-link>
      <router-link to="/registration" class="pages">Реєстрація</router-link>
      <br>
      <br>
    </div>
    <div class="content">
      <router-view></router-view>
    </div>
    <div class="footer">
      <h3>Footer</h3>
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
  color: #2c3e50;
  margin-top: 10px;
}

.pages {
  border-radius: 4px;
  background-color: rgb(153, 153, 153);
  margin-left: 20px;
  padding: 10px;
  color: white;
  text-decoration: none;
}

.header, .content, .footer {
  padding: 10px;
}

.header, .footer {
  background: rgb(235, 235, 235);
}

/* .header {

}

.content {

}

.footer {

} */
</style>
