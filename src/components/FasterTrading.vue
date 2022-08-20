<script setup>
// Importing things we need
import fasterTradingImg from "../assets/imaegs/fs-t.svg";
</script>

<template>
  <!-- Landing  -->
  <div class="faster-trading">
    <!-- Content  -->
    <div class="content">
      <!-- Left  -->
      <section class="left">
        <!-- Title  -->
        <h1 class="title">safer and faster trading</h1>
        <!-- Text  -->
        <p class="text">
          The financial products offered by the company carry a high level of
          risk and can result in the loss of all your funds. You should never
          invest money that you cannot afford to lose.
        </p>
        <!-- Button  -->
        <div class="btn">
          <button class="action-btn">trade crypto</button>
        </div>
      </section>
      <!-- Rigth  -->
      <section class="rigth">
        <!-- Imaegs  -->
        <img :src="fasterTradingImg" alt="" />
      </section>
    </div>
    <!-- Content  -->
  </div>
  <!-- Landing  -->
</template>



<style lang="scss" scoped>
// Styles
.faster-trading {
  background: #fff;
  padding: 10px;
  clip-path: polygon(0 19%, 100% 0%, 100% 100%, 0% 100%);
  .content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
    max-width: 1500px;
    margin: auto;
    padding: 150px 0px;
      min-height: 100vh;
    .left {
      .title {
        font-size: 3rem;
        text-transform: capitalize;
        color: #0a0820;
        letter-spacing: 1px;
      }
      .text {
        font-size: 1.2rem;
        color: #0a0820;
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
          background: #f7bb00;
          color: #0a0820;
          cursor: pointer;
          &:hover {
            box-shadow: rgba(17, 12, 46, 0.15) 0px 48px 100px 0px;
          }
        }
      }
    }
    .rigth {
      img {
        width: 100%;
        max-width: 700px;
        border-radius: 5px;
        overflow: hidden;
      }
    }
  }
}

// Media queries

@media only screen and (max-width: 1346px) {
  .faster-trading {
    .content {
      justify-content: center;
    }
  }
}
@media only screen and (max-width: 552px) {
  .faster-trading {
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