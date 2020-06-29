<template>
    <div class="container-master">
        <HomeSlider />
        <ProductCardSlider />
    </div>
</template>

<script>
import HomeSlider from "~/components/HomeSlider";
import ProductCardSlider from "~/components/ProductCardSlider";


export default {
    components: {
        HomeSlider,
        ProductCardSlider
    }  
}
</script>

<style lang="scss">
.container-master {
    max-width: 1300px;
    margin-left: auto;
    margin-right: auto;
}
</style>
