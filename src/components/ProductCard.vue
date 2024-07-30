<script>
export default {
    props:{
        pathImage: String,
        title: String 
    }
}
</script>
<template lang="">
    <div class="col-12 col-md-2">
        <div class="p-2 m-3">
            <img class="img-fluid" :src="pathImage" alt="title">
            <h4 class="text-center">{{ series }}</h4>
        </div>
    </div>
</template>
<style lang="">
    
</style>