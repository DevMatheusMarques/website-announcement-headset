<script>
import ImageCard from "@/components/ImageCard.vue";

export default {
  name: "SpecialSupport",
  components: {ImageCard},
  data() {
    return {
      imageUrl: '/assets/celular.png',
      imageDescription: 'Foto do suporte especial'
    }
  }
}
</script>

<template>
  <section>
    <div class="container-support">
      <div class="container-special-support">
        <p class="title-support">Suporte Especial</p>
        <p class="description-support">Bateria de telefone com defeito? Notebook lento? Temos especialistas de tecnologia que podem ajudar você.</p>
        <p class="description-support">Visite nossas lojas!</p>

        <div>
          <p class="adress-title">NOSSAS LOJAS</p>
          <div class="containers-address">
            <p>Rua Qualquer, 123</p>
            <p>Qualquer Cidade, Estado, País</p>
            <p>(12) 34567-7890</p>
          </div>
          <div class="containers-address">
            <p>Rua Qualquer, 123</p>
            <p>Qualquer Cidade, Estado, País</p>
            <p>(12) 34567-7890</p>
          </div>
        </div>
      </div>
      <div class="image-support">
        <ImageCard :image="imageUrl" :description="imageDescription"/>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Celulares até 600px */
@media only screen and (max-width: 600px) {
  .container-support {
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
    gap: 4rem;
    color: #000000;
    box-shadow: inset 0 0 20px -20px #000000;
  }

  .container-special-support {
    width: 80%;
    text-align: justify;
    padding-bottom: 4rem;
  }

  .title-support {
    font-size: 30px;
    padding-top: 4rem;
    padding-bottom: 2rem;
    text-align: center;
  }

  .description-support {
    font-size: 16px;
    padding-bottom: 2rem;
    text-align: center;
  }

  .image-support {
    display: none;
  }

  .containers-address {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding-top: 2rem;
  }

  .adress-title {
    text-align: center;
    font-weight: bold;
    font-size: 20px;
    padding-top: 4rem;
  }
}

/* Tablets entre 601px a 1024px */
@media only screen and (min-width: 601px) and (max-width: 1024px) {
  .container-support {
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
    gap: 4rem;
    color: #000000;
    box-shadow: inset 0 0 20px -20px #000000;
  }

  .container-special-support {
    width: 80%;
    text-align: justify;
    padding-bottom: 10rem;
  }

  .title-support {
    font-size: 70px;
    padding-top: 10rem;
    padding-bottom: 2rem;
    text-align: center;
  }

  .description-support {
    font-size: 35px;
    padding-bottom: 2rem;
    text-align: center;
  }

  .image-support {
    display: none;
  }

  .containers-address {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding-top: 2rem;
    font-size: 35px;
  }

  .adress-title {
    text-align: center;
    font-weight: bold;
    font-size: 35px;
    padding-top: 10rem;
  }
}

/* Computadores desktop a partir de 1025px */
@media only screen and (min-width: 1025px) {
  .container-support {
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

  .container-special-support {
    width: 30%;
    margin-left: 6%;
    text-align: justify;
  }

  .title-support {
    font-size: 50px;
    padding-bottom: 2rem;
  }

  .description-support {
    font-size: 16px;
    padding-bottom: 2rem;
  }

  .image-support {
    width: 50%;
    margin-right: 6%;
    margin-left: 10%;
  }

  .containers-address {
    padding-top: 2rem;
  }

  .adress-title {
    font-weight: bold;
    font-size: 20px;
    padding-top: 6rem;
  }
}
</style>