<template lang="">
    <div class="my-bgc-footer-img">
        <div class="container">
            <div class="row d-flex justify-content-between ">
                <div class=" col-sm-2 text-white " v-for=" ftLink in footerArray">
                    <div class="footer-link-list">
                        <h3>{{ ftLink.title}}</h3>
                        <ul class="list-unstyled text-secondary ">
                            <li v-for="linkName in ftLink.footerLinks "> {{linkName}} </li>
                        </ul>
                    </div>
                </div>
                <div class="col-sm-4 ">
                    <img class="img-fluid" src="img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
    </div>
  
</template>
<script>
export default {
    data(){
        return{
            footerArray:[
                {
                    title:"DC COMICS",
                    footerLinks:["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
                    
                },
                {
                    title:"SHOP",
                    footerLinks:["Shop DC", "Shop DC Collectibles"],
                },
                {
                    title:"DC",
                    footerLinks:["Terms Of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
                },
                {
                    title:"SITES",
                    footerLinks:["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
                },
              
            ]
        }
    }
    
}
</script>
<style scoped lang="scss">
@use "../styles/partials/variables"  as *;
.my-bgc-footer-img{
    background-image: url("./img/footer-bg.jpg");
    object-fit: cover;
}
.footer-link-list{
    padding: 1rem;
}
</style>