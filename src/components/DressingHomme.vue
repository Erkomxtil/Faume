<template>
  <section class="dressingHomme">
    <div><img src="../assets/images/dressing.jpg" alt="Dressing"></div>
    <div class="greyBtn"><span class="btn discover">Découvrir</span></div>
  </section>
</template>

<script>
export default {
    name: 'DressingHomme',
    mounted() {
    }
}
</script>

<style lang="scss">
  .dressingHomme {
    display: flex;
    margin-bottom: -8px;
    div {
      width: 50%;
      img {
        width: 100%;
      }
    }
    .greyBtn {
      background-color: #eeeeee;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .btn {
      font-size: 26px;
      border: 2px solid #000000;
      padding: 40px 106px;
      text-transform: uppercase;

      @media (max-width: 650px) {
        padding: 20px 53px;
      }
    }
    .discover:hover {
      background-color: #000000;
      color: #ffffff;
      cursor: pointer;
    }

    @media (max-width: 1260px) {
      flex-direction: column;

      div {
        width: 100%;
      }

      .greyBtn {
        height: 300px;
        margin-top: -20px;
      }
    }
  }
</style>