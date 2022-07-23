<template>
  <section class="popinWrapper">
    <div class="popin">Votre panier est vide</div>
  </section>
</template>

<script>

export default {
  name: 'PopinCart',
  mounted() {
    let cartBtn = document.querySelector('.cart')
    let popinWrapper = document.querySelector('.popinWrapper')
    cartBtn.addEventListener('click', (e) => {
      e.preventDefault()
      popinWrapper.classList.toggle('open')
    })
  }
}
</script>

<style lang="scss">

  .popinWrapper {
    display: none;

    &.open {
      display: block;
      position: sticky;
      bottom: 0vh;
      left: 0vw;
      background-color: #C4CBD0;
      color: #ffffff;
      max-width: 200px;
      text-align: center;
      height: 150px;
      -webkit-border-top-left-radius: 10px;
      -webkit-border-top-right-radius: 10px;
      -moz-border-radius-topleft: 10px;
      -moz-border-radius-topright: 10px;
      border-top-left-radius: 10px;
      border-top-right-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
    }
  }
</style>