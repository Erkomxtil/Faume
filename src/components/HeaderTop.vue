@include 
<template>
    <section class="header">
      <div class="menu">
        <div><span><a href="#">Homme</a></span> <span><a href="#">Femme</a></span> <a href="#">Concept</a> </div>
        <div><img class="logo" src="../assets/images/logo.svg" alt="logo"></div>
        <div class="cartWrapper">
          <a href="#" data-modal><img data-img-link class="cart" src="../assets/images/icon-cart.png" alt="Cart"></a>
        </div>
      </div>
      <div class="mainTitle">
        <h1>Femme</h1>
        <span class="discover">Découvrir</span>
      </div>
    </section>
</template>

<script>
export default {
    name: 'HeaderTop',
    mounted() {
      window.addEventListener('scroll', () => {
        let positionScroll = window.scrollY
        let menu = document.querySelector('.menu')
        let header = document.querySelector('.header')
        let logo = document.querySelector('.logo')
        let cart = document.querySelector('.cart')

        if (positionScroll > 10) {
          menu.classList.add('active')
          header.classList.add('active')
          logo.classList.add('black')
          cart.classList.add('black')
        } else {
          menu.classList.remove('active')
          header.classList.remove('active')
          logo.classList.remove('black')
          cart.classList.remove('black')
        }
      })
    }

}
</script>

<style lang="scss">
.header {
  padding: 22px 40px 0px 40px;
  height: 100vh;
  background-image: url('../assets/images/femme.jpeg');
  width: auto;  background-position: 0 0;
  background-size: cover;
  position: relative;

  .menu {
    display: flex;
    justify-content: space-between;
    text-transform: uppercase;
    color: #ffffff;
    font-size: 20px;
    font-weight: bold;
    position: relative;
    span {
      padding-right: 60px;
    }

    &.active {
      position: fixed;
      background-color: #ffffff;
      color: #000000;
      z-index: 100;
      width: 100%;
      padding: 20px 40px;

    }
  }

  .logo {
    width: auto;
    height: 70px;
    margin-left: -120px;

    &.black {
      filter: invert(100%) sepia(63%) saturate(6234%) hue-rotate(246deg) brightness(87%) contrast(156%);
    }
  }
  .cartWrapper {
    min-width: 234px;
    text-align: right;
    .cart {
      width: auto;
      height: 40px;

      &.black {
        filter: invert(100%) sepia(63%) saturate(6234%) hue-rotate(246deg) brightness(87%) contrast(156%);
      }
    }
  
    .popin {
      display: none;
      top:50px;
      right: 0;

      &.active {
        display: block;
      }
    }
  }

  .mainTitle {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: #ffffff;
    text-align: center;
    h1 {
      font-size: 150px;
      text-transform: uppercase;
      padding-bottom: 120px;
    }
    span {
      font-size: 26px;
      border: 2px solid #ffffff;
      padding: 40px 106px;
      text-transform: uppercase;
    }

    .discover:hover {
      background-color: #000000;
      color: #ffffff;
      cursor: pointer;
    }
  }
  &.active {
    padding: 0;
  }
}
</style>