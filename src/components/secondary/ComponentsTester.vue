<template>
    <div>
        <text-block :classVariant="1" />
        <span></span>
        <text-block classVariant="2" />
        <span></span>
    </div>
</template>

<script>
import TextBlock from "../secondary/TextBlock.vue";

export default {
    components: { TextBlock },
    name: "ComponentsTester",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

div {
    width: 99%;
    margin: 0 auto;

    span {
        height: 10vh;
        display: block;
    }
}
</style>
