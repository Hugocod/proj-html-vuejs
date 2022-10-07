<template>
    <header>
        <div class="wrapper">
            <img src="../../../public/images/avada-movers-logo.png" alt="logo" />

            <div class="nav-container">
                <nav>
                    <ul>
                        <li v-for="n in 6" :key="n">
                            <a>link{{ n }}</a>
                        </li>
                    </ul>
                </nav>
                <btn-mono buttonText="Free Quote" />
            </div>
        </div>
    </header>
</template>

<script>
import BtnMono from "../secondary/BtnMono.vue";
export default {
    components: { BtnMono },
    name: "IntroSection",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

header {
    width: 100%;
    background-color: aqua;
    padding: 2rem 0;

    .wrapper {
        display: flex;
        justify-content: space-between;
        align-items: center;

        background-color: antiquewhite;

        @include wrapper-size;
    }

    .nav-container {
        display: flex;
        justify-content: center;
        align-items: center;

        ul {
            display: flex;

            li {
                @include title-list;
                text-transform: none;
                padding: 0 2rem;
            }
        }
    }
}
</style>
