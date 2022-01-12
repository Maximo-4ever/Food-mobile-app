<template>
  <div class="home">
    <header class="header">
      <h1 class="title">Hi <span>Vadim!</span></h1>
      <form class="form">
        <input
          class="form__search"
          type="text"
          placeholder="Find what you want..."
        />
        <i class="bx bx-search bx-sm"></i>
      </form>
      <div class="combo">
        <div class="combo-body">
          <h3>Free combo</h3>
          <p>
            Burger + Coca-Cola <br />
            for new users
          </p>
        </div>
        <img src="" alt="" />
      </div>
    </header>
    <div class="scroll-menu">
      <div class="food-sections" v-for="(item, index) in 4" :key="index">
        <i class="bx bxs-pizza"></i>
        <h4>Pizza</h4>
      </div>
    </div>
    <main class="main">
      <h2 class="subtitle">Top Products</h2>
      <div class="top-products">
        <div class="products" v-for="(item, index) in 3" :key="index">
          <img src="@/assets/burger.png" alt="" />
          <div class="product__details">
            <h6>
              Berry Juice <br />
              <span>$7.5</span>
            </h6>
            <button>
              <i class="bx bx-plus-medical"></i>
            </button>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<style scoped>
.home {
  padding: 25px;
  margin-bottom: 69px;
}
.header {
  display: flex;
  flex-direction: column;
  row-gap: 16px;
}
.title {
  font-weight: normal;
}
.title span {
  font-weight: 600;
}
.form {
  position: relative;
}
.form__search {
  width: 100%;
  background-color: #e5d1d13d;
  border: none;
  border-radius: 15px;
  outline: none;
  padding: 14px 30px 14px 45px;
}
.bx-search {
  position: absolute;
  top: 9px;
  bottom: 0;
  left: 11px;
  color: #2c3e507a;
}
.combo {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  background-color: rgb(74, 174, 84);
  padding: 16px 21px;
  border-radius: 28px;
  margin-top: 8px;
}
.combo-body {
  color: #fff;
}
.combo-body h3 {
  font-weight: 600;
  letter-spacing: 0.7px;
}
.combo-body p {
  font-weight: 300;
  line-height: 21px;
}

.scroll-menu {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  column-gap: 10px;
  margin-top: 16px;
  overflow: auto;
}
.food-sections {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  background-color: #e5d1d13d;
  padding: 15px 25px;
  border-radius: 24px;
}
.food-sections i {
  font-size: 40px;
  color: #ff833e;
}
.food-sections h4 {
  font-weight: 400;
  font-size: 16px;
  margin-top: 6px;
}

.main {
  margin-top: 20px;
}
.subtitle {
  font-size: 22px;
  font-weight: 600;
  margin-bottom: 14px;
}
.top-products {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  overflow: auto;
  column-gap: 16px;
}
.products {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  background-color: #e5d1d13d;
  border-radius: 24px;
  padding: 25px 15px;
}
.products img {
  height: 95px;
  margin-bottom: 20px;
}
.product__details {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.product__details h6 {
  font-size: 16px;
  font-weight: 400;
  margin-right: 15px;
}
.product__details h6 span {
  font-size: 17px;
  color: #ff833e;
}
.product__details button {
  display: flex;
  padding: 10px;
  background-color: green;
  border-radius: 50%;
  outline: none;
  border: none;
}
.product__details i {
  font-size: 18px;
  color: #fff;
}
</style>
