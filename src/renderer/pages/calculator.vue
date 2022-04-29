<template>
  <div class="e-nuxt-container">
    <div class="">
      <h1>Calculator</h1>
      <h3 class="e-nuxt-content">
        This calculator will give you a baseline idea of the size solar system
        you need to satisfy your energy consumption
      </h3>
      <h4 class="e-nuxt-content">
        We need your zip code in the setup page. This will not get stored or
        sent to our servers for data collection of analyitcs
      </h4>
    </div>
    <div class="e-nuxt-container">Expected loads</div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  components: {},
  data() {
    return {
      externalContent: "",
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
