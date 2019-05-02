<template>
<!-- Note there can only be 1 root element-->
<!-- Use @ to register events -->
  <button @click="buttonClicked">{{text}}</button>
</template>

<script>
export default {
  name: "MyButton",
  props: {
    text: String // Props are parameters that can be passed to the component
  },
  methods: {
    // All functions used inside the component/template can be defined here
    buttonClicked($event) {
      alert('button clicked');
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<!-- Add lang="scss" to allow sass -->
<style scoped lang="scss">
button {
  background-color: aqua;
}
</style>
