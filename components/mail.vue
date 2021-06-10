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
            text: "Me contacter"
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

</style>