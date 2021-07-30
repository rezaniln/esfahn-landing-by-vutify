<template>
  <div class="d1" @scroll="handleScroll">
    <transition name="fade">
      <div v-show="scY > 300" class="img2" id="pagetop" @click="toTop">
        <p>&#8593;</p>
      </div>
    </transition>
    <div class="img1">
      <img
        ref=""
        src="~/assets/images/5f4612fda3acf607e822f585ac7j.png"
        alt=""
      />
    </div>
    <v-row>
      <v-col>
        <p>کلیه حقوق این وبسایت متعلق به شرکت اصفهان آهن آپادانا می باشد</p>
      </v-col>
      <v-col>
        <ul>
          <li><a href="https://esfahanahan.com/"> خانه </a></li>
          <li>
            <a href="https://esfahanahan.com/landing/ussd/#andriod">
              ورژن اندروید
            </a>
          </li>
          <li>
            <a href="https://esfahanahan.com/landing/ussd/#ios"> ورژن IOS </a>
          </li>
          <li>
            <a
              href="https://esfahanahan.com/%D8%AF%D8%B1%D8%A8%D8%A7%D8%B1%D9%87-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"
            >
              درباره ما
            </a>
          </li>
          <li>
            <a
              href="https://esfahanahan.com/%D8%AA%D9%85%D8%A7%D8%B3-%D8%A8%D8%A7-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"
            >
              تماس با ما
            </a>
          </li>
        </ul>
      </v-col>
    </v-row>
  </div>
</template>



<script>
export default {
  data() {
    return {
      scTimer: 0,
      scY: 0,
    }
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll() {
      if (this.scTimer) return
      this.scTimer = setTimeout(() => {
        this.scY = window.scrollY
        clearTimeout(this.scTimer)
        this.scTimer = 0
      }, 100)
    },
    toTop() {
      window.scrollTo({
        top: 0,
        behavior: 'smooth',
      })
    },
  },
}
</script>



<style lang="scss" scoped>
.row {
  width: inherit;
}
.d1 {
  width: 100%;
  direction: rtl;
  background: linear-gradient(
    to right,
    #181156 0%,
    #50498d 42%,
    #706ba4 85%,
    #645f93 100%
  );
}
p {
  text-align: center;
  padding-top: 6px;
  color: white;
}
ul {
  width: fit-content;
  margin: 0 auto;
  display: flex;
  flex-direction: row;
  padding-top: 6px !important;
  align-items: center;

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

      &:hover {
        color: black !important;
      }
    }
  }
}
@media only screen and (max-width: 992px) {
  .row {
    flex-direction: column;
  }
  p {
    font-size: 14px;
  }
}
.img1 {
  position: fixed;
  width: 50px;
  bottom: 70px;
  z-index: 10;
  img {
    width: 70px;
    border-radius: 50% !important;
  }
}
.img2 {
  cursor: pointer;
  border-radius: 50%;
  width: 50px;
  position: fixed;
  border: 1px solid rgb(0, 0, 0);
  bottom: 150px;
  right: 10px;
  z-index: 11;
   background: #181156;
    background: linear-gradient(to right, #181156 0%,#50498d 42%,#706ba4 85%,#645f93 100%);
    p{
      font-weight: bolder;
      color: white;
    }
}
</style>
