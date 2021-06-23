<template>
<div>
    <div class="wrapper">
        <img src="../assets/img/amazon.svg" alt="">
        <img src="../assets/img/google.svg" alt="">
        <img src="../assets/img/lenovo.svg" alt="">
        <img src="../assets/img/paypal.svg" alt="">
        <img src="../assets/img/shopify.svg" alt="">
        <img src="../assets/img/spotify.svg" alt="">
    </div>
</div>
</template>

<script>
export default {
    name:'SezioneLoghi'

}
</script>

<style lang='scss' scoped>
div{
    width: 100%;
    border-bottom-left-radius: 35%;
    border-bottom-right-radius: 35%;
    background-color: #f8f9fc;
}
.wrapper{
    display: flex;
    justify-content: space-around;
    padding: 40px 0px;
   

    img{
        width: 70px;
    }
}

</style>