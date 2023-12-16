<template>
    <main>
        <div class="hero"></div>
        <ListComics/>
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
            height: 100px;
    
            background-image: url("../assets/img/jumbotron.jpg");
            background-repeat: no-repeat;
            background-size: cover;
        }
    }
</style>