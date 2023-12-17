<script>
    export default {
        name: "SingleCard",
        props: {
            thumb: String,
            price: String,
            series: String,
            type: String,
        }
    }
</script>

<template>
    <article>
        <div class="imgWrapper">
            <img :src="thumb" :alt="series + '\'s thumb'">
        </div>
        <p> {{ series }} </p>
    </article>
</template>

<style lang="scss" scoped>
    @use "../styles/partials/variables" as *;
    @use "../styles/partials/mixins" as *;

    article {
        width: calc(100% / 6 - 3rem);
        margin-right: 1rem;
        margin-bottom: 1rem;

        .imgWrapper {
            width: 180px;
            height: 150px;

            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top;
            }
            img:hover{
                opacity: 0.5;
            }
        }

        p {
            margin: 1rem 0;
            color: white;
            text-transform: uppercase;
            font-size: 1rem;
        }

    }
</style>