<template>
    <div>
      <MenuIcon class="icon2"/>
      <SwitchHorizontalIcon class="icon3"/>
        <div class="sort">
            <p> Вибрати товар за <select size="1" class="select">
            <option value="1">ціною</option>
            <option value="2">датою </option>
            </select>
            <input type="submit" value="Відсортувати" class="butsort"></p>
        </div>
        <div class="categories">
            <p id="catg">Категорії</p>
            <button class="btnCategories">
                Реферати
            </button>
            <br>
            <br>
            <button class="btnCategories">
                Конспекти
            </button>
            <br>
            <br>
            <button class="btnCategories">
                Лабораторні
            </button>
            <br>
            <br>
            <button class="btnCategories">
                Самостійні
            </button>
            <br>
            <br>
            <button class="btnCategories">
                Контрольні
            </button>
            <br>
            <br>
            <button class="btnCategories">
                Індивідуальні
            </button>
            <br>
            <br>
            <button class="btnCategories">
                Курсові
            </button>
        </div>
        <div class="mainList">
            <div class="listGoods">
            <goods-item v-for="goods in getGoodsList" :key="goods.id"
            :goods="goods"
            />
            </div>
        </div>
    </div>
</template>

<script>
    import GoodsItem from "@/components/GoodsItem";
    import { mapGetters } from "vuex"
    import { MenuIcon } from '@iconicicons/vue'
    import { SwitchHorizontalIcon } from "@vue-hero-icons/outline"
    export default {
        name: 'GoodsList',
        components: {
            GoodsItem, MenuIcon,SwitchHorizontalIcon
        },
        computed: {
            ...mapGetters(['getGoodsList'])
        },
    }
</script>

<style >
.mainList{
    border: 2px solid;
    margin-left: 210px;
    background-color: black;
    margin-top: -465px;
    width: 1279px;
    margin-bottom: 5px;
}

.listGoods {
    background-color: black;
    width: 1235px;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-auto-rows: 400px;
    grid-column-gap: 10px;
    grid-row-gap: 35px;
    margin-left: 45px;
    padding-top: 30px;
    padding-bottom: 30px;
}
.btnCategories{
    height: 50px;
    width: 190px;
    padding-top: 10px ;
    border-radius: 4px;
    background-color: gold;
    color: Black;
    text-decoration: none;
}

.btnCategories:hover {
  background-color: DarkOrange; 
  color: white;
}
.categories{
    margin-top: -58px;
    color: gold;
    border: 2px solid;
    width: 200px;
    height: 525px;
    background-color: black;
    margin-left: -10px;
}
.butsort{
  border-radius: 4px;
  border-color: black;
  background: gold;
 -webkit-transition: box-shadow 300ms ease-in-out, color 300ms ease-in-out;
  transition: box-shadow 300ms ease-in-out, color 300ms ease-in-out;
}
.butsort:hover{
    box-shadow: 0 0 40px 40px DarkOrange inset;
}
.select{
    background: LemonChiffon;
}
.sort{
    border: 2px solid;
    width: 1279px;
    margin-left: 210px;
    background-color: black;
}
.icon2{
  position: absolute;
  color: gold;
  margin-top: 15px;
  margin-left: -800px;
}
.icon3{
  position: absolute;
  color: gold;
  margin-top: 15px;
  margin-left: -160px;
}
</style>