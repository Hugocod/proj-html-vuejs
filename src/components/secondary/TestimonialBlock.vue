<template>
    <div class="container">
        <img :src="imgUrl" alt="" />

        <div class="text-container">
            <h2>{{ title }}</h2>
            <p>
                {{ description }}
            </p>
        </div>
    </div>
</template>

<script>
export default {
    name: "TestimonialBlock",
    props: ["title", "description", "imgUrl"],
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    padding: 1.5rem;
    h2 {
        @include title-regular;
    }

    p {
        margin: 1.3rem 0;
        font-style: italic;
    }

    img {
        width: 50%;
        margin-bottom: 1.3rem;
        border-radius: 50%;

        @media screen and (max-width: 1024px) {
            width: 200px;
        }
    }

    .text-container {
        padding: 1.5rem;
    }
}
</style>
