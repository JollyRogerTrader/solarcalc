<template>
  <header class="main-header">
    <nav>
      <div>
        <nuxt-link class="e-nuxt-button" to="/" exact> Home </nuxt-link>
      </div>
      <div>
        <nuxt-link class="e-nuxt-button" to="/calculator" exact>
          Calculator
        </nuxt-link>
      </div>
      <div>
        <nuxt-link class="e-nuxt-button" to="/Set_up" exact> Set-up </nuxt-link>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
};
</script>

<style scoped>
.main-header {
  height: 50px;
  display: flex;
  background-color: #364758;
}

nav {
  width: 100%;
  display: flex;
  justify-content: center;
}

nav div {
  height: 100%;
  margin: 0 20px;
  display: flex;
  align-items: center;
}

.e-nuxt-button {
  color: white;
  font-size: 1rem;
  font-weight: bold;
  text-transform: uppercase;
  padding: 5px 20px;
  border: 1px solid #397c6d;
  margin: 0 20px;
  border-radius: 15px;
  text-decoration: none;
}

.e-nuxt-button:hover {
  cursor: pointer;
  color: white;
  background-color: #397c6d;
}
</style>
