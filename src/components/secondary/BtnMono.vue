<template>
    <button>ciao</button>
</template>

<script>
export default {
    name: "BtnMono",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";
button {
    @include btn-primary;
}
</style>
