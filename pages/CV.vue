<template>
  <div>
    <div class="bg-blue-light">
      <h1>Mes expériences</h1>
      <div
        class="contain"
        v-for="(experience, index) in experiences"
        :key="index"
      >
        <experience
          :date="experience.date"
          :title="experience.title"
          :text="experience.text"
        />
      </div>
    </div>
  </div>
</template>
<script>
import experience from "../components/experience.vue";
import skill from "../components/skill.vue";
export default {
  data() {
    return {
      experiences: [
        {
          title: "Création d'une marque de vêtements streetwear",
          date: "2018-2021",
          text:
            "Création d'une marque, d'un réseau de contact, du branding et de la distribution de celle-ci."
        },
        {
          title: "Chef de bar à Ronquière Festival",
          date: "2018",
          text: "Gestion d'une équipe pendant deux shifts de 8 heures"
        },
        {
          title: "Responsable de production pour Guizzi",
          date: "2018-2021",
          text: "Mise en place des tournages, cadrage, acting"
        },
        {
          title: "Participation au Space Office Hackaton",
          date: "2021",
          text:
            "Développement d'un jeu sur navigateur en moins de 48h en équipe, obtention de la 1ère place."
        }
      ],
      skills: [
        {
          title: "Infographie",
          specs: ["Photoshop", "Illustrator", "Gimp", "Lightroom"]
        }
      ]
    };
  }
};
</script>
<style scoped></style>
