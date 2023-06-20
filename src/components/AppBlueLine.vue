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
                },
                {
                    Img: "src/assets/img/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE",
                    url: "#",
                },
                {
                    Img: "src/assets/img/buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION",
                    url: "#",
                },
                {
                    Img: "src/assets/img/buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR",
                    url: "#",
                },
                {
                    Img: "src/assets/img/buy-dc-power-visa.svg",
                    text: "DC POWER VISA",
                    url: "#",
                }
            ]
        }
    }

}
</script>
<template>
    <div class="background-blue">
        <ul>
            <li v-for="(link, index) in links" :key="index">
                <a :href="link.url">
                    <img :src="link.Img" alt="image">
                    {{ link.text }}
                </a>
            </li>
        </ul>

    </div>
</template>
<style lang="scss" scoped>
.background-blue {
    background-color: blue;
    height: 200px;
    align-items: center;
    display: flex;
}

ul {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

li {
    margin-left: 20pt;
    list-style-type: none;
    color: white;
}

a {
    display: flex;
    align-items: center;
}

img {
    width: 70px;
}
</style>