<template>
  <div class="e-nuxt-container">
    <div class="e-nuxt-content">
      <h1>Off Grid solar calculator</h1>
      <h3>
        This calculator will give you a baseline idea of the size solar system
        you need to satisfy your energy consumption
      </h3>
    </div>
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
.e-nuxt-container {
  min-height: calc(100vh - 50px);
  background: linear-gradient(to right, #ece9e6, #ffffff);
  font-family: Helvetica, sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.e-nuxt-content {
  width: 400px;
  padding-top: 100px;
  padding: 20px;
  border-bottom: 1px solid #397c6d;
}

.e-nuxt-links {
  padding: 100px 0;
  display: flex;
  justify-content: center;
}

.e-nuxt-button {
  color: #364758;
  padding: 5px 20px;
  border: 1px solid #397c6d;
  margin: 0 20px;
  border-radius: 15px;
  font-size: 1rem;
}

.e-nuxt-button:hover {
  cursor: pointer;
  color: white;
  background-color: #397c6d;
}
</style>
