<script>
export default {
  name: "SecondaryButton",
  props: {
    text: ""
  }
}
</script>

<template>
  <button class="secondary-button">{{ text }}</button>
</template>

<style scoped>
.secondary-button {
  background-color: white;
  border-radius: 26px;
  padding: 16px 23px 16px 23px;
  border: none;
  font-weight: bold;
  font-size: 16px;
  cursor: pointer;
}

/* Tablets entre 601px a 1024px */
@media only screen and (min-width: 601px) and (max-width: 1024px) {
  .secondary-button {
    font-size: 30px;
    width: 18rem;
  }
}
</style>