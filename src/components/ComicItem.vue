<template lang="">

    <div class="my-card" style="width: 18rem;">
        <div class="my-card-img ratio ratio-1x1">
            <img class="img-fluid" :src="comic.thumb" alt="">
        </div>
        <div class="fs-6 py-2">
            <p class="text-white">{{comic.series}}</p>
        </div>

     
    </div>
    
</template>
<script>
export default {
    props: {
        comic:{
            type: Object,
        }
    }
    
}
</script>
<style scoped lang="scss">
@use "../styles/partials/variables"  as *;

.my-card-img{
    width: 100%;
    
    img{
        width: 100%;
        object-fit: cover;
        display: block;
        aspect-ratio: 1/1;
    }
}

    
</style>