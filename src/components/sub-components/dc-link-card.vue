<template>

    <div class="card-container">
        <img :src="dclink.src" :alt="dclink.title">
        <span>{{dclink.title}}</span>
    </div>
 
</template>

<script>
export default {
    name: "dc-link-card",
    props: {
        'dclink': Object
    }
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