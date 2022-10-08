<template>
    <div class="container">
        <div class="wrapper">
            <text-block :classVariant="1" subtitle="happy customers" title="Testimonials" />
            <div class="card-container">
                <testimonial-block
                    imgUrl="https://avada.theme-fusion.com/movers/wp-content/uploads/sites/108/2018/06/avada-movers-johndoe-final.jpg"
                    title="John Doe"
                    description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.'"
                />
                <testimonial-block
                    imgUrl="https://avada.theme-fusion.com/movers/wp-content/uploads/sites/108/2018/06/avada-movers-johndoe-final.jpg"
                    title="Jane Doe"
                    description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.'"
                />
                <testimonial-block
                    imgUrl="https://avada.theme-fusion.com/movers/wp-content/uploads/sites/108/2018/06/avada-movers-johndoe-final.jpg"
                    title="John Smith"
                    description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.'"
                />
            </div>

            <btn-mono buttonText="read more testimonials" />
        </div>
    </div>
</template>

<script>
import BtnMono from "../secondary/BtnMono.vue";
import TestimonialBlock from "../secondary/TestimonialBlock.vue";
import TextBlock from "../secondary/TextBlock.vue";
export default {
    components: { TextBlock, TestimonialBlock, BtnMono },
    name: "TestimonialsSection",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    .wrapper {
        @include wrapper-size;
        padding: 6rem 0rem;

        p {
            padding: 2rem;
        }

        .card-container {
            display: flex;
            gap: 3rem;
            margin: 3rem 0;

            @media screen and (max-width: 1024px) {
                flex-direction: column;
            }
        }
    }
}
</style>
