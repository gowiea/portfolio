<template>
  <div>
    <div class="bg-blue-dark">
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
      <NuxtLink class="more" to="/CV">En savoir plus</NuxtLink>
    </div>
    <div class="bg-blue-light">
      <h1>Mes compétences</h1>
      <div class="contain" v-for="(skill, index) in skills" :key="index">
        <skill :title="skill.title" :specs="skill.specs" />
      </div>
      <NuxtLink class="more" to="/portfolio">En savoir plus</NuxtLink>
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
        },
        {
          title: "Dev web",
          specs: ["HTML/CSS", "Javascript", "PHP", "Nuxt"]
        }
      ]
    };
  }
};
</script>

<style>
.bg-blue-light {
  background-color: rgba(206, 250, 237, 0.5);
  padding: 1em 0em 5em 0em;
}
.bg-blue-dark {
  background-color: rgb(206, 250, 237);
  padding: 1em 0em;
}
.contain {
  border: solid;
  border-width: 0.1em;
  margin: 1em 15em 0em 15em;
}
.more {
  text-align: center;
  display: block;
  text-decoration: none;
  color: black;
  margin: 0.5em 15em 0em 15em;
  font-size: 1.5em;
  font-weight: 600;
  background-color: rgb(42, 157, 143);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif,
    "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
}
.more:hover {
  text-align: center;
  display: block;
  text-decoration: none;
  color: black;
  margin: 0.5em 15em 0em 15em;
  font-size: 1.5em;
  background-color: rgb(42, 157, 143);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif,
    "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
}
h1 {
  text-align: center;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif,
    "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
    margin: 1em 0em;
}

@media only screen and (max-width: 1000px) {
  .contain {
    width: 32em;
    margin: 1em auto;
  }
  .more {
    width: 12em;
    margin: 0.4em auto;
  }
}
@media only screen and (max-width: 600px) {
  .contain {
    width: 15em;
    margin: 1em auto;
  }
  .more {
    width: 8em;
    margin: 0.4em auto;
  }
  .link{
    font-size: 2em;
  }
}
</style>
