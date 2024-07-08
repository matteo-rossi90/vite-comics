<script>

    export default{
        name: 'Cards'
    }

</script>

<template>

    <div class="card-items">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

    <div class="card-items">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <h3>Prezzo: 5 euro</h3>
        <h4>Serie</h4>
        <h5>Tipo</h5>
    </div>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.card-items{
    width: calc((100% / 6) - 20px);
    margin: 5px;
    cursor: pointer;

    img{
        max-height: 200px;
        width: 100%;
        object-fit: cover;
    }

    h3,
    h4,
    h5{
        color: white;
    }
}

</style>