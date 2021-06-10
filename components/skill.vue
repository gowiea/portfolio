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
</style>
