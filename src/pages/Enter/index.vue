<template>
    <div>
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
    export default {
        name: 'Enter',

    }
</script>

<style lang="css" scoped>
.blockEnt {
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
</style>