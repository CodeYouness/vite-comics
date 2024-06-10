<script>
export default {
    data() {
        return {
            DcComicsLink: [
                { id: 1, title: "Characters", link: "#" },
                { id: 2, title: "Comics", link: "#" },
                { id: 3, title: "Movies", link: "#" },
                { id: 4, title: "TV", link: "#" },
                { id: 5, title: "Games", link: "#" },
                { id: 6, title: "Videos", link: "#" },
                { id: 7, title: "News", link: "#" }
                ]
        }
    },
}
</script>

<template>
    <footer>
        <section class="link">
            <nav>
                <h2>DC COMICS</h2>
                <ul>
                    <li v-for="(title, index) in DcComicsLink">
                        {{ title.title }}
                    </li>
                </ul>
            </nav>
        </section>
        <section class="logo">
            
        </section>
    </footer>
</template>

<style scoped>

</style>