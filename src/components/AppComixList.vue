<script>
export default {
    props: {
        image: string,
        title: string,
        price: string,
        type: string,

    }
}
</script>

<template lang="">
    <div>
        <img :src="image" class="card-img-top" alt="card">
                    <div class="card-body">
                        <h3 class="card-text">{{ title }}</h3>
                        <h3 class="card-text">{{ price }}</h3>
                        <h5 class="card-text">{{ type }}</h5>
                    </div>
    </div>
</template>
<style lang="">
    
</style>