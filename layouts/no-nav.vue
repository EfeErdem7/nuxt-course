<template>
  <div class="container">
    <NuxtLink class="go-back" to="/">Go Back</NuxtLink>
    <Nuxt />
  </div>
</template>

<style scoped>
.container {
  padding-top: 5rem;
}
.go-back {
  color: rgb(231, 81, 43);
  font-weight: 700;
  transition: 0.150s;
  text-decoration: none;
}
.go-back:hover {
  color: rgb(255, 174, 154);
}
</style>