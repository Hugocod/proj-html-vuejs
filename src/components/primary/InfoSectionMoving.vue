<template>
    <div class="container">
        <div class="wrapper">
            <div class="empty-box"></div>
            <div class="green-box">
                <text-block class="t-block" :classVariant="3" subtitle="we remove the headache from moving" title="Move With Ease" />
                <div class="line"></div>
                <p>
                    With our super simple service we can take you from getting a quote, right through to being in your new home with all of your
                    belongings securely packed and safely delivered, even in the rooms of your choice.
                </p>
                <btn-mono buttonText="click here" />
            </div>
        </div>
    </div>
</template>

<script>
import BtnMono from "../secondary/BtnMono.vue";
import TextBlock from "../secondary/TextBlock.vue";
export default {
    components: { TextBlock, BtnMono },
    name: "InfoSectionMoving",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    background-image: url("https://avada.theme-fusion.com/movers/wp-content/uploads/sites/108/2018/06/avada-movers-movewithease-background-new.jpg");
    background-size: cover;
    padding: 7rem 0;
    text-align: center;

    .wrapper {
        @include wrapper-size;
        padding: 2rem 0rem;

        display: flex;
        justify-content: space-between;

        .empty-box {
            width: 0%;
        }

        .green-box {
            width: 55%;
            background-color: $color-green-vivid;
            color: $color-white;
            border: 1rem solid $color-green-darker;
            padding: 2.5rem 0;

            @media screen and (max-width: 1024px) {
                width: 100%;
            }

            .line {
                height: 0.01rem;
                margin: 0 auto;
                margin-top: 2rem;

                width: 70%;
                background-color: rgb(81, 255, 81);
            }

            p {
                padding: 2rem;
            }
        }
    }
}
</style>
