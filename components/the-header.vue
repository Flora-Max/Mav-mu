<script>
    import { ref } from 'vue';
export default {
  setup() {
    let showMenu = ref(false);
    const toggleNav = () => (showMenu.value = !showMenu.value);
    return { showMenu, toggleNav };
  },
};
</script>

<template>

<!-- 
    <nav class="relative w-auto flex justify-between items-center mx-10 mt-10">

        <div class="flex items-center">
            <img class="w-20" src="../assets/img/logo.png" alt="">
            <span class="items-center">Maëva Muësser</span>
        </div>

        <button @click="isOpen" class="w-4 md:hidden cursor-pointer">
            <img src="../assets/img/menu.png" alt="">
        </button>

        <ul class="hidden md:flex">
            <li class="mx-5">Instagram</li>
            <li class="mx-5">Facebook</li>
            <li class="mx-5">Etsy</li>
        </ul>
    </nav> -->

    <div>
    <nav
      class="
        container
        px-6
        py-8
        mx-auto
        md:flex md:justify-between md:items-center
      "
    >
      <div class="flex items-center justify-between">
        <router-link
          to="/"
          class="
            text-xl
            font-bold
            text-gray-100
            md:text-2xl
            hover:text-indigo-400
          "
          >
          <img class="w-1/4" src="../assets/img/mavName.jpeg" alt="">
        </router-link>
        <!-- Mobile menu button -->
        <div @click="toggleNav" class="flex md:hidden">
          <button
            type="button"
            class="
              text-gray-100
              hover:text-gray-400
              focus:outline-none focus:text-gray-400
            "
          >
            <img class="w-8 h-8 fill-current" src="../assets/img/menu.png" alt="">
          </button>
        </div>
      </div>

      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul
        :class="showMenu ? 'flex' : 'hidden'"
        class="
          flex-col
          mt-10
          space-y-8
          items-center
          text-xl
          md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0
        "
      >
        <li>
            Facebook
            <img class="w-5" src="../assets/img/logo-facebook.png" alt="">
        </li>
        <li>
            Etsy
            <img class="w-5" src="../assets/img/etsy.png" alt="">
        </li>
        <li>
            Instagram
            <img class="w-5" src="../assets/img/instagram.png" alt="">
        </li>
      </ul>
    </nav>
  </div>

    <section id="mobile-menu" class="absolute w-full flex flex-col justify-content-center">
        <button class="self-end"></button>
    </section>
</template>