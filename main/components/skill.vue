<template>
  <div>
    <h1>
      {{ title }}
    </h1>
    <ul>
      <li v-for="(spec,index) in specs" :key="index">
        {{ spec }}
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "skill",
  props: {
    title: String,
    specs: Array
  },
  data() {
    return {};
  }
};
</script>
<style scoped>
h1 {
  text-align: center;
  font-size: 2em;
}
p {
  text-align: center;
  font-size: 1em;
}
ul{
  text-align: center;
  list-style-type: none;
  padding: 0;
  margin: 0;
}
li{
  margin: 0em 0em 1em 0em;
}
</style>
