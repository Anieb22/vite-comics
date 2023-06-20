<script>
export default {
    name: "AppBlueLine",
    data() {
        return {
            links: [
                {
                    Img: "src/assets/img/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS",
                    url: "#",
                    current: false
                },
                {
                    Img: "src/assets/img/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE",
                    url: "#",
                    current: true
                },
                {
                    Img: "src/assets/img/buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION",
                    url: "#",
                    current: false
                },
                {
                    Img: "src/assets/img/buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR",
                    url: "#",
                    current: false
                },
                {
                    Img: "src/assets/img/buy-dc-power-visa.svg",
                    text: "DC POWER VISA",
                    url: "#",
                    current: false
                }
            ]
        }
    }

}
</script>
<template>
    <div class="background-blue">

    </div>
</template>
<style lang="scss" scoped>
.background-blue {
    background-color: blue;
    height: 200px;
}
</style>