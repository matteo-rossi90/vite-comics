<script>
    export default{
        name: 'AppMerch',
        data(){
            return{

                merchItems: [
                    {
                        text: "DIGITAL COMICS",
                        image: "buy-comics-digital-comics.png",
                    },
                    {
                        text: "DC MERCHANDISE",
                        image: "buy-comics-merchandise.png"
                    },
                    {
                        text: "SUBSCRIPTIONS",
                        image: "buy-comics-subscriptions.png"
                    },
                    {
                        text: "COMIC SHOP LOCATOR",
                        image: "buy-comics-shop-locator.png"
                    },
                    {
                        text: "DC POWER VISA",
                        image: "buy-dc-power-visa.svg"
                    },
                ]
            }
        }
    }
</script>

<template>

    <section id="merch">
        <div class="container-content">
            <nav>
                <ul>
                    <li v-for="(merch, index) in merchItems" :key="index">
                        <img :src="merch.image" :alt="merch.text">
                        <a href="#">{{ merch.text }}</a>
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
    padding: 25px;
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