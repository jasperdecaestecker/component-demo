<template>
<!-- Template is mandatory for all vue components -->
    <h1>{{ text }}</h1>
</template>

<script>
// Script is not always needed, sometimes embedding a single HTML component is enough
// Styles are also optional (Button.vue) has a working style example
export default {
  name: "TalmundoHeader",
  props: {
    text: String // Props are parameters that can be passed to the component
  },
};
</script>
