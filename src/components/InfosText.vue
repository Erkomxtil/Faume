<template>
    <section class="infos">
        <h2>Lorem ipsum dolor sit amet</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur id officiis magnam vel expedita quam odit eaque possimus et suscipit placeat quia, numquam commodi aspernatur facilis eos porro accusantium laboriosam. Esse id corrupti sunt rerum beatae ipsum corporis possimus error culpa animi. Beatae vitae sed optio nemo quasi incidunt, totam explicabo mollitia ab possimus vel officiis cum excepturi harum illo.</p><br>
        <span class="btn discover">Découvrir</span>
    </section>
</template>

<script>
export default {
    name: 'InfosText',
    mounted() {
    }
}
</script>

<style lang="scss">
    .infos {
        text-align: center;
        padding: 196px 20px 162px 20px;

        h2 {
            font-size: 44px; 
            text-transform: uppercase;
            font-weight: 700;  
            padding-bottom: 64px;
        }
        p {
            font-size: 13px;
            max-width: 1530px;
            display: inline-block;
            padding-bottom: 108px;
        }
        .btn {
            font-size: 26px;
            border: 2px solid #000000;
            padding: 40px 106px;
            text-transform: uppercase;
        }
        .discover:hover {
            background-color: #000000;
            color: #ffffff;
            cursor: pointer;
        }
    }
</style>