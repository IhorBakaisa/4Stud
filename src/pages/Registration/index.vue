<template>
    <div>
        <UserAddIcon class="icon5"/>
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
import { UserAddIcon } from "@vue-hero-icons/outline"
    export default {
        name: 'Registration',
 components: { UserAddIcon
  }
    }
</script>
