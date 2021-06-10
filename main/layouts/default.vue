<template>
  <div>
    <div class="bg parent">
      <div class="enfant">
        <NuxtLink class="a" to="/" >Antoine Gowie</NuxtLink>
      </div>
      <div class="enfant">
        <NuxtLink class="link" to="/CV">CV</NuxtLink>
        <NuxtLink class="link" to="/portfolio">Portfolio</NuxtLink>
        <NuxtLink class="link" to="/contact">Contact</NuxtLink>
      </div>
    </div>
    <Nuxt />
    <div class="footer">
      <h3>Site créé par Antoine Gowie</h3>
    </div>
  </div>
</template>

<script></script>

<style>
.bg {
  background-color: rgb(42, 157, 143);
  min-height: 10em;
}
.footer {
  background-color: rgb(42, 157, 143);
  padding: 1em 0em;
}
.a {
  text-decoration: none;
  color: rgb(38, 70, 83);
  font-family: Halaney, serif;
  font-size: 5em;
  margin: 0.5em;
  transition: 0.3s;
}
.a:hover {
  text-decoration: none;
  color: rgb(38, 70, 83);
  font-family: Halaney, serif;
  font-size: 5.5em;
  margin: 0.5em;
}
.link {
  border: none;
  color: rgb(9, 28, 31);
  background-color: rgb(206, 250, 237);
  opacity: 0.7;
  width: 10em;
  margin: 1em 0em 1em 0em;
  font-family: Prisma, serif;
  font-size: 3em;
  transition: 0.3s;
  text-decoration: none;
  padding-right: 0.06em ;
}
.link:hover {
  border: none;
  color: rgb(9, 28, 31);
  background-color: rgb(206, 250, 237);
  opacity: 1;
  width: 10em;
  margin: 1em 0em 1em 0em;
  font-family: Prisma, serif;
  font-size: 3em;
  text-decoration: none;
  padding-right: 0.06em ;
}
h3{
  text-align: center;
  margin: 1em 0em;
}
</style>

<style scoped>
@font-face {
  font-family: Halaney;
  src: url("../assets/Halaney-Demo.otf");
}
@font-face {
  font-family: Prisma;
  src: url("../assets/Prisma.ttf");
}
.parent {
  display: grid;
}
.enfant {
  margin: auto;
  text-align: center;
}
@media only screen and (max-width: 600px) {
  .a {
    font-size: 2.5em;
  }
}
</style>
