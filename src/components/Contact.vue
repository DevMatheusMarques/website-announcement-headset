<script>
export default {
  name: "Contact"
}
</script>

<template>
  <section>
    <div class="container-contact">
      <div>
        <p class="title-contact">Entre em Contato</p>
      </div>
      <div style="display: flex; gap: 5rem" class="container-texts">
        <div>
          <p class="adress-title">ESCRITÓRIO</p>
          <div class="containers">
            <p class="simple-text">Rua Qualquer, 123</p>
            <p class="simple-text">Qualquer Cidade,</p>
            <p class="simple-text">Estado, País</p>
            <p class="simple-text">(12) 34567-7890</p>
            <p class="adress-title">alo@sitebacana.com.br</p>
          </div>
        </div>
        <div>
          <div>
            <p class="adress-title">MÍDIAS SOCIAIS</p>
            <div class="containers">
              <p class="simple-text">Instagram</p>
              <p class="simple-text">Facebook</p>
              <p class="simple-text">Twitter</p>
            </div>
          </div>
      </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Celulares até 600px */
@media only screen and (max-width: 600px) {
  .container-contact {
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
    box-shadow: inset 0 0 20px -20px #000000;
    padding-bottom: 4rem;
  }

  .title-contact {
    text-align: center;
    font-size: 30px;
    padding-top: 4rem;
  }

  .adress-title {
    text-align: center;
    font-weight: bold;
    font-size: 20px;
    padding-top: 1rem;
  }

  .containers {
    padding-top: 2rem;
  }

  .simple-text {
    font-size: 20px;
    text-align: center;
  }

  .container-texts {
    display: flex;
    flex-direction: column;
  }
}

/* Tablets entre 601px a 1024px */
@media only screen and (min-width: 601px) and (max-width: 1024px) {
  .container-contact {
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
    flex-direction: column;
    gap: 10rem;
    color: #000000;
    box-shadow: inset 0 0 20px -20px #000000;
    padding-bottom: 10rem;
  }

  .title-contact {
    text-align: center;
    font-size: 70px;
    padding-top: 10rem;
  }

  .adress-title {
    text-align: center;
    font-weight: bold;
    font-size: 35px;
    padding-top: 1rem;
  }

  .containers {
    padding-top: 2rem;
  }

  .simple-text {
    font-size: 35px;
    text-align: center;
  }

  .container-texts {
    display: flex;
    flex-direction: column;
  }
}

/* Computadores desktop a partir de 1025px */
@media only screen and (min-width: 1025px) {
  .container-contact {
    max-width: 100%;
    height: 100dvh;
    background-image: url("../assets/background.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    gap: 20rem;
    align-items: center;
    color: #000000;
    box-shadow: inset 0 0 20px -20px #000000;
  }

  .title-contact {
    font-size: 50px;
    padding-bottom: 10rem;
    padding-left: 6rem;
  }

  .adress-title {
    font-weight: bold;
    font-size: 20px;
    padding-top: 6rem;
  }

  .containers {
    padding-top: 2rem;
  }

  .simple-text {
    font-size: 20px;
  }
}
</style>