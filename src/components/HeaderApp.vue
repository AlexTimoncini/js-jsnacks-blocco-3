<script>
    import NavLink from './NavLink.vue';
    export default{
        name: 'HeaderApp',
        components: {
            NavLink,
        },
        data(){
            return{
                links: [
                    {
                        name: 'Home',
                        link: '#'
                    },
                    {
                        name: 'About',
                        link: '#'
                    },
                    {
                        name: 'Shop',
                        link: '#'
                    },
                    {
                        name: 'Contact Us',
                        link: '#'
                    },
                    {
                        name: 'Gallery',
                        link: '#'
                    },
                    {
                        name: 'Team',
                        link: '#'
                    },
                    {
                        name: 'API',
                        link: '#'
                    },
                ]
            }
        }
    }
</script>

<template>
    <header>
        <nav>
            <ul>
                <NavLink v-for="link in links" 
                :linkObj="link"/>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as *;
    @use '../styles/partials/variables.scss' as *;
    header{
        background-color: $primaryColor;
        height: 100vh;
        @include flex();
        ul{
            width: 100vw;
            list-style: none;
            text-align: center;
            overflow: hidden;
        }
    }
</style>
