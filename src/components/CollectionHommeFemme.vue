<template>
  <section class="hommeFemme">
    <div class="femme">
      <img src="../assets/images/collectionFemme.jpg" alt="Femme">
      <h2>Collection femme</h2>
    </div>
    <div class="homme">
      <img src="../assets/images/collectionHomme.jpg" alt="homme">
      <h2>Collection Homme</h2>
    </div>
  </section>
</template>

<script>
export default {
    name: 'CollectionHommeFemme',
    mounted() {
    }
}
</script>

<style lang="scss">
  .hommeFemme {
    display: flex;
    gap: 5px;
    .homme, .femme {
      width: 50%;
      position: relative;
      img {
        width: 100%;
      }
      h2 {
        position: absolute;
        bottom: 65px;
        left: 60px;
        color: #ffffff;
        text-transform: uppercase;
        font-weight: 700;
        font-size: 30px;
      }

      @media (max-width: 1260px) {
        width: 100%;
      }
    }

    @media (max-width: 1260px) {
      flex-direction: column;
      gap: unset;
    }
  }
</style>