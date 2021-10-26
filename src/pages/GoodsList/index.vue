<template>
    <div>
 <p> Вибрати товар за<br> <select size="1" class="select">
<option value="1">ціною</option>
<option value="2">датою </option>
</select></p>
   <p><input type="submit" value="Відсортувати" class="butsort"></p>
  
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style >
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
</style>