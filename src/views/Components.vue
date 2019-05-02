<template>
  <div class="components">

    <!-- Props are passed with the : sign. you can pass variables, string or any data -->
    <!-- Note that talmundo-button might not be the best name, but it cannot be button, because that is a reserved HTML element -->
    <talmundo-button :text="'Click here'"></talmundo-button>

    <!-- In this case titleText a variable defined in the data is used -->
    <!-- In template if you have components with multiple names it is seperated by a -  -->
    <talmundo-header :text="titleText"></talmundo-header>
  </div>
</template>

<script>
// @ is an alias to /src
// Import your component here to use in this file/component
import TalmundoButton from "@/components/TalmundoButton.vue";
import TalmundoHeader from "@/components/TalmundoHeader.vue";

export default {
  name: "home",
  components: {
    TalmundoButton,
    TalmundoHeader // List all components here so they can be used in the template
    // Components Files should always by written as PascalCase thus Capital start, 
    // Capital for each word
  },
  // Data can be used to set some local variables for this component
  data() {
    return {
      titleText: 'Title'
    }
  },
  created() {
    // This function is run when the component is created.
    console.log('Hey look my components.vue page is created')
  }
};
</script>
