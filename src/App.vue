<template lang="pug">
  #app
    .container
      img(src="./assets/reto.jpg", alt="logo del formulario")
      h1 {{msg}}
      form(action="" method="")
        label Nombre
        input(type="text" name="nombre" )
        label Apellido
        input(type="text" name="apellido" )
        label Cargo
        input(type="text" name="cargo" )
        button(type='submit') ENVIAR

</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Registro estación Platzi'
    }
  }
}
</script>

<style lang="scss">
@import './scss/main.scss';
@import url('https://fonts.googleapis.com/css?family=Roboto:400,700&display=swap');
body{
  margin: 0;
  font-family: 'Roboto', sans-serif;
  background-color: white;
}
#app{
  display: flex;
  flex-direction: column;
  width: 400px;
  height: 409px;
  margin: 0 auto;
  justify-content: center;
  align-items: center;

}
.container{
  display: flex;
  flex-direction: column;
  width: 320px;
  height: 409px;
  margin: 0 auto;
  justify-content: center;
  align-items: center;
  font-family: 'Roboto', sans-serif;
  background-color: white;
}
img{
  width: inherit;
}
h1{
  color: #00bfd6;
  font-weight: 700;
  font-size: 29px;
  width: 100%;
  text-align: center;
}
form {
  width: inherit;
  display: inherit;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
input{
  border: none;
  border-bottom: 1px solid #ff9300;
  width: 100%;
}
label{
  color: #ff9300;
  align-self: flex-start;
  font-weight: 700;
  font-size: 8px;
  margin-top: 5px;
}
button {
  align-self: flex-end;
  background-color: #00bfd6;
  color: white;
  font-weight: bold;
  font-size: 15px;
  border: none;
  border-radius: 3px;
  width: 45%;
  margin-top: 20px;
  height: 40px;
  box-shadow: 1px 1px 2px grey;
}

</style>
