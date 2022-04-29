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
        v-model="zip"
        label="Enter your zip code here:"
        contained
        counter
        maxlength="5"
        clearable
        :rules="[rules.counter]"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "SetupPage",
  components: {},
  data() {
    return {
      zip: "",
      externalContent: "",
      rules: {
        counter: (value) => value.length == 5 || "Provide a full 5 digit zip",
      },
    };
  },
  methods: {
    openURL(url) {
      window.open(url);
    },
  },
};
</script>

<style>
</style>
