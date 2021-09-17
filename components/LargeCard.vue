<template>
  <NuxtLink :to="`/products/${card.id}`" class="card">
    <img
      :src="require(`@/assets/images/${card.image || 'fe1.jpg'}`)"
      alt="fe"
      class="image"
    />
    <h3 class="header">
      {{ card.title }}
    </h3>
    <p class="snippet">
      {{ card.snippet }}
    </p>
  </NuxtLink>
</template>

<script>
export default {
  props: ["card"],
};
</script>

<style scoped>
.card {
  width: 31.5%;
  height: 25rem;
  border: none;
  overflow: hidden;
  padding: 0;
  cursor: pointer;
  text-decoration: none;
  transition: all 0.2s ease-in-out;
}
.card:hover {
  transform: scale(1.015);
}
.card::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: 15px;
  width: 100%;
  height: 2px;
  background: rgb(243, 85, 45);
  transition: transform 200ms ease-in;
  transform: scale(0);
  transform-origin: left;
}
.card:hover::after {
  transform: scale(1);
}
.image {
  height: 65%;
  border-radius: 0.5rem;
}
.header {
  font-size: 1.15rem;
  margin-top: 0.4rem;
  color: black;
    text-decoration: none;
    transition: 0.2s;
}
.snippet {
  color: grey;
}
</style>