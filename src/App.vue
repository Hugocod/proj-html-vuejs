<template>
    <div>
        <intro-section data-aos="fade-up" data-aos-duration="700" />
        <info-section-award data-aos="fade-up" data-aos-duration="700" />
        <service-section data-aos="fade-up" data-aos-duration="700" />
        <info-section-moving data-aos="fade-up" data-aos-duration="700" />
        <testimonials-section data-aos="fade-up" data-aos-duration="700" />
        <cta-section data-aos="fade-up" data-aos-duration="700" />
        <footer-section data-aos="fade-up" data-aos-duration="700" />
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

    -webkit-touch-callout: none; /* iOS Safari */
    -webkit-user-select: none; /* Safari */
    -khtml-user-select: none; /* Konqueror HTML */
    -moz-user-select: none; /* Old versions of Firefox */
    -ms-user-select: none; /* Internet Explorer/Edge */
    user-select: none;
}

body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

p {
    line-height: 2rem !important;
}
</style>
