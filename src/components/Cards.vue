<script>

    export default{
        name: 'Cards',
        props:{
            details: Object
        }
    }

</script>

<template>

    <div class="card-items">
        <img :src="details.thumb" alt="">
        <h3>{{ details.series }}</h3>
    </div>


</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.card-items{
    width: calc((100% / 5) - 60px);   
    margin: 5px;
    cursor: pointer;

    img{
        max-height: 200px;
        width: 100%;
        object-fit: cover;
        object-position: top;
    }

    h3{
        color: white;
        margin: 5px 0;
        font-weight:lighter;
    }
}

</style>