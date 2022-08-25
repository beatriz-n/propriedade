<template>
<div class="border">
  <form action="" @submit="checkform">
  <div class="input-group">
      <input type="text" placeholder="Nome">
      <input type="number" placeholder="Clone">
      <input type="number" placeholder="Plantas dominadas">
    </div>
    <div class="input-group">
      <input type="number" placeholder="Plantas ativas">
      <input type="number" placeholder="Plantas inativas">
    </div>
    <div class="input-group">
      <input v-model.number="comp" type="number" placeholder="Comprimento em metros">
      <input v-model.number="larg" type="number" placeholder="Largura em metros">
    </div>
<v-row no-gutters>
        <v-row
        >
           <v-btn v-on:click.prevent="calc"
  elevation="2"
  x-small
>calcular</v-btn>
        </v-row>
        <br>
        <v-row
          class="pa-2"
        >
         <p>A area serà: {{area}} m²</p>
        </v-row>
    </v-row>
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
    calc () {
      this.area = this.comp * this.larg
    }
  }
}
</script>

<style scoped>
.border{
  border:solid rgba(216,216,216,255) 1.3px;
  border-radius: 0.3rem;
  margin: 1rem;
  padding-bottom: 1rem;
}
.v-row{
  margin-left: 2rem;
   margin-top: 7px;
   display: flex;
   align-items: baseline;
}
.v-btn{
   background-color: rgba(1, 149, 247, 255);
   height: 1.5rem;
   color: aliceblue;
   font-size: 11px;
  text-align: center;
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
