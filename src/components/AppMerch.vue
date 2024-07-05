<script>
    export default{
        name: 'AppMerch'
    }
</script>

<template>

    <section id="merch">
        <div class="container-content">
            <nav>
                <ul>
                    <li>
                        <img src="../assets/buy-comics-digital-comics.png" alt="digital-comic">
                        <a href="#">DIGITAL COMICS</a>
                    </li>
                    <li>
                        <img src="../assets/buy-comics-merchandise.png" alt="digital-comic">
                        <a href="#">MERCHANDISE</a>
                    </li>
                    <li>
                        <img src="../assets/buy-comics-shop-locator.png" alt="digital-comic">
                        <a href="#">SHOP LOCATOR</a>
                    </li>
                    <li>
                        <img src="../assets/buy-comics-subscriptions.png" alt="digital-comic">
                        <a href="#">SUBSCRIPTIONS</a>
                    </li>
                    <li>
                        <img src="../assets/buy-dc-power-visa.svg" alt="digital-comic">
                        <a href="#">DC POWERVISA</a>
                    </li>
                </ul>
            </nav>
        </div>
    </section>


</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

#merch{
    background-color: $merch;
    height: 150px;
    padding: 20px;
    display: flex;
    align-items: center;

    ul{
        list-style-type: none;
        @include flexbox();

        li {
            width: 50px;
            gap: 10px;
            @include flexbox(); 

            img{
                max-width: 80%;
            }

            a{
                text-decoration: none;
                color: white;
                font-size: 13px;
            }
        }
    }
}

</style>