<template>
  <section class="notreSelection">
    <h2>Notre sélection</h2>
    <div class="productWrapper">
      <div class="product">
        <div class="imgWrapper">
          <img class="product1" src="../assets/images/product1.jpeg" alt="T-shirt">
          <img class="product1a" src="../assets/images/product5.jpeg" alt="T-shirt zoom">
        </div>
        <div class="textInfo">
          <span>T-shirt Homme</span><br>
          70€
        </div>
      </div>
      <div class="product">
        <img src="../assets/images/product2.jpeg" alt="Veste cuir"><br>
        <span>Veste cuir</span><br>
        170€
      </div>
      <div class="product">
        <img src="../assets/images/product3.jpeg" alt="Trench Homme"><br>
        <span>Trench Homme</span><br>
        250€
      </div>
      <div class="product">
        <img src="../assets/images/product4.jpeg" alt="Sac cuir"><br>
        <span>Sac cuir</span><br>
        360€
      </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'NotreSelection',
    mounted() {
      let imageWrapper = document.querySelector('.imgWrapper')
      let product1 = document.querySelector('.product1')
      let product1a = document.querySelector('.product1a')
      imageWrapper.addEventListener('mouseover', () => {
        product1.classList.add('over')
        product1a.classList.add('visible')
      })

      imageWrapper.addEventListener('mouseleave', () => {
        product1.classList.remove('over')
        product1a.classList.remove('visible')
      })
    }
}
</script>

<style lang="scss">
  .notreSelection {
    padding: 210px 60px;
    h2 {
      font-size: 30px;
      font-weight: 700;
      text-transform: uppercase;
    }

    .productWrapper {
      display: flex;
      gap: 22px;

      .product {
        font-size: 20px;
        .imgWrapper {
          height: 858.08px;
        }

        img {
          max-width: 587px;
        }
        span {
          font-size: 22px;
          font-weight: bold;
        }

        .product1.over {
          display: none;
        }

        .product1a {
          display: none;
          &.visible {
            display: block;
          }
        }
      }

      @media (max-width: 2480px){
        overflow: hidden;
        overflow-x: scroll;
      }
    }

    @media (max-width: 2480px ) {
      padding: 180px 20px;
    }
  }

</style>