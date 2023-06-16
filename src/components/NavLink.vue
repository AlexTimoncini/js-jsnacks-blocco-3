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
    li{
        margin-bottom: 2rem;
        transition: all ease 0.3s;
        width: 100%;
        a{
            text-decoration: none;
            color: bisque;
            font-size: 6rem;
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            text-transform: uppercase;
            text-shadow: 5px 5px 10px #000;
        }

        &:hover{
            transform: scale(1.05);
            background-color: rgba(0, 0, 0, 0.1);
        }
    }
</style>
