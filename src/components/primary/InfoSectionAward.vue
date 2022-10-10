<template>
    <div class="container">
        <div class="wrapper">
            <text-block :classVariant="1" subtitle="HEADACHE FREE" title="Award Winning" />
            <text-block :classVariant="4" title="Moving Company" />
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac augue. Orci varius natoque penatibus et magnis dis parturient
                montes, ridiculus mus. Aliquam enim leo, condimentum facilisis nulla sed, cursus arcu. Aliquam enim leo.
            </p>
            <btn-mono buttonText="read out our testimonials" />
        </div>
    </div>
</template>

<script>
import BtnMono from "../secondary/BtnMono.vue";
import TextBlock from "../secondary/TextBlock.vue";
export default {
    components: { TextBlock, BtnMono },
    name: "InfoSectionAward",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    text-align: center;
    background-color: $color-gray-light;
    .wrapper {
        @include wrapper-size;
        padding: 6rem 0rem;
        width: 80%;

        p {
            padding: 2rem;
        }
    }
}
</style>
