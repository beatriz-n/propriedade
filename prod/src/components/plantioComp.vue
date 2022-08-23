<template>
<div>
  <form action="" @submit="checkform">
    <div class="input-group">
      <input v-model="comp" type="number" placeholder="Comprimento">
      <input v-model="larg" type="number" placeholder="Largura">
      {{larg}}

    </div>
    <div class="input-group">
      <input type="text" placeholder="Clone">
      <input type="text" placeholder="Plantas ativas">
      <input type="text" placeholder="Plantas inativas">
    </div>
     <div class="input-group">
      <input type="text" placeholder="Plantas dominadas">
      <input type="text" placeholder="Nome">
    </div>
    </form>
</div>
</template>

<script>

export default {
  name: 'plantioComp',
  data () {
    return {
      comp: null,
      larg: null,
      area: null
    }
  },
  methods: {
    checkform () {
      this.area = (this.comp + this.larg) / 2
    }
  }
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
    margin-left: 70.5%;
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
p{
  color: black;
}
</style>
