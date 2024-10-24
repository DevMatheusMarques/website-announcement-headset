<script>
import SecondaryButton from "@/components/SecondaryButton.vue";
import PrimaryButton from "@/components/PrimaryButton.vue";

export default {
  name: "Header",
  components: {PrimaryButton, SecondaryButton}
}
</script>

<template>
  <section>
    <div class="header-container">
      <div class="header-text">
        <div class="header-container-enterprise">
          <span><img src="/assets/icons/icone-empresa.png" alt="Logo Empresa" class="header-logo"></span>
          <span class="header-name-enterprise">Cabos do Oeste</span>
        </div>
        <div>
            <div class="header-container-title">
              <h1>Fone de Ouvido <br> Oeste A56</h1>
            </div>

            <div class="header-container-buttons">
              <SecondaryButton text="compre agora" class="buy-now-button"/>
              <PrimaryButton text="COMPRE TUDO"/>
            </div>
        </div>
      </div>
      <span class="img-container">
        <img class="img-headset" src="/src/assets/fone-ouvido (2).png" alt="Imagem Fone de Ouvido Oeste A56" srcset="">
      </span>
    </div>
  </section>
</template>

<style scoped>

/* Celulares até 600px */
@media only screen and (max-width: 600px) {
  .header-container {
    max-width: 100%;
    height: 100%;
    background-image: url("../assets/background.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    gap: 4rem;
    color: #000000;
  }

  .header-text {
    width: 70%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .header-container-enterprise {
    padding-top: 4rem;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .header-logo {
    width: 30px;
    height: 30px;
    margin-right: 10px;
    margin-top: 10px;
  }

  .header-name-enterprise {
    font-size: 30px;
    font-weight: bold;
    justify-content: center;
  }

  .img-container {
    align-self: center;
    display: flex;
    align-items: center;
    justify-content: center;
    padding-bottom: 5rem;
  }

  .img-headset {
    width: 70%;
    height: 70%;
  }

  .header-container-title {
    width: 100%;
    font-weight: bold;
    font-size: 25px;
    line-height: 1.6em;
    text-align: center;
    padding-top: 4rem;
    padding-bottom: 4rem;
  }

  .header-container-buttons {
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }

  .buy-now-button {
    margin-right: 3%;
  }
}

/* Tablets entre 601px a 1024px */
@media only screen and (min-width: 601px) and (max-width: 1024px) {
  .header-container {
    max-width: 100%;
    height: 100%;
    background-image: url("../assets/background.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    gap: 6rem;
    color: #000000;
  }

  .header-text {
    width: 70%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .header-container-enterprise {
    padding-top: 4rem;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .header-logo {
    width: 50px;
    height: 50px;
    margin-right: 10px;
    margin-top: 10px;
  }

  .header-name-enterprise {
    font-size: 50px;
    font-weight: bold;
    justify-content: center;
  }

  .img-container {
    align-self: center;
    display: flex;
    align-items: center;
    justify-content: center;
    padding-bottom: 10rem;
  }

  .img-headset {
    width: 70%;
    height: 70%;
  }

  .header-container-title {
    width: 100%;
    font-weight: bold;
    font-size: 50px;
    line-height: 1.6em;
    text-align: center;
    padding-top: 4rem;
    padding-bottom: 4rem;
  }

  .header-container-buttons {
    display: flex;
    flex-direction: row;
    gap: 2rem;
    align-items: center;
  }
}


/* Computadores desktop a partir de 1025px */
@media only screen and (min-width: 1025px) {
  .header-container {
    max-width: 100%;
    height: 100dvh;
    background-image: url("../assets/background.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    color: #000000;
  }

  .header-text {
    width: 70%;
  }

  .header-container-enterprise {
    padding-top: 6%;
    padding-left: 10%;
    display: flex;
  }

  .header-logo {
    width: 30px;
    height: 30px;
    margin-right: 10px;
    margin-top: 10px;
  }

  .header-name-enterprise {
    font-size: 30px;
    font-weight: bold;
    justify-content: center;
  }

  .img-container {
    align-self: center;
  }

  .img-headset {
    width: 70%;
    height: 70%;
  }

  .header-container-title {
    font-weight: bold;
    font-size: 48px;
    margin-top: 15%;
    margin-left: 16%;
    line-height: 1.6em;
  }

  .header-container-buttons {
    margin-top: 10%;
    margin-left: 16%;
  }

  .buy-now-button {
    margin-right: 3%;
  }
}

</style>