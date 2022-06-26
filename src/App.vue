<script>
import { RouterLink, RouterView } from "vue-router";
export default {
  data() {
    return {
      listMenu: [
        {
          title: "Home",
          link: "/",
        },
        {
          title: "Todo App",
          link: "/todo",
        },
        {
          title: "Pokemon Picker",
          link: "/pokemon",
        },
      ],
    };
  },
};
</script>
<template>
  <div class="max-w-3xl my-10 mx-auto">
    <nav class="flex items-center gap-3 justify-center mb-5">
      <RouterLink
        v-for="(menu, i) in listMenu"
        :key="i"
        :to="menu.link"
        :class="[menu.link === $route.path ? 'font-bold' : '', 'text-2xl']"
      >
        {{ menu.title }}
      </RouterLink>
    </nav>
    <RouterView />
  </div>
</template>
