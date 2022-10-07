<template>
    <div class="container">
        <h3>title</h3>
        <ul>
            <li v-for="n in 5" :key="n">
                <a>link{{ n }}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "ListBlock",
};
</script>

<style scoped lang="scss">
@import "../../scss/_resources.scss";

.container {
    h3 {
        @include title-list;
        margin-bottom: 1rem;
    }

    li {
        margin-bottom: 1rem;
    }
}
</style>
