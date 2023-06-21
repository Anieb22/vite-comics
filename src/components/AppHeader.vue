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
          <li v-for="(link, index) in  links " :key="index">
            <a :href="link.url" :class="{ active: link.current }" class="linea-blu">
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

.linea-blu {
  padding-bottom: 60px;
}

li {
  margin-left: 20pt;

  & .active,
  & :hover {
    border-bottom: 4px solid #0282F9;
  }

}

a {
  color: black;

  & :hover {
    color: #0282F9;
  }
}
</style>