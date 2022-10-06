<template>
    <div class="container">
        <img src="https://avada.theme-fusion.com/movers/wp-content/uploads/sites/108/2018/06/avada-movers-serviceonephoto-final.jpg" alt="" />

        <div class="text-container">
            <h2>Award Winning Moving Company</h2>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis
                parturient montes, nascetur ridiculus mus.
            </p>
            <btn-mono />
        </div>
    </div>
</template>

<script>
import BtnMono from "./BtnMono.vue";
export default {
    components: { BtnMono },
    name: "CardBlock",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

/////////////////////////////////////////////////////////////////// MIXINS
.container {
    background-color: $color-gray-light;

    padding: 1.5rem;
    h2 {
        @include title-regular;
    }

    p {
        margin: 1.3rem 0;
    }

    img {
        width: 100%;
        margin-bottom: 1.3rem;
    }

    .text-container {
        background-color: $color-white;
        padding: 1.5rem;
    }
}
/////////////////////////////////////////////////////////////////// MIXINS
</style>
