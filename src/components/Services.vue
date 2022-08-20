<script setup>
// Importing things we need
import growthImg from "../assets/imaegs/se-gr.svg";
import transparentImg from "../assets/imaegs/se-tr.svg";
import transactionImg from "../assets/imaegs/se-tran.svg";
import supportImg from "../assets/imaegs/se-su.svg";

// Variables
const data = [
  {
    id: 1,
    src: growthImg,
    title: "best rate",
    text: "The financial products offered by the company carry a high level of risk and can result in the loss of all your funds. You should never invest money that you cannot afford to lose.",
  },
  {
    id: 2,
    src: transparentImg,
    title: "transparent free",
    text: "The financial products offered by the company carry a high level of risk and can result in the loss of all your funds. You should never invest money that you cannot afford to lose.",
  },
  {
    id: 3,
    src: transactionImg,
    title: "fast transactions",
    text: "The financial products offered by the company carry a high level of risk and can result in the loss of all your funds. You should never invest money that you cannot afford to lose.",
  },
  {
    id: 4,
    src: supportImg,
    title: "24/7 support",
    text: "The financial products offered by the company carry a high level of risk and can result in the loss of all your funds. You should never invest money that you cannot afford to lose.",
  },
];
</script>

<template>
  <!-- Buy crypto   -->
  <div class="services">
    <!-- Content  -->
    <div class="content">
      <!-- Top bar  -->
      <div class="top-bar">
        <!-- Title  -->
        <h1 class="title">the services you deserve</h1>
      </div>
      <!-- Cards  -->
      <div class="cards">
        <div v-for="item in data" :key="item.id" class="card">
          <!-- image  -->
          <div class="img">
            <img :src="item.src" alt="" />
          </div>
          <!-- Title  -->
          <h2 class="title">{{ item.title }}</h2>
          <!-- Text  -->
          <p class="text">{{ item.text }}</p>
        </div>
      </div>
    </div>
    <!-- Content  -->
  </div>
  <!-- Buy crypto  -->
</template>

<style lang="scss" scoped>
// Styles
.services {
  background: #f6f7fb;
  padding: 150px 10px;
  .content {
    max-width: 1200px;
    margin: auto;
    .top-bar {
      .title {
        font-size: 3rem;
        text-transform: capitalize;
        color: #0a0820;
        letter-spacing: 1px;
        text-align: center;
      }
    }
    .cards {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 100px;
      .card {
        max-width: 280px;
        padding:30px 10px;
        box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
        border-radius: 5px;
        .img {
          text-align: center;
          img {
            width: 50px;
            height: 50px;
          }
        }
        .title{
          font-size: 1.5rem;
          text-transform: capitalize;
          padding: 10px 0px;
          font-weight: 400;
          text-align: center;
        }
        .text{
          text-align: left;
          font-size: 1rem;
          letter-spacing: 1px;
          line-height: 1.6rem;
          text-align: center;
        }
      }
    }
  }
}

// Media queries

@media only screen and (max-width: 830px) {
  .services {
    .content {
      .top-bar {
        .title {
          font-size: 2rem;
        }
      }
    }
  }
}
</style>

