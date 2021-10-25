<template>
    <div class ="container">
        <div>
       <img :src = "imgSrc" class ="img">
    </div>
    <div class ="info">
        <div>{{title}}</div>
        <div>{{author}}</div>
        <div>{{price}}</div>
    </div>
        </div>
</template>

<script>

export default {
    name:'BookCard',
    props: {
        imgSrc: {
            type: String,
            default:null
        },
        tittle: {
            type : String,
            default:'No tittle'
        },
        author: {
            type : String,
            default:null
        },
        price: {
            type : Number,
            default:0
        },
    },

}
</script>
<style lang ="css" scoped>
.container {
    display: grid;
    grid-template-columns: 1fr 2fr;
    border: 2px solid greenyellow;
    border-radius:10px;
    width: 500px;
    margin:20px;
    padding:10px;
}
.info{
    border: 2px solid red;
    border-radius:10px;
}
.img{
    width: 150px;
}
</style>
