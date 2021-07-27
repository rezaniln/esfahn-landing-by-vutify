<template>
 <div class="d1">
   <v-row>
     <v-col>
        <p>
                کلیه حقوق این وبسایت متعلق به شرکت اصفهان آهن آپادانا می باشد
            </p>
     </v-col>
     <v-col>
        <ul>
            <li><a href="#"> خانه </a></li>
            <li><a href="#"> امکانات </a></li>
            <li><a href="#"> آموزش استفاده </a></li>
            <li><a href="#"> درباره ما </a></li>
            <li><a href="#"> تماس با ما </a></li>
          </ul>
     </v-col>
   </v-row>
 </div>
</template>

<style lang="scss" scoped>
.row{
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
p{
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
  .row{
    flex-direction: column;
  }
  p{
    font-size: 14px;
  }
}



</style>
