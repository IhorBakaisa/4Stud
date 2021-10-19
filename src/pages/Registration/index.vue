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
    background: rgb(235, 235, 235);
    margin-left: 40%;
    padding: 0.5%;
}

button {
  border: 1px solid rgb(196, 195, 195);
  border-radius: 4px;
  background-color: rgb(196, 195, 195);
  margin-left: 1%;
  padding: 10px;
  color: black;
  text-decoration: none;
  margin-bottom: 2%;
}
</style>