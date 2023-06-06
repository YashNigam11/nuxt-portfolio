<template>
  <v-app dark>
    <v-main>
      <div class="bottom-navigation">
        <div class="nav-item">
          <a href="/">Home</a>
        </div>
        <div class="nav-item">
          <a href="/about">About</a>
        </div>
        <div class="nav-item">
          <a href="/contact">Contact Us</a>
        </div>
      </div>
      <Nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {};
</script>

<style scoped>
.bottom-navigation {
  background-color: teal;
  display: flex;
  height: 56px;
}

.nav-item {
  flex-grow: 1;
  display: flex;
  align-items: center;
  justify-content: center;
}

.nav-item a {
  font-size: 20px;
  text-decoration: none;
  color: white;
}
</style>
