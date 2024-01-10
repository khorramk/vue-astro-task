<template>
  <nav class="navigation" role="navigation" aria-label="Main Navigation">
    <a to="/" class="navigation__logo">
        <img src="../assets/img/logo.png" sizes="200px xs:200px sm:400px lg:640px" />
    </a>

    <a
      class="navigation__toggle"
      id="menu-toggle"
      role="button"
      aria-expanded="false"
      aria-controls="menu"
      href="#menu"
    >
      <svg
        class="hamburger-icon"
        viewBox="0 0 100 110"
        fill="#333"
        xmlns="http://www.w3.org/2000/svg"
      >
        <rect class="bar bar1" width="100" height="4" transform="translate(0 0)" />
        <rect
          class="bar bar2"
          width="100"
          height="4"
          transform="translate(0 45)"
        />
        <rect
          class="bar bar3"
          width="100"
          height="4"
          transform="translate(0 95)"
        />
      </svg>
    </a>

    <ul role="menubar" id="menu" class="navigation__list">
      <li v-for="(menu, i) in menuItems" :key="i" role="menuitem" class="navigation__item">
        <a class="navigation__link"  :to="menu.link">{{ menu.name }}</a>
      </li>
      <a href="#" class="clear-modal">&times;</a>
    </ul>
  </nav>
</template>

<script lang="ts" setup>
import { computed } from 'vue';


 const menuItems = [
    {
      name: 'Home',
      link: '/home'
    },
    {
      name: 'About',
      link: '/about'
    }
 ]

</script>

