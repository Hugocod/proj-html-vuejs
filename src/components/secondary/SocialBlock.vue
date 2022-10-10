<template>
    <div :class="availableVariants[setClass()]">
        <div class="wrapper">
            <p>{{ description }}</p>

            <div class="social-container">
                <font-awesome-icon icon="fa-brands fa-facebook" />
                <font-awesome-icon icon="fa-brands fa-twitter" />
                <font-awesome-icon icon="fa-brands fa-instagram" />
                <font-awesome-icon icon="fa-brands fa-youtube" />
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "SocialBlock",
    data() {
        return {
            availableVariants: ["variant-1", "variant-2"], // a ognuna delle classi corrisponde una variante del componente
        };
    },

    props: { classVariant: Number, description: String },
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
    background-color: $color-green-vivid;
    color: white;

    .wrapper {
        @include wrapper-size;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0.8rem 0;

        .social-container {
            display: flex;
            flex-wrap: nowrap;
            .fa-facebook,
            .fa-twitter,
            .fa-instagram,
            .fa-youtube {
                margin: 0 0.5rem;
                font-size: 1.2rem;
                cursor: pointer;
            }
        }

        p {
            font-size: 0.9rem;
            font-weight: 500;
        }
    }
}
/////////////////////////////////////////////////////////////////// VARIANT-----/

/////////////////////////////////////////////////////////////////// VARIANT-2
.variant-2 {
    background-color: $color-green-vivid;
    color: white;

    .wrapper {
        @include wrapper-size;
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-direction: column;
        padding: 2rem 0;

        .social-container {
            display: flex;
            flex-wrap: nowrap;
            padding-top: 2rem;
            .fa-facebook,
            .fa-twitter,
            .fa-instagram,
            .fa-youtube {
                margin: 0 0.5rem;
                font-size: 1.4rem;
                cursor: pointer;
            }
        }

        p {
            font-size: 0.9rem;
            font-weight: 500;
            text-align: center;
        }
    }
}
/////////////////////////////////////////////////////////////////// VARIANT-----/
</style>
