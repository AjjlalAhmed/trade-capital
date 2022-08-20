<script setup>
// Importing things we need
</script>

<template>
  <!-- Buy crypto   -->
  <div class="buy-crypto">
    <!-- Content  -->
    <div class="content">
      <!-- Top bar  -->
      <div class="top-bar">
        <!-- Title  -->
        <h1 class="title">buy cryptocurrency with your credit card</h1>
        <p class="text">
          become a crypto owner in minutes using your debit or credit card
        </p>
      </div>
      <!-- Form  -->
      <form class="form">
        <!-- Form control  -->
        <div class="form-control">
          <!-- Label  -->
          <label>i want to spend</label>
          <!-- Field wrapper  -->
          <div class="field-wrapper">
            <!-- Input  -->
            <input type="number" placeholder="50" />
            <!-- Select  -->
            <select>
              <option value="usd">usd</option>
              <option value="pkr">kr</option>
            </select>
          </div>
        </div>
        <!-- Form control  -->
        <div class="form-control">
          <!-- Label  -->
          <label>i want to buy</label>
          <!-- Field wrapper  -->
          <div class="field-wrapper">
            <!-- Select  -->
            <select class="select">
              <option value="btc">btc</option>
              <option value="etc">etc</option>
            </select>
          </div>
        </div>
        <!-- Form control  -->
        <div class="form-control">
          <button class="submit-btn">buy crypto</button>
        </div>
      </form>
    </div>
    <!-- Content  -->
  </div>
  <!-- Buy crypto  -->
</template>

<style lang="scss" scoped>
// Styles
.buy-crypto {
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
      .text {
        font-size: 1rem;
        color: #0a0820;
        letter-spacing: 1px;
        padding: 10px 0px;
        line-height: 2rem;
        text-align: center;
      }
    }
    .form {
      border-radius: 5px;
      background: #fff;
      padding: 30px 20px;
      padding-bottom: 40px;
      display: flex;
      align-items: center;
      justify-content: space-evenly;
      gap: 20px;
      box-shadow: rgba(0, 0, 0, 0.1) 0px 4px 12px;
      .form-control {
        label {
          display: block;
          font-size: 1rem;
          text-transform: capitalize;
          color: #555;
          padding-bottom: 5px;
        }
        .field-wrapper {
          border: 1px solid #5555;
          padding: 10px;
          border-radius: 5px;
          input {
            width: 400px;
            padding: 5px;
            border: 0px;
            font-size: 1.2rem;
          }
          select {
            padding: 5px;
            border: 0px;
            font-size: 1.2rem;
            text-transform: uppercase;
          }
          .select {
            min-width: 70px;
          }
        }
        .submit-btn {
          padding: 8px 20px;
          border: 1px solid #f7bb00;
          border-radius: 1px;
          text-decoration: none;
          font-size: 1rem;
          letter-spacing: 1px;
          text-transform: capitalize;
          transition: 0.3s linear;
          font-weight: 700;
          background: transparent;
          background: #f7bb00;
          color: #0a0820;
          cursor: pointer;
          margin-top: 25px;
          &:hover {
            box-shadow: rgba(17, 12, 46, 0.15) 0px 48px 100px 0px;
          }
        }
      }
    }
  }
}

// Media queries

@media only screen and (max-width: 830px) {
  .buy-crypto {
    .content {
      .top-bar {
        .title {
          font-size: 2rem;
        }
      }
      .form {
        flex-direction: column;
        .form-control {
          width: 100%;
          .field-wrapper {
            display: flex;
            width: 100%;
            input {
              width: 80%;
            }
            .select {
              min-width: 100%;
            }
          }
        }
      }
    }
  }
}
</style>

