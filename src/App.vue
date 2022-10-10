<template>
    <div>
        <intro-section />
        <info-section-award />
        <service-section />
        <info-section-moving />
        <testimonials-section />
        <cta-section />
        <footer-section />
    </div>
</template>

<script>
import CtaSection from "./components/primary/CtaSection.vue";
import FooterSection from "./components/primary/FooterSection.vue";
import InfoSectionAward from "./components/primary/InfoSectionAward.vue";
import InfoSectionMoving from "./components/primary/InfoSectionMoving.vue";
import IntroSection from "./components/primary/IntroSection.vue";
import ServiceSection from "./components/primary/ServiceSection.vue";
import TestimonialsSection from "./components/primary/TestimonialsSection.vue";
export default {
    name: "App",
    components: { IntroSection, InfoSectionAward, InfoSectionMoving, ServiceSection, TestimonialsSection, CtaSection, FooterSection },
};
</script>
, CtaSection
<style lang="scss">
#app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    font-family: "Roboto", sans-serif;

    margin: 0;
    padding: 0;
    box-sizing: border-box;
    color: #2c3e50;
}

body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    /*  pointer-events: none; */
}

p {
    line-height: 2rem !important;
}
</style>
