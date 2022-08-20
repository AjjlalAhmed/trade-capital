<script setup>
// Importing things we need
import { ref } from "@vue/reactivity";

// Variables
const showMenu = ref(false);

// Functions
const toggleNavbar = () => (showMenu.value = !showMenu.value);
</script>



<template>
  <!-- Header -->
  <header class="header">
    <!-- Nav  -->
    <nav class="nav">
      <!-- Logo  -->
      <div class="logo">
        <h1>trade capital</h1>
      </div>
      <!-- Nav ul  -->
      <ul :class="{ 'nav-ul': true, hide: showMenu }">
        <!-- Item  -->
        <li class="item">
          <!-- Link  -->
          <router-link to="#" class="link">exchange crypto</router-link>
        </li>
        <!-- Item  -->
        <li class="item">
          <!-- Link  -->
          <router-link to="#" class="link">trade crypto</router-link>
        </li>
        <!-- Item  -->
        <li class="item">
          <!-- Link  -->
          <router-link to="#" class="link">buy crypto</router-link>
        </li>
        <!-- Item  -->
        <li class="item">
          <!-- Link  -->
          <router-link to="#" class="link">contact</router-link>
        </li>
        <!-- Item  -->
        <li class="item">
          <!-- Link  -->
          <router-link to="#" class="action-btn">create account</router-link>
        </li>
      </ul>
      <!-- Menu  -->
      <div @click="toggleNavbar" class="menu">
        <!-- Bars  -->
        <div class="bar"></div>
        <div class="bar"></div>
        <div class="bar"></div>
      </div>
    </nav>
  </header>
  <!-- Header -->
</template>


<style lang="scss" scoped>
// Styles
.header {
  padding: 20px;
    background: #0a0820;
  .nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1500px;
    margin: auto;
    .logo {
      h1 {
        font-family: "DynaPuff", cursive;
        font-size: 1.5rem;
        text-transform: capitalize;
        color: #f7bb00;
        letter-spacing: 1px;
      }
    }
    .nav-ul {
      display: flex;
      align-items: center;
      justify-content: center;
      margin-left: 10%;
      .item {
        list-style: none;
        padding: 20px;
        .link {
          display: inline-block;
          text-decoration: none;
          font-size: 1rem;
          letter-spacing: 1px;
          text-transform: capitalize;
          transition: 0.3s ease-in-out;
          position: relative;
          color: #fff;
          letter-spacing: 1px;
        }
        .action-btn {
          padding: 8px 20px;
          border: 1px solid #f7bb00;
          border-radius: 1px;
          text-decoration: none;
          font-size: 1rem;
          letter-spacing: 1px;
          text-transform: capitalize;
          color: #f7bb00;
          transition: 0.3s linear;
          font-weight: 700;
          &:hover {
            background: #f7bb00;
            color: #0a0820;
          }
        }

        .link:after {
          content: "";
          position: absolute;
          width: 100%;
          transform: scaleX(0);
          height: 2px;
          bottom: 0;
          left: 0;
          transform-origin: bottom right;
          transition: transform 0.25s ease-out;
          background-color: #f7bb00;
        }

        .link:hover:after {
          transform: scaleX(1);
          transform-origin: bottom left;
        }
      }
    }
    .menu {
      display: none;
      .bar {
        display: block;
        background: #f7bb00;
        width: 30px;
        height: 3px;
        margin: 5px;
      }
    }
  }
}

// Media queries
@media only screen and (max-width: 1100px) {
  .header {
    padding-bottom: 0px;
    .nav {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      .logo {
        grid-column: 1 / 3;
        grid-row: 1 / 2;
        justify-self: left;
        align-self: center;
      }
      .menu {
        display: block;
        grid-column: 3 / 4;
        grid-row: 1 / 2;
        justify-self: right;
        align-self: center;
      }
      .nav-ul {
        flex-direction: column;
        grid-column: 1 / 4;
        grid-row: 2 / 3;
        justify-self: center;
        height: 0;
        overflow: hidden;
        padding: 0;
        transition: 0.3s ease-in-out;
        width: 100%;
        margin: 10px auto;
        text-align: center;
      }
      .action-btns {
        display: none;
      }
    }
  }
  .hide {
    height: 300px !important;
    background: rgba(255, 255, 255, 0.25);
    box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
    backdrop-filter: blur(4px);
    -webkit-backdrop-filter: blur(4px);
    border-radius: 10px;
    border: 1px solid rgba(255, 255, 255, 0.18);
    .item:first-child {
      padding-top: 40px !important;
    }
    .item:last-child {
      padding-bottom: 40px !important;
    }
  }
}
</style>