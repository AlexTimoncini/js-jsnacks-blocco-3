<script>
    export default{
        name: 'NavLink',
        props: {
            linkObj : Object,
        }
    }
</script>

<template>
    <li>
        <a :href="linkObj.link">{{ linkObj.name }}</a>
    </li>
</template>

<style lang="scss" scoped>
    
</style>
