<template>
    <div :class="availableVariants[setClass()]">
        <h4>{{ subtitle }}</h4>
        <h2>{{ title }}</h2>
    </div>
</template>

<script>
export default {
    name: "TextBlock",
    data() {
        return {
            availableVariants: ["variant-1", "variant-2"], // a ognuna delle classi corrisponde una variante del componente
        };
    },
    props: { classVariant: Number, title: String, subtitle: String },
    methods: {
        setClass() {
            return this.classVariant - 1; // fa partire il conto da 1
        },
    },
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

/////////////////////////////////////////////////////////////////// VARIANT-1
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
/////////////////////////////////////////////////////////////////// VARIANT-----/

/////////////////////////////////////////////////////////////////// VARIANT-2
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
/////////////////////////////////////////////////////////////////// VARIANT-----/
</style>
