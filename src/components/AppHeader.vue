<script>
export default {
    data() {
        return {
            headerLink: [
    { id: 1, title: "characters", active: false },
    { id: 2, title: "comics", active: true },
    { id: 3, title: "movies", active: false },
    { id: 4, title: "tv", active: false },
    { id: 5, title: "games", active: false },
    { id: 6, title: "collectibles", active: false },
    { id: 7, title: "videos", active: false },
    { id: 8, title: "fan", active: false },
    { id: 9, title: "news", active: false },
    { id: 10, title: "shop", active: false }
]
        }
    },
}
</script>

<template>
    <div>
        <p v-for="title in headerLink">{{title.title}}</p>
    </div>
</template>

<style scoped>

</style>