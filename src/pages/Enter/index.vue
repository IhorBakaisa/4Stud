<template>
    <div>
        <LoginIcon class="icon4"/>
        <div class="blockEnt">
            <h3 >Вхід</h3>
            <input type="text" placeholder="Логін">
            <br>
            <br>
            <input type="text" placeholder="Пароль">
            <br>
            <br>
            <button>Увійти</button>
        </div>
    </div>
</template>

<script>
import { LoginIcon } from "@vue-hero-icons/outline"
    export default {
        name: 'Enter',
components: { LoginIcon
  }
    }
</script>

<style lang="css" scoped>
.blockEnt {
    border:2px Gold  solid;
    width: 20%;
    background: black;
    margin-left: 40%;
    padding: 0.5%;
}

button {
  border-color: black;
  color: Black;
  box-shadow: 0 0 40px 40px Gold inset, 0 0 0 0 Gold;
  -webkit-transition: all 150ms ease-in-out;
  transition: all 150ms ease-in-out;
  margin-bottom: 10px;
}

button:hover {
  box-shadow: 0 0 10px 0 DarkOrange inset, 0 0 10px 4px DarkOrange;
}
.icon4{
  position: absolute;
  color: gold;
  margin-top: 25px;
  margin-left: 35px;
}
</style>