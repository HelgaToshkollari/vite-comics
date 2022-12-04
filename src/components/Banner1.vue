<template >
    <div class="my-bgc-blue">
        <div class="container"> 
            <div class="my-banner" >
                <ul class=" my-banner-ul list-unstyled py-3 ">
                    <li class="" v-for="(icons, i) in iconLinks" :key="i">
                        <div class="">
                            <img class="size-sm" :src="icons.iconImg">
                            {{icons.iconName}} 
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            iconLinks:[
                {
                    iconImg: "img/buy-comics-digital-comics.png",
                    iconName: "DIGITAL COMICS"
                },
                {
                    iconImg: "img/buy-comics-merchandise.png",
                    iconName: "DC MERCHANDISE"
                },
                {
                    iconImg: "img/buy-comics-subscriptions.png",
                    iconName: "SUBSCRIPTION"
                },
                {
                    iconImg: "img/buy-comics-shop-locator.png",
                    iconName: "COMIC SHOP LOCATION"
                },
                {
                    iconImg: "img/buy-dc-power-visa.svg",
                    iconName: "DC POWER VISA"
                },
            ]
        }
    }
    
}
</script>
<style scoped lang="scss">
@use "../styles/partials/variables"  as *;
.my-bgc-blue{
    background-color:$my-bgc-color-blue;
    
}
.my-banner-ul{
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    margin: 0;

    li{
        padding: 1.5rem ;

        img{
            width: 60px;
            padding: .5rem;
        }
    }
}
    
</style>