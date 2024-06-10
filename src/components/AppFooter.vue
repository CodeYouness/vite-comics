<script>
export default {
    data() {
        return {
            dcComicsLink: [
                { id: 1, title: "Characters", link: "#" },
                { id: 2, title: "Comics", link: "#" },
                { id: 3, title: "Movies", link: "#" },
                { id: 4, title: "TV", link: "#" },
                { id: 5, title: "Games", link: "#" },
                { id: 6, title: "Videos", link: "#" },
                { id: 7, title: "News", link: "#" }
            ],

            shop: [
                { id: 1, title: "Shop DC", link: "#" },
                { id: 2, title: "Shop DC Collectibles", link: "#" },
            ],

            dc: [
                { id: 1, title: "Term Of Use", link: "#" },
                { id: 2, title: "Privacy Policy (New)", link: "#" },
                { id: 3, title: "Ad Choices", link: "#" },
                { id: 4, title: "Advertising", link: "#" },
                { id: 5, title: "Jobs", link: "#" },
                { id: 6, title: "Subscription", link: "#" },
                { id: 7, title: "Tallene Workshop", link: "#" },
                { id: 8, title: "CPSC Certificates", link: "#" },
                { id: 9, title: "Ratings", link: "#" },
                { id: 10, title: "Shop Help", link: "#" },
                { id: 11, title: "Contact Us", link: "#" }
            ],

            sites: [
                { id: 1, title: "DC", link: "#" },
                { id: 2, title: "MAD Magazine", link: "#" },
                { id: 3, title: "DC Kids", link: "#" },
                { id: 4, title: "DC Universe", link: "#" },
                { id: 5, title: "DC Power Visa", link: "#" }
            ]
        }
    },
}
</script>

<template>
    <footer>
        <div class="container">
            <section class="link">
                <nav>
                    <h2>dc comics</h2>
                    <ul>
                        <li v-for="(title, index) in dcComicsLink">
                            {{ title.title }}
                        </li>
                    </ul>
                    <h2>shop</h2>
                    <ul>
                        <li v-for="title in shop">
                            {{ title.title }}
                        </li>
                    </ul>
                </nav>
                <nav>
                    <h2>dc</h2>
                    <ul>
                        <li v-for="title in dc">
                            {{ title.title }}
                        </li>
                    </ul>
                </nav>
                <nav>
                    <h2>dc</h2>
                    <ul>
                        <li v-for="title in sites">
                            {{ title.title }}
                        </li>
                    </ul>
                </nav>
            </section>
        
            <section class="logo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </section>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variable' as *;
@use '../styles/partials/mixin' as *;
footer {
    background-image: url(../assets/img/footer-bg.jpg);
    .container {
        @include max-width();
        position: relative;
    }
    .link {
        @include max-width();
        display: flex;
        align-items: start;
        padding: 3rem 0;
        h2 {
            text-transform: uppercase;
            color: white;
            font-size: 1.3rem;
        }
        ul {
            padding: 1rem 0;
            li {
                color: $secondary-txt;
                padding: 0.2rem 2rem 0.2rem 0;
                font-size: 0.8rem
            }
        }
    }

    .logo {
        img {
            position: absolute;
            right: 0;
            top: -25%;
            z-index: 1;
        }
    }
}
</style>