<template lang="">
    <div class="my-bgc-footer">
       <div class="container">
        <div class="footer-banner py-4">
            <button class="btn btn-outline-primary text-white "> SIGN-UP NOW! </button>
            <div class="social-container ">
                <h5 class="clr-blue" >FOLLOW US </h5>
                <div class="social-icon">
                    <img src="img/footer-facebook.png" alt="">
                    <img src="img/footer-periscope.png" alt="">
                    <img src="img/footer-pinterest.png" alt="">
                    <img src="img/footer-twitter.png" alt="">
                    <img src="img/footer-youtube.png" alt="">
                </div>

            </div>
        </div>
       </div>
    </div>
  
</template>
<script>
export default {
 
}
</script>
<style scoped lang="scss">
@use "../styles/partials/variables"  as *;
.my-bgc-footer{
    background-color:$my-bgc-color-footer;
    
}
.footer-banner{
    display: flex;
    justify-content: space-between;
}
.clr-blue{
    color: $my-bgc-color-blue;
    margin: 0;
}
.social-container{
    display: flex;
    align-items: center;

}
.social-icon{
    padding: 0 1rem;
    img{
        padding: 0 .5rem;
    }
}

</style>