<template>
<div class="register">
<div class="form">
<div class="input-form">
    <input type="text" placeholder="Nome da propriedade">
    <input type="text" placeholder="Contato">
    <input type="text" placeholder="Localização completa">
    <input type="text" placeholder="Gerente">
    <input type="text" placeholder="Telefone">
    <input type="text" placeholder="Proprietário">
</div>
<v-row no-gutters>
        <v-row
          class="pa-3"
        >
           <v-btn  class="btn-register"
>salvar</v-btn>
        </v-row>
        <br>
        <v-row
          class="pa-3"
        >
         <v-btn  class="btn-danger"
>Cancelar</v-btn>
        </v-row>
    </v-row>
</div>
</div>
</template>
<script>
export default {
  name: 'camposComp'
}
</script>
<style scoped>
.register{
    align-items: center;
}
h1 {
    color: black;
    margin-bottom: 1rem;
}
h5{
    color: rgb(163, 163, 163);
    margin-right: 30px;
    margin-left: 30px;
}
.form {
    text-align: center;

}
.text-register, b{
   color: rgb(163, 163, 163);
font-size: 10px;
 margin-right: 25px;
    margin-left: 25px;
    display: inline-table;
}
.v-btn{
    display: flex;
     height: 1.5rem;
     margin-left: 10px;
     font-size: 10px;
     width: 14rem;
     margin-top: 1rem;
}
.btn-register{
     background-color: rgba(1,149,247,255);
     color: aliceblue;
     transition: .5s;
}
.btn-register:hover{
 background-color: transparent;
  color: rgb(0, 0, 0);
}
.btn-danger{
     background-color: red;
     color: aliceblue;
     transition: .5s;
}
.btn-danger:hover{
 background-color: transparent;
  color: rgb(0, 0, 0);
}
.v-divider{
margin-left: 10px;
margin-right: 10px;
}
.v-text-field{
    display: flex;
}
input{
    border:solid rgba(216,216,216,255) 1.3px;
    border-radius: 0.3rem;
    margin: 4px;
    background-color:rgba(250,250,250,255) ;
    width: 27rem;
    height: 2rem;
    color: rgb(34, 34, 34);
    font-size: 12px;
    padding-left: 0.7rem;
}
.input-form{
    padding-top: 1rem;
    padding-bottom: 1rem;
}
.v-row{
    padding-left: 1rem;
    padding-top: 2rem;
}
</style>
