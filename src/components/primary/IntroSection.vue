<template>
    <div class="container">
        <social-block classVariant="1" description="Call us for a Free Quote: 1.800.555.6789" />
        <header>
            <div class="wrapper">
                <img src="../../../public/images/avada-movers-retinalogo.png" alt="logo" />

                <div class="nav-container">
                    <nav>
                        <ul>
                            <li v-for="(link, index) in navLinks" :key="index">
                                <a>{{ link }}</a>
                            </li>
                        </ul>
                    </nav>
                    <btn-mono buttonText="Free Quote" />
                </div>

                <font-awesome-icon icon="fa-solid fa-bars" />
            </div>
        </header>

        <div class="text-block">
            <text-block classVariant="2" title="we make it simple" subtitle="moving without the hassle" />
            <p>PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMER SATISFACTION</p>
        </div>

        <button class="large-button">
            <font-awesome-icon icon="fa-regular fa-paper-plane" />
            get a free quote online now
        </button>
    </div>
</template>

<script>
import BtnMono from "../secondary/BtnMono.vue";
import SocialBlock from "../secondary/SocialBlock.vue";
import TextBlock from "../secondary/TextBlock.vue";
export default {
    components: { BtnMono, TextBlock, SocialBlock },
    name: "IntroSection",
    data() {
        return {
            navLinks: ["Home", "Rates", "Testimonials", "FAQ", "Blog", "Contact"],
        };
    },
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    background-image: url(../../../public/images/avada-movers-homeherobackground-final.jpg);
    background-size: cover;
    background-position: fixed;
}

header {
    width: 100%;
    padding: 2rem 0;

    img {
        width: 12rem;
    }

    .wrapper {
        display: flex;
        justify-content: space-between;
        align-items: center;
        @include wrapper-size;
    }

    .nav-container {
        display: flex;
        justify-content: center;
        align-items: center;

        @media screen and (max-width: 1024px) {
            display: none;
        }

        ul {
            display: flex;

            li {
                font-weight: 900;
                text-transform: none;
                padding: 0 1.3rem;

                & :hover {
                    color: $color-green-vivid;
                }
            }
        }
    }

    .fa-bars {
        @media screen and (min-width: 1024px) {
            display: none;
        }
        font-size: 1.5rem;
    }
}

.text-block {
    p {
        @include title-small;
        text-align: center;
    }

    padding: 6rem 0rem 11rem 0rem;
}

.large-button {
    width: 100%;
    padding: 4rem 0;
    text-transform: uppercase;
    font-size: 1.3rem;
    background-color: $color-blue;
    color: $color-white;
    text-align: center;

    &:hover {
        background-color: $color-blue-light;
        cursor: pointer;
    }
}
</style>
