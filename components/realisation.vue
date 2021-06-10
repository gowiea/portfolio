<template>
    <div>
        <img :src="img">
        <h1>
            {{title}}
        </h1>
        <a :href="link" target=_blank>
            equipage.team
        </a>
        <p>
            {{text}}
        </p>
    </div>
</template>
<script>

    export default{
        name:'realisation',
        props:{
            img: String,
            title: String,
            link: String,
            text: String,
        },
        data(){
            return{
               
            }
        }
    }
</script>
<style scoped>
img{
    height: 5em;
}
h1{
    text-align: center;
    font-size: 2em;
}
p{
    text-align: center;
    font-size: 1em;
}
</style>
