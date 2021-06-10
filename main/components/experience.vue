<template>
    <div>
        <h1>
            {{title}}
        </h1>
         <p>
            {{date}}
        </p>
        <p>
            {{text}}
        </p>
    </div>
</template>
<script>
    export default{
        name:'experience',
        props:{
            title: String,
            date: String,
            text: String,
        },
        data(){
            return{
               
            }
        }
    }
</script>
<style scoped>
h1{
    text-align: center;
    font-size: 2em;
}
p{
    text-align: center;
    font-size: 1em;
}
</style>
