<script>
export default {
  name: "CardImage",
  props: {
    image: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    }
  }
}
</script>

<template>
  <div class="card-new-tecnology">
    <img :src="image" :alt="description" class="image">
  </div>
</template>

<style scoped>
.card-new-tecnology {
  width: 100%;
  height: 80%;
  display: flex;
  align-items: center;
  justify-content: center;
  border-top-right-radius: 100px;
  overflow: hidden;
}

.image {
  width: 100%;
  height: 80%;
  object-position: center;
  margin-top: 5px;
}

</style>