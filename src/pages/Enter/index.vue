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

