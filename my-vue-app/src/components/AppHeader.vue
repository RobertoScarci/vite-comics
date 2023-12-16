<template>
    <header>
        <div class="imgWrapper">
            <img src="../assets/dc-logo.png" alt="Logo DC">
        </div>
        <nav>
            <ul>
                <li v-for="link in navLinks" :class=" (link.active) ? 'active' : '' ">
                    <a :href="link.href">
                        {{ link.name }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
    export default {
        name: "AppHeader",
        data() {
            return {
                navLinks: [
                    {
                        name: "Characters",
                        active: false
                    },
                    {
                        name: "Comics",
                        active: true
                    },
                    {
                        name: "Movies",
                        active: false
                    },
                    {
                        name: "Tv",
                        active: false
                    },
                    {
                        name: "Games",
                        active: false
                    },
                    {
                        name: "Tv",
                        active: false
                    },
                    {
                        name: "Collectibles",
                        active: false
                    },
                    {
                        name: "Videos",
                        active: false
                    },
                    {
                        name: "News",
                        active: false
                    },
                    {
                        name: "Shop",
                        active: false
                    },
                ]
            }
        }
    }
</script>
<style lang="scss" scoped>
    @use "../styles/partials/variables" as *;
    @use "../styles/partials/mixins" as *;
    header {
        width: 100%;
        height: 110px;
        @include flex();
        div.imgWrapper {
            width: 40%;
            @include flex(row, center, center);
            img {
                height: 70%;
            }
        }
        nav ul {
            height: 80%;
            @include flex(row, center);
            list-style: none;
            li {
                line-height: 70px;
                margin-right: 2rem;
                text-transform: uppercase;
                font-weight: bold;
                font-size: 0.9rem;
                &.active {
                    border-bottom: 4px solid $main-color;
                    a {
                        color: $main-color;
                    }
                }
            }
            li:hover{
                color: #0082F9;
            }
        }
    }
</style>