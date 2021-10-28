<template>
    <div>
        <div class="myAccountInfo">
            <UserCircleIcon  class="icon11"/>
            <p id="cabinet">Мій кабінет</p>
            <UploadIcon class="icon10"/>
            <div class="timeoutPhoto">
                Загрузити <br>зображення
            </div>
            <p id="infoContacts">
                Прізвища Ім’я Побатькові <br>
                <br>Номер телефону: 0666666666 <br>
               <br> Пошта: Daybozhe@gmail.com <br>
            </p>
            <router-link to="/addGoods" class="pages" id="addAdvertisement">Додати товар</router-link><br>
            <ClipboardListIcon class="icon12"/>
            <p id="myAdvertisemen">
                Мої оголошення
            </p>
            <div id="Advertisemen">

            </div>

            
        </div>
        
    </div>
</template>

<script>
import { UploadIcon } from "@vue-hero-icons/outline"
import { UserCircleIcon } from "@vue-hero-icons/solid"
import { ClipboardListIcon } from "@vue-hero-icons/outline"
    export default {
     components: {  UploadIcon,UserCircleIcon,ClipboardListIcon
  }
    } 
    
</script>

<style lang="css" scoped>
.myAccountInfo{
    background-color: black;
    width: 1000px;
    height: 900px;
    margin-left: 350px;
    border: 2px solid;
}
.timeoutPhoto{
    width: 200px;
    height: 250px;
    background-color: gray;
    margin-left: 50px;
    margin-top: 50px;
    border: 2px solid;
}
#infoContacts{
    text-align: left;
    margin-top: -255px;
    margin-left: 300px;
    font-size: 18px;
    width: 400px;
}
#addAdvertisement{
  margin-left: 100px;
  border-color: black;
  color: Black;
  box-shadow: 0 0 40px 40px Gold inset, 0 0 0 0 Gold;
  -webkit-transition: all 150ms ease-in-out;
  transition: all 150ms ease-in-out;
  margin-bottom: 10px;
}

#addAdvertisement:hover {
 box-shadow: 0 0 10px 0 white inset, 0 0 10px 4px darkorange;
}
#myAdvertisemen{
    margin-top: 150px;
    text-align: center;
    font-size: 20px;
}
#Advertisemen{
    width: 900px;
    height: 500px;
    border: 2px solid;
    margin-left: 50px;
}
#cabinet{
    margin-top: 10px;
    text-align: center;
    font-size: 20px;
}
.icon10{
  position: absolute;
  color: gold;
  margin-top: 90px;
  margin-left: -360px;
}
.icon11{
  position: absolute;
  color: gold;
  margin-top: 10px;
  margin-left: 60px;
}
.icon12{
  position: absolute;
  color: gold;
  margin-top: 150px;
  margin-left: 80px;
}
</style>