<template>
    <div>
        <img :src="img">
        <h1>
            {{title}}
        </h1>
        <a :href="link" target=_blank>
            Voir le site
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
    display: block;
    margin: 1em auto;
}
h1{
    font-size: 2em;
}
p{
    font-size: 1em;
}
div{
    text-align: center;
}
a{
    color: black;
    opacity: 0.8;
}
a:hover{
    text-decoration: none;
    opacity: 1;
}
</style>
