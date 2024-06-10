<script>
export default {
    data() {
        return {
        }
    },
}
</script>

<template>
    <main>
        <div class="content">

            <p>--> content goes here<--</p>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variable' as *;
@use '../styles/partials/mixin' as *;
main {
    background-color: $dark-bg;
    padding: 3rem 0;
    color: white;
    .content {
        @include max-width()
    }

}
</style>