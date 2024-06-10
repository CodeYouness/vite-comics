<script>
export default {
    data() {
        return {
            headerLink: [
    { id: 1, title: "characters", active: false, link: "#" },
    { id: 2, title: "comics", active: true, link: "#" },
    { id: 3, title: "movies", active: false, link: "#" },
    { id: 4, title: "tv", active: false, link: "#" },
    { id: 5, title: "games", active: false, link: "#" },
    { id: 6, title: "collectibles", active: false, link: "#" },
    { id: 7, title: "videos", active: false, link: "#" },
    { id: 8, title: "fan", active: false, link: "#" },
    { id: 9, title: "news", active: false, link: "#" },
    { id: 10, title: "shop", active: false, link: "#" }
]
        }
    },
}
</script>

<template>
    
    <header>
        <div class="container">
            <section class="image">
                <img src="../assets/img/dc-logo.png" alt="">
            </section>
            <section class="list-title">
                <ul>
                    <li v-for="(title,index) in headerLink" :key="title.id" :class="(title.active) ? 'active': ''">
                        {{ title.title }}
                    </li>
                </ul>
            </section>
        </div>
    </header>
</template>

<style lang='scss' scoped>
@use '../styles/partials/variable' as *;
@use '../styles/partials/mixin' as *;

.container {
    @include sp-between();
    align-items: center;
    max-width: $max-width;
    margin: 0 auto;
    font-weight: 600;
    font-size: 0.8rem;
    text-transform: uppercase;
    height: fit-content;
    .image {
    width: 8%;
        img {
            width: 100%;
        }
    }
    .list-title {
    display: flex;
    align-items: center;
        ul {
        display: flex;
        list-style-type: none;
            li {
                margin: 0 0.5rem;
                padding: calc(15vh/2) 0;
            }
            .active {
            color: $primary-color;
            border-bottom: 5px solid $primary-color;
            }
        }
    }
}








</style>