<template>
    <div class="jumbo">

    </div>
    <div class="my-bgc-dark">
        <div class="container py-4">
            <ComicList></ComicList>
        </div>
    </div>
</template>
<script>
import ComicList from './ComicList.vue';
export default {
    components:{ComicList},
    data() {
        return {
            
        }
    },
    
}
</script>
<style scoped lang="scss">
@use "../styles/partials/variables"  as *;
.my-bgc-dark{
    background-color:$my-bgc-color-dark;
    
}
.jumbo{
    background-image: url("./img/jumbotron.jpg");
    object-fit: cover;
    height: 400px;
    background-repeat: no-repeat;
}
    
</style>