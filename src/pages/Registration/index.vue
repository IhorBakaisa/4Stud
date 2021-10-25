<template>
    <div>
        <div class="blockRegestration">
            <h3 >Реєстрація</h3>
            <input type="text" placeholder="П.І.Б">
            <br>
            <br>
            <input type="text" placeholder="Пошта">
            <br>
            <br>
            <input type="text" placeholder="Номер">
            <br>
            <br>
            <input type="text" placeholder="Логін">
            <br>
            <br>
            <input type="text" placeholder="Пароль">
            <br>
            <br>
            <input type="text" placeholder="Повтор паролю">
            <br>
            <br>
            <button>Зареєструватися</button>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="css" scoped>
.blockRegestration {
    width: 20%;
    background: Black;
    margin-left: 40%;
    padding: 0.5%;
}
button {
  border-color: OrangeRed;
  color: Black;
  box-shadow: 0 0 40px 40px Gold inset, 0 0 0 0 Gold;
  -webkit-transition: all 150ms ease-in-out;
  transition: all 150ms ease-in-out;
}

button:hover {
  box-shadow: 0 0 10px 0 DarkOrange inset, 0 0 10px 4px DarkOrange;
}
</style>