<template>
    <button>{{ buttonText }}</button>
</template>

<script>
export default {
    name: "BtnMono",
    props: { buttonText: String },
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";
button {
    @include btn-primary;
    text-align: center;
}
</style>
