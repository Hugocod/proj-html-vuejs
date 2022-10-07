<template>
    <div class="container">
        <div class="wrapper">
            <text-block :classVariant="1" subtitle="we are professional" title="Full-Service Solution" />
            <div class="card-container">
                <card-block />
                <card-block />
                <card-block />
            </div>
        </div>
    </div>
</template>

<script>
import CardBlock from "../secondary/CardBlock.vue";
import TextBlock from "../secondary/TextBlock.vue";
export default {
    components: { TextBlock, CardBlock },
    name: "ServiceSection",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    .wrapper {
        @include wrapper-size;
        padding: 6rem 0rem;

        p {
            padding: 2rem;
        }

        .card-container {
            display: flex;
            gap: 3rem;
            margin: 3rem 0;
        }
    }
}
</style>
