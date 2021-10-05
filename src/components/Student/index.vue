<template>
    <div class="conteiner">
        <div>
            <span><img :src="photoStudent" alt="Photo not found" class="img"></span>
        </div>
        <div class="info"> 
            <span class="infoStudent">{{nameStudent}}</span><br>
            <span class="infoStudent">{{studentAddress}}</span>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Student',
        props: {
            photoStudent: {
                type: String,
                default: null
            },
            nameStudent: {
                type: String,
                default: null
            },
            studentAddress: {
                type: String,
                default: null
            }
        }
    }
</script>

<style lang="css" scoped>
.conteiner {
    display: grid;
    grid-template-columns: 1fr 2fr;
    border-radius: 10px;
    width: 300px;
    margin: 20px;
    padding: 10px;
    border: 2px solid black;
}
.info {
    margin-left: 10px;
    border: 2px solid gray;
    border-radius: 10px;
}
.img {
    width: 150px;
}
.infoStudent {
    margin-left: 30px
}
</style>