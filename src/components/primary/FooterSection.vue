<template>
    <div class="container">
        <div class="wrapper">
            <div class="block">
                <h3>about</h3>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis convallis ex ut sem accumsan vehicula. Integer elit arcu, hendrerit
                    id sapien ut, facilisis accumsan arcu.
                </p>
                <img src="../../../public/images/avada-movers-logo.png" alt="logo" />
            </div>

            <div class="block">
                <list-block />
            </div>

            <div class="block">
                <list-block />
            </div>
        </div>

        <social-block :classVariant="2" />
    </div>
</template>

<script>
import ListBlock from "../secondary/ListBlock.vue";
import SocialBlock from "../secondary/SocialBlock.vue";
export default {
    components: { ListBlock, SocialBlock },
    name: "FooterSection",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    .wrapper {
        @include wrapper-size;
        display: flex;
        padding: 3rem 0;
        flex-wrap: wrap;

        h3 {
            @include title-list;
            margin-bottom: 1rem;
        }

        .block {
            width: calc(100% / 3);
            padding: 1.5rem 2rem 1.5rem 0rem;

            @media screen and (max-width: 640px) {
                width: 100%;
            }

            img {
                margin: 2rem 0rem;
            }
        }
    }
}
</style>
