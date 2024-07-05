<script>
    export default{
        name: 'AppHeader'
    }
</script>

<template>
    <header class="container">
        <div id="box-image">
            <a href="#">
                <img src="../assets/dc-logo.png" alt="">
            </a>
        </div>

        <!-- navigazione -->
        <nav>
            <ul>
                <li>
                    <a href="#">Item</a>
                </li>
                <li>
                    <a href="#">Item</a>
                </li>
                <li>
                    <a href="#">Item</a>
                </li>
                <li>
                    <a href="#">Item</a>
                </li>
                <li>
                    <a href="#">Item</a>
                </li>
                <li>
                    <a href="#">Item</a>
                </li>
                <li>
                    <a href="#">Item</a>
                </li>
                <li>
                    <a href="#">Item</a>
                </li>
                <li>
                    <a href="#">Item</a>
                </li>
                <li>
                    <a href="#">Item</a>
                </li>
                
            </ul>
        </nav>
        
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header{

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
        }
    }


}

</style>