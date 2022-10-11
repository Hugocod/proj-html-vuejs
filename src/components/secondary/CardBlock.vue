<template>
    <div class="container">
        <img :src="imgUrl" alt="" />

        <div class="text-container">
            <h2>{{ title }}</h2>
            <p>
                {{ description }}
            </p>
            <btn-mono buttonText="read more" />
        </div>
    </div>
</template>

<script>
import BtnMono from "./BtnMono.vue";
export default {
    name: "CardBlock",
    /*    data() {
        return {
            img_1: [require("../../../public/images/avada-movers-serviceonephoto-final.jpg")],
            img_2: [require("../../../public/images/avada-movers-serviceonephoto-final.jpg")],
            img_3: [require("../../../public/images/avada-movers-serviceonephoto-final.jpg")],
            images: [this.img_1, this.img_2, this.img_3],
        };
    }, */
    components: { BtnMono },
    props: ["title", "description", "imgUrl"],
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    background-color: $color-gray-light;

    padding: 1.1rem;
    h2 {
        @include title-regular;
    }

    p {
        margin: 1.1rem 0;
    }

    img {
        width: 100%;
        margin-bottom: 1.3rem;
    }

    .text-container {
        background-color: $color-white;
        padding: 1.5rem;
    }
}
</style>
