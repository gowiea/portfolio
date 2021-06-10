<template>
    <div>
    <div class="bg-blue-light">
      <h1>Mes réalisations</h1>
      <div
        class="contain"
        v-for="(realisation, index) in realisations"
        :key="index"
      >
        <realisation
          :img="realisation.img"
          :title="realisation.title"
          :link="realisation.link"
          :text="realisation.text"
        />
      </div>
    </div>
  </div>
</template>
<script>
import realisation from "../components/realisation.vue";
    export default {
  data() {
    return {
      realisations: [
        {
          img: require("~/static/equipage.png"),
          title: "L'équipage",
          link: 'https://equipage.team',
          text:
            "Développement du front-end, choix de la direction graphique"
        },
        {
          img: require("../static/bourgy.svg"),
          title: "Bertrand's Quest",
          link: 'https://bourgysquest.netlify.app',
          text:
            "Développement de la logique, équilibrage du jeu"
        },
      ],
    };
  }
};
</script>
<style scoped>
h1{
    text-align: center;

}
p{
    text-align: center;
    font-size: 1em;
}
</style>