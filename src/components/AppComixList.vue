<script>
export default {
    props: {
        image: String,
        title: String,
        price: String,
        type: tring,

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
<style lang="scss">
h3,
h5 {
    color: white;
}

.card {
    width: calc(100% / 6 - 20px);
    margin: 10px 0;
}

img {
    width: 60%;
}
</style>