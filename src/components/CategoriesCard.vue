<script>
export default {
  name: "CategoriesCard",
  props: {
    imageUrl: {
      type: String,
      required: true
    },
    imageDescription: {
      type: String,
      required: true
    },
    cardTitle: {
      type: String,
      required: true
    },
    text: {
      type: String,
      required: true
    },
    fontSize: String
  },
  computed: {
    fonte() {
      let x = 'font-size:';
      return this.fontSize === null ? x + '23px;' : x + this.fontSize + ';'
    }
  }
}
</script>

<template>
  <div class="container-categories-card">
    <div class="container-image-category">
      <img :src="imageUrl" :alt="imageDescription" style="">
    </div>
    <span class="texts" :style="fonte" style="">{{ cardTitle }}</span>
    <p>{{ text }}</p>
  </div>
</template>

<style scoped>
.texts {
  font-weight: 500;
  text-align: center;
}
img {
  width: 100%;
  height: 100%;
  border-radius: 0 3.5rem 0 0;
}
.container-categories-card {
  height: 380px;
  width: 250px;
  border-radius: 0 3.5rem 0 3.5rem;
  background-color: white;
  padding: 1rem;
}

.container-image-category {
  border-top-right-radius: 100px;
  width: 204px;
  height: 204px;
}
</style>