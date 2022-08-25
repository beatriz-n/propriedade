<template>
  <v-app>
    <v-main class="body">
      <v-sheet class="box-container"
  width="600"
>
      <h4>Propriedade:</h4>
<v-sheet
  color="white"
  height="400"
  width="555"
>
<CamposComp></CamposComp>
</v-sheet>
<BtnAdd></BtnAdd>
</v-sheet>
    </v-main>
  </v-app>
</template>

<script>
import CamposComp from './components/camposComp.vue'
import BtnAdd from './components/btnAdd.vue'

export default {
  name: 'App',
  components: {
    CamposComp,
    BtnAdd
  },

  data: () => ({
    //
  })
}
</script>
<style scoped>
.v-sheet{
  margin-left: 3.4%;
  margin-top: 3%;
  padding-top: 1%;
   border:solid rgba(216,216,216,255) 1.3px;
    border-radius: 0.1rem;
    padding-bottom: 1rem;
}
.box-bottom{
  margin-top: 1rem;
  margin-bottom: 2rem;
}
a{
  /* color: rgb(106, 193, 244); */
  color: rgb(253, 127, 127);
}
p{
  text-align: center;
  font-size: small;
  padding-top: 1.3rem;
}
.box-container{
  background-color:rgba(250,250,250,255);
  margin-left: 35%;
}
.body{
  background-color: rgba(245,245,245,255);
}
h4{
  margin-left: 1rem;
  color: rgb(62, 62, 62);
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}
</style>
