<script>

</script>

<template>
    <header>
        <h1>Main Logo</h1>
        <nav>
            <ul v-for="n in 4">
                <li>Home</li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as *;
    @use '../styles/partials/variables.scss' as *;
    header{
        background-color: $primaryColor;
    }
</style>
