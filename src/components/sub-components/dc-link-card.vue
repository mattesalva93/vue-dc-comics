<template>

    <div class="card-container">
        <img src="../../assets/img/buy-comics-digital-comics.png" alt="">
        <span>Digital Comics</span>
    </div>
 
</template>

<script>
export default {
    name: "dc-link-card"
}
</script>

<style lang="scss">
    .card-container{
        height: 165px;
        display: flex;
        align-items: center;
        color: white;
        text-transform: uppercase;

        img{
            height: 40%;
            width: auto;
            margin-right: 10px;
        }
    }
</style>