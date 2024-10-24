<script>
import PrimaryButton from "@/components/PrimaryButton.vue";
import CategoriesCard from "@/components/CategoriesCard.vue";

export default {
  name: "Categories",
  components: {CategoriesCard, PrimaryButton},
}
</script>

<template>
  <section class="container-categories">
    <div>
      <div class="title-category">
        <span>Compre por categoria</span>
      </div>
      <div class="container-cards">
        <CategoriesCard image-url="/assets/telefone.png" font-size="23px" image-description="teste" card-title="TELEFONES & ACESSÓRIOS" text="Telefones de alta qualidade a preços acessíveis" class="card-category"/>
        <CategoriesCard image-url="/assets/computador.png" font-size="23px" image-description="teste" card-title="EQUIPAMENTO DE COMPUTADOR" text="Do desktop ao notebook, não importa a necessidade" class="card-category"/>
        <CategoriesCard image-url="/assets/fone.png" font-size="24px" image-description="teste" card-title="OUTROS PRODUTOS" text="Diversos Produtos  para atender às suas necessidades" class="card-category"/>
      </div>
      <div style="text-align: center; padding-top: 4rem" class="sale-all-button">
        <PrimaryButton text="COMPRE TUDO" style="font-weight: bold"/>
      </div>
    </div>
  </section>
</template>
<style scoped>
/* Celulares até 600px */
@media only screen and (max-width: 600px) {
  .container-categories {
    max-width: 100%;
    height: 100%;
    background-image: url("../assets/background.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    color: #000000;
  }

  .title-category {
    font-size: 30px;
    text-align: center;
    padding-top: 4rem;
    padding-bottom: 3.5rem;
  }

  .container-cards {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 3rem;
  }

  .card-category {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: .5rem;
  }

  .sale-all-button {
    padding-bottom: 4rem;
  }
}

/* Tablets entre 601px a 1024px */
@media only screen and (min-width: 601px) and (max-width: 1024px) {
  .container-categories {
    max-width: 100%;
    height: 100%;
    background-image: url("../assets/background.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    color: #000000;
  }

  .title-category {
    font-size: 70px;
    text-align: center;
    padding-top: 10rem;
    padding-bottom: 3.5rem;
  }

  .container-cards {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    gap: 3rem;
  }

  .card-category {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: .5rem;
  }

  .sale-all-button {
    padding-bottom: 10rem;
  }
}

/* Computadores desktop a partir de 1025px */
@media only screen and (min-width: 1025px) {
  .container-categories {
    max-width: 100%;
    height: 100dvh;
    background-image: url("../assets/background.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    color: #000000;
  }

  .title-category {
    font-size: 46px;
    text-align: center;
    padding-top: 2%;
    padding-bottom: 3.5rem;
  }

  .container-cards {
    display: flex;
    justify-content: space-evenly;
    gap: 3rem;
  }

  .card-category {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    gap: .5rem;
  }
}
</style>