<template>
    <div :class="classVariant">
        <h4>i am a subtitle</h4>
        <h2>Award Winning Moving Company</h2>
    </div>
</template>

<script>
export default {
    name: "TextBlock",
    props: { classVariant: String },
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

div {
    border: 2px solid black;
    margin: 2rem;

    width: 70%;
    margin: 0 auto;
}

/////////////////////////////////////////////////////////////////// MIXINS
.variant-1 {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    h4 {
        @include title-small;
    }

    h2 {
        @include title-medium;
        width: 50%;
    }
}
/////////////////////////////////////////////////////////////////// MIXINS

/////////////////////////////////////////////////////////////////// MIXINS
.variant-2 {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    h4 {
        @include title-small;
    }

    h2 {
        @include title-big;
    }
}
/////////////////////////////////////////////////////////////////// MIXINS
</style>
