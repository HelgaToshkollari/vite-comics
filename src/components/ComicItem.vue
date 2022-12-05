<template lang="">
    <div class="card" style="width: 18rem;">
        <img class="card-img-top" :src="comic.thumb" alt="Card image cap">
        <div class="card-body">
        <p class="card-text">{{comic.series}}</p>
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
<style lang="">
    
</style>