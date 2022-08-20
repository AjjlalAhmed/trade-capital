<script setup>
// Importing things we need
</script>

<template>
  <!-- Container  -->
  <footer class="footer">
    <!-- Content  -->
    <div class="content">
      <!-- Main  -->
      <div class="main">
        <section class="left">
          <h1 class="logo">trade capital</h1>
          <h3 class="tag-line">
            trade capital : bitcoin & cryptocurrency trading platform
          </h3>
        </section>
        <section class="rigth">
          <ul>
            <li class="title">links</li>
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
          </ul>
          <ul>
            <li class="title">contact</li>
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
          </ul>
          <ul>
            <li class="title">legal</li>
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
          </ul>
        </section>
      </div>
      <!-- Bottom bar -->
      <div class="bottom-bar">
        <p>copyrigths 2022 trade cpital. all rigth reserved</p>
      </div>
    </div>
    <!-- Content  -->
  </footer>
  <!-- Container  -->
</template>

<style lang="scss">
// Styles
.footer {
  padding: 100px 0px;
  padding-bottom: 0px;
  background: #0a0820;
  .content {
    .main {
      display: flex;
      justify-content: space-around;
      align-items: flex-start;
      flex-wrap: wrap;
      max-width: 1500px;
      gap: 30px;
      margin: auto;
      padding: 0px 10px;
      .left {
        .logo {
          font-family: "DynaPuff", cursive;
          font-size: 1.5rem;
          text-transform: capitalize;
          color: #f7bb00;
          letter-spacing: 1px;
        }
        .tag-line {
          color: rgb(175, 173, 173);
          font-weight: 400;
          text-transform: capitalize;
          font-size: 0.9rem;
          letter-spacing: 1px;
          padding: 10px 0px;
          max-width: 250px;
        }
      }
      .rigth {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 50px;
        ul {
          list-style: none;
          .title {
            font-size: 1rem;
            text-transform: uppercase;
            font-weight: 700;
            color: #fff;
            padding-bottom: 20px;
          }
          .item {
            padding: 5px 0px;
            a {
              color: rgb(175, 173, 173);
              font-weight: 400;
              text-transform: capitalize;
              font-size: 0.9rem;
              text-decoration: none;
            }
          }
        }
      }
    }
    .bottom-bar {
      margin-top: 50px;
      background: #f7bb00;
      padding: 20px 0px;
      p{
        color: #0a0820;
        font-size: 1.3rem;
        text-transform: capitalize;
        text-align: center;
        font-weight: 700;
      }
    }
  }
}
</style>

