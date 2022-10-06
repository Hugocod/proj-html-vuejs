<template>
    <div class="container">
        <img src="https://avada.theme-fusion.com/movers/wp-content/uploads/sites/108/2018/06/avada-movers-johndoe-final.jpg" alt="" />

        <div class="text-container">
            <h2>John Doe</h2>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis
                parturient montes, nascetur ridiculus mus.
            </p>
        </div>
    </div>
</template>

<script>
export default {
    name: "TestimonialBlock",
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
        font-style: italic;
    }

    img {
        width: 50%;
        margin-bottom: 1.3rem;
        border-radius: 50%;
    }

    .text-container {
        padding: 1.5rem;
    }
}
/////////////////////////////////////////////////////////////////// MIXINS
</style>
