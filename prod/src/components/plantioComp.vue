<template>
<div>
  <div class="btn-center">
    <v-btn class="mx-1" fab dark v-on:click="propri">
      <v-icon dark> mdi-plus </v-icon>
      <p class="text-btn">propriedade</p>
    </v-btn>
    </div>
    <div class="input-group">
      <input type="text" placeholder="Comprimento">
      <input type="text" placeholder="Area">
      <input type="text" placeholder="Largura">
    </div>
    <div class="input-group">
      <input type="text" placeholder="Clone">
      <input type="text" placeholder="Plantas ativas">
      <input type="text" placeholder="Plantas inativas">
    </div>
     <div class="input-group">
      <input type="text" placeholder="Plantas dominadas">
    </div>
</div>
</template>

<script>
export default {
  name: 'plantioComp'
}
</script>

<style scoped>
.v-btn {
  background-color: rgba(1, 149, 247, 255);
  color: aliceblue;
  display: flex;
  height: 2rem;
  font-size: 11px;
  text-align: center;
}
.btn-center{
    margin-left: 67%;
    margin-top: 1rem;
}
input{
  margin-top: 1rem;
  padding-left: 4px;
  margin-left: 1rem;
  background-color: white;
  border:solid rgba(216,216,216,255) 1.3px;
  border-radius: 0.3rem;
  color: rgb(34, 34, 34);
  font-size: 12px;
}
.input-group{
  margin-left: 3rem;
}
</style>
