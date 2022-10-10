<template>
    <div class="container">
        <h3>{{ title }}</h3>
        <ul>
            <li v-for="(link, index) in links" :key="index + link">
                <a><font-awesome-icon icon="fa-solid fa-chevron-right" /> {{ link }}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "ListBlock",
    props: ["links", "title"],
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    h3 {
        @include title-list;
        margin-bottom: 2.2rem;
    }

    li {
        margin-bottom: 1.8rem;
        font-weight: 400;
        cursor: pointer;
        & :hover {
            color: $color-green-vivid;
        }
    }
}
</style>
