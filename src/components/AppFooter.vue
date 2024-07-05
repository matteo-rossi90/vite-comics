<script>
    export default{
        name: 'AppFooter'
    }
</script>

<template>
    
    <section>

        <div class="background">

            <div class="container">

                <div id="flex-wrap">
                    
                    <div class="col">

                        <nav class="navigation">
        
                            <h3>DC-Comics</h3>
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
                            </ul>
                            
                        </nav>
                        <nav class="navigation">
                            <h3>SHOP</h3>
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
                            </ul>
                        </nav>
                    </div>

                    <div class="col">
                        <nav class="navigation">
                            <h3>DC</h3>
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
                            </ul>
                            
                        </nav>
                    </div>

                    <div class="col">
                        <nav class="navigation">
                            <h3>SITES</h3>
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
                            </ul>
                        </nav>
                    </div>

                </div>
    
            </div>


        </div>

    </section>

    <section id="bottom-bar">
        <div class="container" id="flex-container">
            
            <a href="#" id="btn-sign">
                <span>SIGN-UP NOW!</span>
            </a>


            <div id="list-icon">
                <h3 id="title">FOLLOW US</h3>
                <nav>
                    <ul>
                        <li>
                            <a href="#">
                                <img src="../assets/footer-facebook.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/footer-periscope.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/footer-facebook.png" alt="">
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>

        </div>
    </section>
    
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.background{
    background-image: url('../assets/dc-logo-bg.png'), url('../assets/footer-bg.jpg');
    background-size: 30%, cover;
    background-position-x: 75%;
    background-position-y: center;
    background-repeat: no-repeat;
    // height: 400px;

    #flex-wrap{

        display:flex;
        gap: 20px;

        .navigation{

            padding: 20px 0;

            h3{
                color: white;
            }
            ul{
                list-style-type: none;
                padding: 10px 0;
            }
            li a{
                color:rgb(165, 165, 165);
                text-decoration: none;
                font-size: 10px;
            }
        }
    }

}

#bottom-bar{
    background-color: $bottomFooter;
    // height: 100px;
    padding: 20px 0;
    
    a{
        text-decoration: none;
        color: white;
    }

    #btn-sign{
        border: 2px solid $merch;
        padding: 12px 16px;
    }
    
    #flex-container{
        @include flexbox();

        ul{
            text-decoration: none;
            list-style-type: none;
            display: flex;
            gap: 10px;
        }

        #list-icon{
            display: flex;
            align-items: center;
            gap: 10px;

            #title{
                color: $merch;
                font-weight: 600;
                padding: 0 20px;
            }

            li img{
                max-width: 80%;
            }
        }
    }
}
</style>