<template>
  <div class="e-nuxt-container">
    <div class="e-nuxt-content">
      <h1 calss="e-nuxt-content">Location</h1>
      <h3>
        What is your zip code? Your zip code will give us the best solar
        radiation information specific to your location.
      </h3>
    </div>
    <div class="e-nuxt-content">
      <v-text-field
        v-model="zip_entry"
        label="Enter yor zip code here:"
        contained
        counter
        maxlength="5"
        clearable
        :rules="[rules.counter]"
        @keyup.enter="fetchzip(zip_entry)"
      />
    </div>
  </div>
</template>

<script>
import * as zipdata from "../assets/zipcode";
export default {
  name: "SetupPage",
  components: {},
  data() {
    return {
      zip_entry: "",
      externalContent: "",
      rules: {
        counter: (value) => value.length == 5 || "Provide a full 5 digit zip",
      },
    };
  },
  methods: {
    fetchzip(zip) {
      console.log(zip);
    },
  },
  mounted() {
    console.log("loading zip data");
    console.log(zipdata);
  },
};
</script>

<style>
</style>
