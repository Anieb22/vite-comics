<script>
export default {
    name: "AppBlueLine",
    data() {
        return {
            DcComics: [
                {
                    text: "Characters",
                    url: "#",
                },
                {
                    text: "Comics",
                    url: "#",
                },
                {
                    text: "Movies",
                    url: "#",
                },
                {
                    text: "TV",
                    url: "#",
                },
                {
                    text: "Games",
                    url: "#",
                },
                {
                    text: "Videos",
                    url: "#",
                },
                {
                    text: "News",
                    url: "#",
                }
            ],

            Shop: [
                {
                    text: "Shop DC",
                    url: "#",
                },
                {
                    text: "Shop DC Collectibles",
                    url: "#",
                }
            ],

            Dc: [
                {
                    text: "Terms Of Use",
                    url: "#",
                },
                {
                    text: "Privacy policy (New)",
                    url: "#",
                },
                {
                    text: "Ad Choices",
                    url: "#",
                },
                {
                    text: "Advertising",
                    url: "#",
                },
                {
                    text: "Jobs",
                    url: "#",
                },
                {
                    text: "Subscription",
                    url: "#",
                },
                {
                    text: "Talent Workshops",
                    url: "#",
                },
                {
                    text: "CPSC Certificates",
                    url: "#",
                },
                {
                    text: "Ratings",
                    url: "#",
                },
                {
                    text: "Shop Help",
                    url: "#",
                },
                {
                    text: "Contact Us",
                    url: "#",
                }
            ],

            Sites: [
                {
                    text: "DC",
                    url: "#",
                },
                {
                    text: "MAD Magazine",
                    url: "#",
                },
                {
                    text: "CD Kids",
                    url: "#",
                },
                {
                    text: "DC Universe",
                    url: "#",
                },
                {
                    text: "DC Power Visa",
                    url: "#",
                }
            ],
            Social: [
                {
                    img: "src/assets/img/footer-facebook.png",
                    url: "#",
                },
                {
                    img: "src/assets/img/footer-periscope.png",
                    url: "#",
                },
                {
                    img: "src/assets/img/footer-pinterest.png",
                    url: "#",
                },
                {
                    img: "src/assets/img/footer-twitter.png",
                    url: "#",
                },
                {
                    img: "src/assets/img/footer-youtube.png",
                    url: "#",
                }
            ]
        }
    }
}
</script>
<template>
    <footer>
        <div class="container-footer container">
            <div class="container-ul">
                <ul> DC COMICS
                    <li v-for="(link, index) in DcComics" :key="index">
                        <a :href="link.url">
                            {{ link.text }}
                        </a>
                    </li>
                    <ul> SHOP
                        <li v-for="(link, index) in Shop" :key="index">
                            <a :href="link.url">
                                {{ link.text }}
                            </a>
                        </li>
                    </ul>

                </ul>
                <ul> DC
                    <li v-for="(link, index) in Dc" :key="index">
                        <a :href="link.url">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
                <ul> SITES
                    <li v-for="(link, index) in Sites" :key="index">
                        <a :href="link.url">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="background-footer">
            <div class="container container-footer2">
                <button>
                    <h3>SING-UP NOW</h3>
                </button>
                <ul class="social"> FOLLOW US
                    <li v-for="(link, index) in Social" :key="index">
                        <a :href="link.url">
                            <img :src="link.img" alt="">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
.container-ul {
    width: 40%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-position: center;
    background-size: cover;

}

.container-footer {
    height: 350px;
    display: flex;
    align-items: center;
}

.container-footer2 {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}

.background-footer {
    background-color: rgb(54, 54, 54);
}

.social {
    display: flex;
    flex-direction: row;
    align-items: center;
    color: #0282F9;
}

img {
    margin-left: 10px;
}

ul {
    text-align: left;
    font-weight: 800;
    color: white;
}

a {
    font-weight: 100;
    color: lightgray;
}

button {
    margin: 30px 0;
    background-color: rgb(54, 54, 54);
    border: 1px solid #0282F9;
    padding: 10px;
    color: white;
}
</style>