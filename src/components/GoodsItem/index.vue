<template>
     <div class="blockgoods">
        <div> 
            <div class="cardPhoto"><img :src="goods.photo" alt="photo" class="photo"></div> <br> 
            <div class="cardInfo">{{goods.name}}</div> <br>
            <div class="cardInfo">{{goods.price}} грн</div>
            <button>Переглянути</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'GoodsItem',
        props: {
            goods: {
                type: Object,
                default: ()=>({})
            },
        },
    }
</script>

<style lang="css" scoped>

.blockgoods {
    width: 250px;
    border: 4px solid rgb(0, 0, 0);
    margin: 3px;
    border-radius:  20px;
    border-color:gold ;
    color: black;
    background: white;
}

.photo {
    width: 200px;
    height: 200px;
}

.cardPhoto {
    margin-top: 20px;
    margin-left: 5px;
    height: 200px;
}

.cardInfo {
    border: 2px solid black;
    color: Gold;
    border-color: gold;
    background: black;
    margin-left: 40px;
    margin-right: 40px;
    border-radius: 5px;
}

button {
  border-color: gold;
  color: #fff;
  box-shadow: 0 0 0 0 black;
  -webkit-transition: all 150ms ease-in-out;
  transition: all 150ms ease-in-out;
  border-radius: 6px;
  background-color: black;
  margin-left: 0px;
  padding: 10px;
  color: gold;
  text-decoration: none;
  margin-top: 25px;
  border: 2px solid gold;
  width: 175px;
}
button:hover {
  box-shadow: 0 0 10px 0 gold inset, 0 0 10px 4px gold;
}

</style>