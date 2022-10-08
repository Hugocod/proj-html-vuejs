<template>
    <div class="container">
        <div class="wrapper">
            <text-block :classVariant="1" subtitle="we are professional" title="Full-Service Solution" />
            <div class="card-container">
                <card-block
                    imgUrl="https://avada.theme-fusion.com/movers/wp-content/uploads/sites/108/2018/06/avada-movers-serviceonephoto-final.jpg"
                    title="Two Man Teams"
                    description="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus."
                />
                <card-block
                    imgUrl="https://avada.theme-fusion.com/movers/wp-content/uploads/sites/108/2018/06/avada-movers-serviceonephoto-final.jpg"
                    title="We Do All The Lifting"
                    description="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus."
                />
                <card-block
                    imgUrl="https://avada.theme-fusion.com/movers/wp-content/uploads/sites/108/2018/06/avada-movers-serviceonephoto-final.jpg"
                    title="Coast To Coast"
                    description="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus."
                />
            </div>
        </div>
    </div>
</template>

<script>
import CardBlock from "../secondary/CardBlock.vue";
import TextBlock from "../secondary/TextBlock.vue";
export default {
    components: { TextBlock, CardBlock },
    name: "ServiceSection",
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
