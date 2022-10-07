<template>
    <div>
        <intro-section />
        <info-section-award />
    </div>
</template>

<script>
import InfoSectionAward from "./components/primary/InfoSectionAward.vue";
import IntroSection from "./components/primary/IntroSection.vue";
export default {
    name: "App",
    components: { IntroSection, InfoSectionAward },
};
</script>

<style lang="scss">
#app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    font-family: "Roboto", sans-serif;
    text-align: center;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    color: #2c3e50;
}

body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
</style>
