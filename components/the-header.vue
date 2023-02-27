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
  <div>
    <nav
      class="
        container
        px-6
        mx-auto
        lg:flex lg:justify-between lg:items-center
      "
    >
      <div class="flex items-center justify-between">
        <router-link
          to="/"
          class="
            md:text-2xl"
          >
          <img class="w-96" src="../assets/img/mavName.jpeg" alt="">
        </router-link>

        <!-- Mobile menu button -->
        <div @click="toggleNav" class="flex lg:hidden">
          <button
            type="button"
            class="
              text-gray-100
              hover:text-gray-400
              focus:outline-none focus:text-gray-400
            "
          >
            <img class="w-8 mb-12 fill-current" src="../assets/icons/menu.png" alt="">
          </button>
        </div>
      </div>

      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul
        :class="showMenu ? 'flex' : 'hidden'"
        class="
          flex-col
          space-y-6
          items-center
          text-xl
          lg:flex lg:space-y-0 lg:flex-row lg:items-center lg:space-x-10 lg:mt-0
        "
      >
       
        <nuxt-link to="andMore" class="lg:hidden font-thin hover:font-normal">
          Mais aussi 
        </nuxt-link>
        <nuxt-link to="about" class="lg:hidden font-thin hover:font-normal">
          A propos
        </nuxt-link>
        <nuxt-link to="contact" class="lg:hidden font-thin hover:font-normal">
          Contact
        </nuxt-link>
        <div :class="showMenu ? 'flex' : 'hidden'"
              class="flex space-x-6">    
          <a href="https://instagram.com/maevamue?igshid=YmMyMTA2M2Y=">
            <img class="w-7" src="../assets/icons/instagram.png" alt="">
          </a>
          <a href="https://etsy.com/fr/shop/MaevaMu">
            <img class="w-7" src="../assets/icons/etsy.png" alt="">
          </a>
        </div>
      </ul>
    </nav>
  </div>

    
</template>