<template>
<div>
    <div class="btn-center">
    <v-btn class="mx-1" fab dark v-on:click.prevent="propri" type="submit">
      <v-icon dark> mdi-plus </v-icon>
      <p class="text-btn">Plantio</p>
    </v-btn>
    </div>
    <PlantioComp></PlantioComp>
    <div v-for="box in boxes" :key="box.id" :value="box.tipo">
    </div>
    </div>
</template>
<script>
import PlantioComp from './plantioComp.vue'

export default {
  name: 'btnAdd',
  data () {
    return {
      boxes: [1, 2, 3],
      nextBox: ''
    }
  },
  methods: {
    propri: function () {
      // alert('aqui')
      /*       this.boxes.push({
        box: this.nextBox++
      }) */
    },
    components: { PlantioComp }
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
</style>
