<script>
    export default{
        name: 'AppHeader',
        data(){
            return{

                menuItems: [
                    {
                        text: "CHARACTERS",
                        current: false
                    },
                    {
                        text: "COMICS",
                        current: true
                    },
                    {
                        text: "MOVIES",
                        current: false
                    },
                    {
                        text: "TV",
                        current: false
                    },
                    {
                        text: "GAMES",
                        current: false
                    },
                    {
                        text: "VIDEOS",
                        current: false
                    },
                    {
                        text: "FANS",
                        current: false
                    },
                    {
                        text: "NEWS",
                        current: false
                    },
                    {
                        text: "SHOP",
                        current: false
                    }
                ]
            }
        }
    }
</script>

<template>
    <header class="container">

        <!-- logo -->
        <div id="box-image">
            <a href="#">
                <img src="../assets/dc-logo.png" alt="">
            </a>
        </div>

        <!-- inserimento dinamico in DOM del menu di navigazione -->
        <nav>
            <ul>
                <li v-for="(item, index) in menuItems" :key="index">
                    <a href="#" :class="{active: item.current}">{{ item.text }}</a>
                </li>
                
            </ul>
        </nav>
        
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header{

    height: 100px;
    padding: 10px;
    @include flexbox();

    #box-image img{
        max-width: 70%;
    }

    ul{
        display: flex;
        gap: 20px;
        list-style: none;

        li a{
            font-weight: 600;
            text-decoration: none;
            padding: 38px 0;
            font-size: 12px;
        }

        .active{
            border-bottom: 4px solid $merch;
            color: $merch
        }
    }


}

</style>