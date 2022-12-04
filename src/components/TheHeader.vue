<template>
    <div class="container my-bgc-white">
        <div class="my-nav-bar">
            <div class="logo-dc">
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
.links{
    list-style: none;
    display: flex;

    a{
        color: $my-bgc-color-dark;
        text-decoration: none;
        padding: 10px;
         
    }
}
    
</style>