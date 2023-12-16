<template>
    <div class="listComics">
        <h1>Content goes here</h1>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
    @use "../styles/partials/variables" as *;
    @use "../styles/partials/mixins" as *;
    .listComics {
        background-color: $list-comics-color;
        padding: 3rem 10rem;
        h1 {
            color: white;
        }
    }
</style>