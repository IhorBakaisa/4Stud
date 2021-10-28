<template>
    <div>
        <div class="myAccountInfo">
            <p id="cabinet">Мій кабінет</p>
            <div class="timeoutPhoto">
                Зображення
            </div>
            <p id="infoContacts">
                Прізвища Ім’я Побатькові <br>
                Номер телефону: 0666666666 <br>
                Пошта: Daybozhe@gmail.com <br>
            </p>
            <router-link to="/addGoods" class="pages" id="addAdvertisement">Додати товар</router-link><br>
            <p id="myAdvertisemen">
                Мої оголошення
            </p>
            <div id="Advertisemen">

            </div>

            
        </div>
        
    </div>
</template>

<script>
    export default {
        
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
}
#addAdvertisement{
    height: 50px;
    width: 190px;
    padding-top: 10px ;
    border-radius: 4px;
    background-color: gold;
    color: Black;
    text-decoration: none;
    margin-left: -280px;
}

#addAdvertisement:hover {
  background-color: DarkOrange; 
  color: white;
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

</style>