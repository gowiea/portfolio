<template>
  <div class="bg-blue-light">
    <h1 class="mail">Mon profil vous intéresse ? Contactez moi dès maintenant !</h1>
    <mail />
  </div>
</template>
<script>
import mail from "../components/mail.vue";
export default{
  components: { mail },
    data() {
        return{

        }
    }
}
</script>
<style>
.mail{
  margin: 3em 0em;
}
</style>
