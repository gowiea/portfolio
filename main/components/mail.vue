<template>
    <button @click="change()">
        {{text}}
    </button>
</template>
<script>
export default {
    name: "mail",
    data(){
        return{
            text: "Cliquez ici"
        }
    },
    methods: {
        change(){
            this.text="gowiea@hotmail.fr"
        }
    }
}
</script>
<style>
button{
border: none;
  color: rgb(9, 28, 31);
  background-color: rgb(206, 250, 237);
  opacity: 100%;
  width: 10em;
  margin: auto;
  display: block;
  font-size: 1.5em;
  transition: 0.3s;
  text-decoration: none;
  padding-right: 0.06em ;
}
</style>