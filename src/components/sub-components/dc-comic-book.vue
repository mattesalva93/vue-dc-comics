<template>

    <div class="comic-container">
        <img :src="dccomic.thumb" :alt="dccomic.type">
        <h4>{{dccomic.series}}</h4>
    </div>
 
</template>

<script>
export default {
    name: "dc-comic-book",
    props: {
        'dccomic': Object
    }
}
</script>

<style lang="scss">
    .comic-container{
        margin: 50px 0;
        padding: 15px;
        height: 250px;
        width: 15%;
        text-align: center;
        h4{
            color: white;
        }
        img{
            height: 100%;
            width: auto;
        }
    }
</style>