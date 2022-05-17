<template>
  <header class="container">
    <nav>
      <div>
        <nav class="navbar">
          <div>
            <img class="navbar__logo" src="../img/svg/logo.svg" alt="logo" />
          </div>

          <ul class="menu__first" :class="isActive ? 'active' : 'inactive'">
            <li class="menu__item">
              <a href="#" class="menu__item-link">Falcon 9</a>
            </li>
            <li class="menu__item">
              <a href="#" class="menu__item-link"> Falcon Heavy </a>
            </li>
            <li class="menu__item">
              <a href="#" class="menu__item-link"> Dragon </a>
            </li>
            <li class="menu__item">
              <a href="#" class="menu__item-link"> Updates </a>
            </li>
          </ul>

          <ul class="menu__second">
            <li class="menu__item">
              <a href="#" class="menu__item-link"> About </a>
            </li>
            <li class="menu__item">
              <a href="#" class="menu__item-link"> Gallery </a>
            </li>
            <li class="menu__item">
              <a href="#" class="menu__item-link"> Shop </a>
            </li>
          </ul>

          <div
            class="burger"
            :class="isActive ? 'active' : 'inactive'"
            @click="isActive = !isActive"
          >
            <span class="bar"></span>
            <span class="bar"></span>
            <span class="bar"></span>
          </div>
        </nav>
      </div>
    </nav>
  </header>
</template>

<script setup>
import { ref } from "vue";

const isActive = ref(false);
</script>
