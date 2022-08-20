<script setup>
// Importing things we need
import landindImg from "../assets/imaegs/landing.svg";
</script>

<template>
  <!-- Landing  -->
  <div class="landing">
    <!-- Content  -->
    <div class="content">
      <!-- Left -->
      <section class="left">
        <!-- Title  -->
        <h1 class="title">limitless crypto exchange</h1>
        <!-- Text  -->
        <p class="text">
          Buy and sell 250+ cryptocurrencies with 20+ fiat currencies using bank
          transfers or your credit/debit card.
        </p>
        <!-- Button  -->
        <div class="btn">
          <!-- Action button -->
          <button class="action-btn">exchange crypto</button>
        </div>
      </section>
      <!-- Rigth  -->
      <section class="rigth">
        <!-- Imaegs  -->
        <img :src="landindImg" alt="" />
      </section>
    </div>
  </div>
  <!-- Landing  -->
</template>



<style lang="scss" scoped>
// Styles
.landing {
  min-height: 90vh;
  padding: 20px;
  .content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
    max-width: 1500px;
    margin: auto;
    margin-top: 80px;
    .left {
      .title {
        font-size: 3rem;
        text-transform: capitalize;
        color: #fff;
        letter-spacing: 1px;
      }
      .text {
        font-size: 1.2rem;
        color: #fff;
        letter-spacing: 1px;
        max-width: 500px;
        padding: 20px 0px;
        line-height: 2rem;
      }
      .btn {
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
          background: transparent;
          margin-bottom: 50px;
          cursor: pointer;
          &:hover {
            background: #f7bb00;
            color: #0a0820;
          }
        }
      }
    }
    .rigth {
      img {
        max-width: 700px;
        width: 100%;
      }
    }
  }
}

// Media queries

@media only screen and (max-width: 1346px) {
  .landing {
    .content {
      justify-content: center;
    }
  }
}
@media only screen and (max-width: 552px) {
  .landing {
    .content {
      .left {
        .title {
          text-align: center;
          font-size: 2rem;
        }
        .text {
          text-align: center;
          font-size: 1rem;
        }
        .btn {
          text-align: center;
        }
      }
    }
  }
}
</style>