<script>
export default {
    props:{
        cardData: Object, 
    }
}
</script>
<template lang="">
    <div class="col-12 col-md-2">
        <div class="p-2 m-3">
            <img class="img-fluid" :src="cardData.thumb" alt="cardData.thumb">
            <h4 class="text-center">{{ cardData.series }}</h4>
        </div>
    </div>
</template>
<style lang="">
    
</style>