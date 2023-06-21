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
            ]
        }
    }
}
</script>
<template>
    <div class="container-footer">
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
</template>
<style>
.container-ul {
    width: 30%;
    display: flex;
    flex-direction: row;
}

.container-footer {
    height: 350px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-position: center;
    display: flex;
    align-items: center;
}

ul {
    list-style-type: none;
    text-align: left;
    font-weight: 800;
    color: white;
}
</style>