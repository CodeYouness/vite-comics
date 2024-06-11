<script>
export default {
    data() {
        return {
        }
    },
    props: {
        singleCard: {
            type: Object,
            required:true 
        }
        
    }
}
</script>

<template>
<article>
    <div>
        <img :src="singleCard.thumb" :alt="singleCard.type">
    </div>
    <p>{{ singleCard.series }}</p>
</article>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variable' as *;
@use '../styles/partials/mixin' as *;

article {
    width: calc((100%/6) - 1.5rem);
    margin-left: 1.5rem;
    height: 40vh;
    text-transform: uppercase;

    div {
        height: 70%;
        overflow: hidden;
        img {
                width: 100%;
            }
        }
    p {
        padding-top: 1rem;
        font-size: 0.8rem;
    }
}

</style>