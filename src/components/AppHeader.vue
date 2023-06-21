<script>
export default {
  name: "AppHeader",
  data() {
    return {
      logo: "src/assets/img/dc-logo.png",
      links: [
        {
          text: "CHARACTERS",
          url: "#",
          current: false
        },
        {
          text: "COMICS",
          url: "#",
          current: true
        },
        {
          text: "MOVIES",
          url: "#",
          current: false
        },
        {
          text: "TV",
          url: "#",
          current: false
        },
        {
          text: "GAMES",
          url: "#",
          current: false
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          current: false
        },
        {
          text: "VIDEOS",
          url: "#",
          current: false
        },
        {
          text: "FANS",
          url: "#",
          current: false
        },
        {
          text: "NEWS",
          url: "#",
          current: false
        },
        {
          text: "SHOP",
          url: "#",
          current: false
        },
      ]
    }
  }
}

</script>
<template>
  <header>
    <div class="container-header">

      <a href="#" class="logo">
        <img :src="logo" alt="logo">
      </a>

      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.url" :class="{ active: link.current }">
              {{ link.text }}
            </a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>
<style lang="scss" scoped>
.container-header {
  height: 150px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: white;
}

ul {
  display: flex;
  flex-direction: row;
}

li {
  margin-left: 20pt;
  list-style-type: none;
}
</style>