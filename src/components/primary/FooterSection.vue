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
                <list-block :title="avadaResources.title" :links="avadaResources.links" />
            </div>

            <div class="block">
                <list-block :title="recentPosts.title" :links="recentPosts.posts" />
            </div>
        </div>

        <social-block
            :classVariant="2"
            description="This is a clone of Avada Theme by ThemeFusion | For educational purposes | developed by hugo with ❤️"
        />
    </div>
</template>

<script>
import ListBlock from "../secondary/ListBlock.vue";
import SocialBlock from "../secondary/SocialBlock.vue";
export default {
    components: { ListBlock, SocialBlock },
    name: "FooterSection",
    data() {
        return {
            avadaResources: {
                title: "avada movers",
                links: ["Home", "Rates", "Testimonials", "Blog", "Free Quote"],
            },
            recentPosts: {
                title: "recent posts",
                posts: ["Heading Out To College?", "Moving Your Business?", "Outstanding Quality", "Cost of Moving", "Best Moving Tips"],
            },
        };
    },
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
            margin-bottom: 2.2rem;
        }

        .block {
            width: calc(100% / 3);
            padding: 1.7rem 3rem 1.7rem 0rem;

            @media screen and (max-width: 640px) {
                width: 100%;
            }

            img {
                margin-top: 2rem;
            }
        }
    }
}
</style>
