<template>
  <footer>
    <p>
      <span>Faq</span> <span>Mentions légales</span> <span>CGV</span>
    </p>
  </footer>
</template>

<script>
export default {
    name: 'FooterBlack',
    mounted() {
    }
}
</script>

<style lang="scss">
  footer {
    background-color: #000000;
    color: #ffffff;
    text-align: center;
    font-size: 13px;
    margin-bottom: -150px;
    p{
      padding: 210px 20px;
      display: flex;
      justify-content: center;
      gap: 120px;
    }
  }

</style>