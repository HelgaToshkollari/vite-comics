<template>
    <div class="container my-bgc-white">
        <div class="my-nav-bar py-3">
            <div class="logo-dc ">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <div class="nav-bar-links">
                <ul class="links">
                    <li v-for="links in navbarLinks"><a href="#"> <strong>{{links.link}}</strong></a></li>
                </ul>

            </div>

        </div>

        
    </div>
</template>
<script>
export default {
    data(){
        return{
            navbarLinks: [
                {
                    link: "CHARACTERS"

                },
                {
                    link: "COMICS"

                },
                {
                    link: "MOVIES"

                },
                {
                    link: "TV"

                },
                {
                    link: "GAMES"

                },
                {
                    link: "COLLECTIBLES"

                },
                {
                    link: "VIDEOS"

                },
                {
                    link: "FANS"

                },
                {
                    link: "NEWS"

                },
                {
                    link: "SHOP"

                },

            ],
        }
    }
    
}
</script>
<style scoped lang="scss">
@use "../styles/partials/variables"  as *;
.my-bgc-white{
    background-color:$my-bgc-color-header;
    
}
.my-nav-bar{
    display: flex;
    justify-content: space-between;
    align-items: center;

}
.logo-dc img{
    width: 80px;
}
.links{
    list-style: none;
    display: flex;

    & li:hover{
        border-bottom: 5px solid $my-bgc-color-blue;
    }

    a{
        color: $my-bgc-color-dark;
        text-decoration: none;
        padding: 10px;

        &:hover{
            color: $my-bgc-color-blue;

        }
        
         
    }
}
    
</style>