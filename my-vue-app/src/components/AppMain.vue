<template>
    <main>
        <div class="hero"></div>
        <ListDc/>
    </main>
</template>

<script>
    import ListDc from './ListDc.vue'

    export default {
        components: {
            ListDc
        }
    }
</script>

<style lang="scss" scoped>
    @use "../styles/partials/variables" as *;
    @use "../styles/partials/mixins" as *;

    main {
        background-color: $list-comics-color;
        .hero {
            width: 100%;
            height: 300px;
    
            background-image: url("../assets/jumbotron.jpg");
            background-repeat: no-repeat;
            background-size: cover;
        }
    }
</style>