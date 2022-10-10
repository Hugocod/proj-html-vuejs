<template>
    <div class="container">
        <div class="wrapper">
            <text-block :classVariant="1" title="Request A Free Quote" />
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis
                parturient montes, nascetur ridiculus mus.
            </p>
            <btn-mono buttonText="click here" />
        </div>
    </div>
</template>

<script>
import BtnMono from "../secondary/BtnMono.vue";
import TextBlock from "../secondary/TextBlock.vue";
export default {
    components: { TextBlock, BtnMono },
    name: "CtaSection",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    background-image: url("../../../public/images/avada-movers-request-quote-background.jpg");
    border-bottom: 15px solid $color-green-vivid;
    background-size: cover;
    text-align: center;
    .wrapper {
        @include wrapper-size;
        padding: 6rem 0rem;
        width: 60%;

        @media screen and (max-width: 1024px) {
            width: 90%;
        }

        p {
            padding: 2rem 0;
        }
    }
}
</style>
