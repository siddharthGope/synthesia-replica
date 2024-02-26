<template>
  <div class="d-flex justify-space-around align-center appbar-wrap">
    <div class="logowrap">
      <img class="logo" src="/images/synthesia logo.svg" />
    </div>
    <div class="d-flex justify-space-around align-center navigation-wrap">
      <v-menu
        v-for="(item, i) in items"
        :key="i"
        transition="slide-y-transition"
        open-on-hover=""
      >
        <template v-slot:activator="{ props }">
          <div class="titles nav-margin-left" v-bind="props">
            {{ item.title }}
          </div>
        </template>
        <v-list class="navlists">
          <v-list-item
            class="navlistitem"
            v-for="(other, j) in item.others"
            :key="j"
          >
            <template v-slot:prepend>
              <v-icon class="navbaricon" :icon="other.icon"></v-icon>
            </template>
            <v-list-item-title>{{ other.productTitle }}</v-list-item-title>
            <v-list-item-subtitle>{{ other.desc }}</v-list-item-subtitle>
          </v-list-item>
        </v-list>
      </v-menu>
    </div>
    <div class="d-flex justify-space-around align-center nav-buttons-wrap">
      <div class="login-btn">Log in</div>
      <div class="blue-button nav-margin-left">Create Account</div>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    items: [
      {
        title: "Features",
        others: [
          {
            productTitle: "All features",
            desc: "See all features",
            icon: "mdi-clock",
          },
          {
            productTitle: "AI avatars",
            desc: "160+ diverse AI avatars",
            icon: "mdi-account",
          },
        ],
      },
      {
        title: "Use cases",
        others: [
          {
            productTitle: "All features",
            desc: "See all features",
            icon: "mdi-clock",
          },
          {
            productTitle: "AI avatars",
            desc: "160+ diverse AI avatars",
            icon: "mdi-account",
          },
        ],
      },
      {
        title: "Pricing",
        others: [
          {
            productTitle: "All features",
            desc: "See all features",
            icon: "mdi-clock",
          },
          {
            productTitle: "AI avatars",
            desc: "160+ diverse AI avatars",
            icon: "mdi-account",
          },
        ],
      },
      {
        title: "Resources",
        others: [
          {
            productTitle: "All features",
            desc: "See all features",
            icon: "mdi-clock",
          },
          {
            productTitle: "AI avatars",
            desc: "160+ diverse AI avatars",
            icon: "mdi-account",
          },
        ],
      },
      {
        title: "Company",
        others: [
          {
            productTitle: "All features",
            desc: "See all features",
            icon: "mdi-clock",
          },
          {
            productTitle: "AI avatars",
            desc: "160+ diverse AI avatars",
            icon: "mdi-account",
          },
        ],
      },
    ],
  }),
};
</script>

<style scoped>
.appbar-wrap {
  --light-gray-color: #f5f7fe;
  --grey-darkest: #2c374f;
  --synthesia-blue-main: #084df2;
  font-family: "Poppins", sans-serif;
  border-bottom: 1px solid #e9ecf6;
  transition: background-color 0.5s ease !important;
  padding: 1rem 0;
}
.logo {
  height: 30px;
}
.titles {
  color: var(--grey-darkest);
  margin-right: 1rem;
}
.titles:hover {
  color: #084df2;
}
.navlists {
  padding: 1rem;
  border-radius: 0.75rem !important;
}
.navlistitem {
  padding: 0.5rem !important;
  margin: 0.5rem 0;
}

.navlistitem:hover {
  background-color: #f5f7fe;
  border-radius: 0.75rem;
}
.navbaricon {
  border-radius: 50%;
  background-color: #f5f7fe;
  width: 2.5rem;
  height: 2.5rem;
}
.navlistitem:hover .navbaricon {
  background-color: #fff;
  width: 2.5rem;
  height: 2.5rem;
  border-radius: 50%;
}
.nav-margin-left {
  margin-left: 20px;
}
.login-btn:hover {
  color: #084df2;
}
</style>
