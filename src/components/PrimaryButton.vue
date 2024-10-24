<script>
export default {
  name: "PrimaryButton",
  props: {
    text: ""
  }
}
</script>

<template>
  <button class="primary-button">{{ text }}</button>
</template>

<style scoped>
.primary-button {
  background-color: white;
  opacity: 70%;
  border-radius: 26px;
  padding: 16px 23px 16px 23px;
  border: none;
  font-size: 16px;
  cursor: pointer;
}

/* Tablets entre 601px a 1024px */
@media only screen and (min-width: 601px) and (max-width: 1024px) {
  .primary-button {
    font-size: 30px;
    width: 18rem;
  }
}
</style>