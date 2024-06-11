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
    <img :src="singleCard.thumb" :alt="singleCard.type">
    <p>{{ singleCard.type }}</p>
</article>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variable' as *;
@use '../styles/partials/mixin' as *;

</style>