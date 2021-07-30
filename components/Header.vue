<template>
  <v-container fluid class="pa-0 d-container">
    <div class="b1">
      <v-row class="nav-container ma-0">
        <v-col>
          <img
            class="logo-svg"
            src="~assets/images/logo-full.svg"
            width="300px"
          />
        </v-col>
        <v-col>
          <div class="dropdown-1">
            <v-menu>
              <template #activator="{ on, attrs }">
                <v-btn color="black" v-bind="attrs" v-on="on">
                  <i style="color:white" class="icon-list"></i>
                </v-btn>
              </template>
              <v-list>
                <v-list-item href="https://esfahanahan.com/"> خانه </v-list-item>
                <v-list-item href="#features"> امکانات </v-list-item>
                <v-list-item href="#guid-use"> آموزش استفاده </v-list-item>
                <v-list-item href="https://esfahanahan.com/%D8%AF%D8%B1%D8%A8%D8%A7%D8%B1%D9%87-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"> درباره ما </v-list-item>
                <v-list-item href="https://esfahanahan.com/%D8%AA%D9%85%D8%A7%D8%B3-%D8%A8%D8%A7-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"> تماس با ما </v-list-item>
              </v-list>
            </v-menu>
          </div>
          <div class="nav-item">
            <ul>
              <li><a href="https://esfahanahan.com/"> خانه </a></li>
              <li><a href="#features"> امکانات </a></li>
              <li><a href="#guid-use"> آموزش استفاده </a></li>
              <li><a href="https://esfahanahan.com/%D8%AF%D8%B1%D8%A8%D8%A7%D8%B1%D9%87-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"> درباره ما </a></li>
              <li><a href="https://esfahanahan.com/%D8%AA%D9%85%D8%A7%D8%B3-%D8%A8%D8%A7-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"> تماس با ما </a></li>
            </ul>
          </div>
        </v-col>
      </v-row>
      <v-row class="text-mobile">
        <v-col class="mobile-png" cols="6">
          <img src="~assets/images/banner.png" alt="" />
        </v-col>
        <v-col class="text-container" cols="6">
          <div class="text-box">
            <h1>معرفی امکان پرداخت سریع موبایلی</h1>
            <p>
              مجموعه اصفهان آهن به منظور سهولت در پرداخت صورت حساب مشتریان خود
              اقدام به راه اندازی سیستم پرداخت موبایلی از طریق کد USSD نموده است
              . در ادامه به معرفی مزایای این روش و آموزش استفاده از آن
              میپردازیم.
            </p>
            <button ><a href="#features">امکانات</a></button>
            <button><a href="#guid-use">آموزش استفاده</a></button>
          </div>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script>
export default {
  data() {
    
    }
  
}
</script>

<style lang="scss" scoped>
.dropdown-1{
  display: none;
}
.row {
  width: inherit;
}
.b1 {
  margin: 0;
  padding: 12px 0 170px 0;
  position: relative;
  z-index: 1;
  overflow: hidden;
  background: linear-gradient(to top right, #181156 40%, #fff 100%);
  &:before {
    content: '';
    top: -35px;
    left: 0;
    right: -35px;
    bottom: 0;
    background-image: url(~assets/images/header-shape.png);
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    z-index: -1;
    position: absolute;

    width: inherit;
    height: inherit;
  }
}

ul {
  float: left;
  display: flex;
  flex-direction: row;
  padding-left: 0px !important;
  align-items: center;
  padding-top: 20px;

  li {
    vertical-align: baseline;
    list-style-type: none;
    padding-right: 15px;
    &:first-child {
      a {
        color: black !important;
      }
    }

    a {
      color: white !important;
      text-decoration: none;
      font-weight: bold;
      &:hover {
        color: black !important;
      }
    }
  }
}
.nav-container {
  padding: 0px 150px;
}
.text-mobile {
  justify-content: center;
  align-items: center;
  .mobile-png {
    width: fit-content;
    img {
      float: left;
    }
  }
  .text-box {
    h1,
    p {
      color: white;
      padding-left: 200px;
    }
  }
}
button {
  font-weight: bold;
  color: white;
  margin: 20px 0 0 8px;
  padding: 5px 20px;
  background-color: rgba(0, 0, 0, 0);
  border: 1px solid white;
  border-radius: 20px;
  box-shadow: none !important;
  &:hover {
    background-color: white;
    color: black;
  }
    a{
      text-decoration: none;
      color: white;
    }
}
@media only screen and (max-width: 992px) {
  .text-mobile {
    flex-direction: column;
    justify-content: center !important;
    align-items: center !important;
  }
  .text-box {
    h1,
    p {
      padding: 0 !important;
    }
  }
  .nav-item {
    display: none;
  }
  .dropdown-1 {
    display: block;
    float: left;

    button {
      padding: 0 5px;
      background-color: black;
      border-radius: 5px;
      height: 28px;
      &:after {
        border: none;
      }
      svg {
        display: block;
        color: white !important;
        margin: 0 auto;
        font-size: 180%;
      }
    }
  }
  .logo-svg {
    width: 200px;
  }
  .nav-container {
    padding: 0 !important;
  }
  .v-list {
    background: linear-gradient(
      to right,
      #609eea 0%,
      #47b7e4 42%,
      #21dfdb 85%,
      #1ae7da 100%
    );
    .v-list-item {
      color: white !important;
      cursor: pointer;
      &:first-child{
      color:black !important;
    }
    }
    
  }
  .text-container{
    max-width: 100% !important;
      .text-box{
        width: inherit;
      }
  }
  .mobile-png{
    max-width: 100% !important;
  }
}
</style>
