<template>
  <div class="god">
    <nav class="container d-flex align-items-center justify-content-between">
      <span>
        <img src="img/dc-logo.png" alt="Logo" />
      </span>
      <ul class="d-flex m-0 p-0">
        <li
          @click="changeActiveOption(option.id)"
          :class="activeElement(option.id)"
          v-for="(option, id) in menu"
          :key="option.id"
        >
          <a href="#">{{ option.text }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
  data() {
    return {
      menu: [
        {
          id: 1,
          text: "CHARACTERS",
        },
        {
          id: 2,
          text: "COMICS",
        },
        {
          id: 3,
          text: "MOVIES",
        },
        {
          id: 4,
          text: "TV",
        },
        {
          id: 5,
          text: "GAMES",
        },
        {
          id: 6,
          text: "COLLECTIBLES",
        },
        {
          id: 7,
          text: "VIDEOS",
        },
        {
          id: 8,
          text: "FANS",
        },
        {
          id: 9,
          text: "NEW",
        },
        {
          id: 10,
          text: "SHOP",
        },
      ],
      activeOption: 0,
    };
  },
  methods: {
    changeActiveOption(id) {
      for (let i = 0; i < this.menu.length; i++) {
        if (this.menu[i].id === id) {
          this.activeOption = i;
        }
      }
    },
    activeElement(id) {
      if (this.menu[this.activeOption].id === id) {
        return "is-active";
      }
    },
  },
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;
.god {
  background-color: white;
  color: black;
}
.is-active {
  border-bottom: 5px solid $color-electric-blue;
}
a {
  color: black;
  font-weight: bold;
  font-size: 0.9em;
}
li {
  padding: 60px 15px;

  &:hover {
    cursor: pointer;
    border-bottom: 5px solid $color-electric-blue;
  }
}
</style>
