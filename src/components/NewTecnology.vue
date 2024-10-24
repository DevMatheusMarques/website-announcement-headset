<script>
import ImageCard from "@/components/ImageCard.vue";

export default {
  name: "NewTecnology",
  components: {ImageCard},
  data() {
    return {
      imageUrl: '/assets/new-tecnology.png',
      imageDescription: 'Foto da nova tecnologia'
    }
  }
}
</script>

<template>
  <section>
    <div class="container">
      <div class="container-new-tecnology">
        <span class="title-new-tecnology">Nova Tecnologia</span>
        <p class="description-new-tecnology">As publicações de notícias oferecem uma ótima maneira de informar os clientes sobre novos produtos e
          serviços, eventos, prêmios e muito mais. As publicações de notícias oferecem uma ótima maneira de informar os
          clientes sobre novos produtos e serviços, eventos, prêmios e muito mais.
        </p>
      </div>
      <div class="image-new-tecnology">
        <ImageCard :image="imageUrl" :description="imageDescription"/>
      </div>
    </div>
  </section>
</template>

<style scoped>

/* Celulares até 600px */
@media only screen and (max-width: 600px) {
  .container {
    max-width: 100%;
    height: 100%;
    background-image: url("../assets/background2.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    gap: 2rem;
    color: #000000;
    box-shadow: inset 0 0 20px -20px #000000;
  }

  .container-new-tecnology {
    width: 80%;
    text-align: justify;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 2rem;
  }

  .title-new-tecnology {
    font-size: 30px;
    padding-top: 4rem;
  }

  .description-new-tecnology {
    font-size: 15px;
  }

  .image-new-tecnology {
    width: 80%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding-bottom: 4rem;
  }
}

/* Tablets entre 601px a 1024px */
@media only screen and (min-width: 601px) and (max-width: 1024px) {
  .container {
    max-width: 100%;
    height: 100%;
    background-image: url("../assets/background2.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    gap: 8rem;
    color: #000000;
    box-shadow: inset 0 0 20px -20px #000000;
  }

  .container-new-tecnology {
    width: 80%;
    text-align: justify;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 4rem;
  }

  .title-new-tecnology {
    font-size: 70px;
    padding-top: 10rem;
  }

  .description-new-tecnology {
    font-size: 35px;
  }

  .image-new-tecnology {
    width: 80%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding-bottom: 10rem;
  }
}

/* Computadores desktop a partir de 1025px */
@media only screen and (min-width: 1025px) {
  .container {
    max-width: 100%;
    height: 100dvh;
    background-image: url("../assets/background2.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #000000;
    box-shadow: inset 0 0 20px -20px #000000;
  }

  .container-new-tecnology {
    width: 30%;
    margin-left: 6%;
    text-align: justify;
  }

  .title-new-tecnology {
    font-size: 50px;
  }

  .description-new-tecnology {
    font-size: 20px;
  }

  .image-new-tecnology {
    width: 50%;
    margin-right: 6%;
    margin-left: 10%;
  }
}
</style>