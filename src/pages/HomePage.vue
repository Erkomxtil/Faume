<template>
    <div class="mainWrapper">
        <HeaderTop />
        <InfosText />
        <CollectionHommeFemme />
        <NotreSelection />
        <DressingHomme />
        <FooterBlack />
        <PopinCart />
    </div>
</template>

<script>
import HeaderTop from "@/components/HeaderTop.vue"
import InfosText from "@/components/InfosText.vue"
import CollectionHommeFemme from "@/components/CollectionHommeFemme.vue"
import FooterBlack from "@/components/FooterBlack.vue"
import DressingHomme from "../components/DressingHomme.vue"
import PopinCart from "@/components/PopinCart.vue"
import NotreSelection from "@/components/NotreSelection.vue"

export default {
    name: 'HomePage',
    components: { HeaderTop, InfosText, FooterBlack, CollectionHommeFemme, DressingHomme, PopinCart, NotreSelection },
    mounted() {

    }
}

</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap');
.mainWrapper {
    font-family: 'Open Sans', sans-serif;
    position: relative;
}
</style>