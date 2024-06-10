<script>
export default {
    data() {
        return {
            merch: [
                { id:1, product: 'digital comics', url: 'src/assets/img/buy-comics-digital-comics.png'},
                { id:2, product: 'dc merchandise', url: 'src/assets/img/buy-comics-merchandise.png'},
                { id:3, product: 'subscription', url: 'src/assets/img/buy-comics-subscriptions.png'},
                { id:4, product: 'comic shop locator', url: 'src/assets/img/buy-comics-shop-locator.png'},
                { id:5, product: 'dc power visa', url: 'src/assets/img/buy-dc-power-visa.svg'}
            ]
        }
    },
}
</script>

<template>
    <main>
        <section>
            <div v-for="product in merch">
                <img :src="product.url" alt="product.product">
                <p>{{ product.product }}</p>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variable' as *;
    @use '../styles/partials/mixin' as *;

    main {
        background-color: $primary-color;
        position: relative;
        z-index: 2;
        section {
            @include max-width();
            @include sp-around();
            align-items: center;
            height: 20vh;
            div {
                @include centered();
                height: 3rem;
                img {
                    height: 100%;
                    margin-right: 1rem;
                }

                p {
                    text-transform: uppercase;
                    color: white;
                    height: fit-content;
                    font-size: 0.8rem;
                }
            }
        }
    }
</style>