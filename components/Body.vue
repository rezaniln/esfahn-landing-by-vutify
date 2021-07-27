<template>
 <v-container>
    <div>
    <v-row class="main-body-flex-container">
      <v-col
        ><section class="ussd">
          <span class="ussd-text">۳۴۰۴۵#*۶۶۵۵*</span>
        </section>
      </v-col>
      <v-col>
        <section class="text-field">
          <h2>امکانات</h2>
          <p>
            استفاده از روش پرداخت USSD به وسیله موبایل امکانات زیر را به شما
            میدهد
          </p>
        </section>
      </v-col>
      <v-col class="card-container">
        <v-row>
          <v-col
            ><v-card>
              <i class="icon-signal"></i>
              <h2>دسترسی</h2>
              <h5>ساده در هر کجا</h5>
            </v-card></v-col
          >
          <v-col
            ><v-card>
              <i class="icon-speedometer"></i>
              <h2>سرعت</h2>
              <h5>بالا برای پرداخت</h5>
            </v-card></v-col
          >
          <v-col
            ><v-card>
              <i class="icon-bars"></i>
              <h2>صرفه جویی</h2>
              <h5>در وقت و هزینه</h5>
            </v-card></v-col
          >
          <v-col
            ><v-card>
              <i class="icon-padlock"></i>
              <h2>امنیت</h2>
              <h5>بالای پرداخت اینترنتی</h5>
            </v-card></v-col
          >
        </v-row>
      </v-col>
      <v-col>
        <v-row class="about-area">
          <v-col>
            <h4>آموزش پرداخت از طریق USSD کد</h4>
            <ul class="ul-content mt-5">
              <li>فرایند پرداخت موبایلی اصفهان آهن بسیار ساده است</li>
              <li>
                <span> &#8592;</span>
                <p>ابتدا وارد صفحه شماره گیری تلفن همراه خود شوید</p>
              </li>
              <li>
                <span> &#8592; </span>
                <p>سپس کد *6655*34045# را شماره گیری نمایید.</p>
              </li>
              <li>
                <span> &#8592; </span>
                <p>پس از شماره گیری بر روی تماس کلیک کنید.</p>
              
              </li>
              <li>
                <span> &#8592; </span>
                <p
                  >یکی از دو گزینه پرداخت بیعانه و تسویه حساب را وارد نموده و بر
                  روی ارسال کلیک کنید.</p
                >
              </li>
              <li>
                <span> &#8592; </span>
                <p
                  >مبلغ مورد نظر را انتخاب یا وارد نموده و بر روی ارسال کلیک
                  کنید.</p
                >
              </li>
              <li>
                <span> &#8592; </span>
                <p
                  >لینک پرداخت اینترنتی برای شما از طریق پیامک ارسال
                  میشود.</p
                >
              </li>
              <li>
                <span> &#8592; </span>
                <p
                  >بر روی لینک داخل پیامک کلیک کنید تا وارد صفحه پرداخت
                  شوید.</p
                >
              </li>
              <li>
                <span> &#8592; </span>
                <p
                  >با تکمیل فرایند خرید اینترنتی پرداخت شما کامل شده است.
                </p>
              </li>
            </ul>
          </v-col>
          <v-col class="video-box">
            <video controls>
            <source
              src="https://esfahanahan.com/landing/ussd/assets/video/ussd.mp4"
              type="video/mp4"
            />
          </video>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </div>
 </v-container>
</template>
<style lang="scss">
.main-body-flex-container {
  flex-direction: column;
  justify-content: center;
  align-items: center;

  div {
    .ussd {
      width: fit-content;
      justify-content: center;
      margin: 0 auto;
    }
    .ussd-text {
      text-align: center;
      margin: 0 auto;
      font-size: 150px;
      color: hsl(220 46% 48% / 1);
      text-shadow: 1px 1px 1px hsl(220deg 46% 38%),
        1px 2px 1px hsl(220deg 46% 38%), 1px 3px 1px hsl(220deg 46% 38%),
        1px 4px 1px hsl(220deg 46% 38%), 1px 5px 1px hsl(220deg 46% 38%),
        1px 6px 1px hsl(220deg 46% 38%), 1px 7px 1px hsl(220deg 46% 38%),
        1px 8px 1px hsl(220deg 46% 38%), 1px 9px 1px hsl(220deg 46% 38%),
        1px 10px 1px hsl(220deg 46% 38%), 1px 18px 6px rgb(60 60 60 / 30%),
        1px 22px 10px rgb(60 60 60 / 10%), 1px 25px 35px rgb(60 60 60 / 10%),
        1px 30px 60px rgb(60 60 60 / 30%);
    }
    .text-field {
      text-align: center;
    }
  }
  .card-container {
    margin-top: 20px;
    padding: 0px 250px ;
    div {
      div {
        box-shadow: none !important;
        div {
          text-align: center;
          padding: 20px 0;
          border-radius: 10px;
          box-shadow: 0px 30px 60px -20px rgb(222 222 222) !important;

          i {
            color: #4268b3;
            margin: 10px;
            font-size: 50px;
            font-weight: bold;
          }
        }
      }
    }
  }
  .about-area{
    padding: 50px 250px;
    div{
      padding: 0;
      h4{
        
        
      }
      ul{
        margin-top: 0!important;
        line-height: 1.5rem;
       display: unset;
        li{ padding: 0;
          display: flex;
            p{
              display: inline-block;
              margin-right: 15px;
              font-size: 15px;
              
            }
        }
      }
    }
    video{
      max-width: inherit;
    }
  }
}
@media (min-width:768px) and (max-width:991px){
  .ussd{
    span{
      font-size:80px !important;
     
    }
}
.card-container{
    padding: unset!important;;
    .row{
      display: block;
      width: 100% !important;
    }
  }
  .about-area{
    flex-direction: column-reverse;
    padding: unset !important;
  }
  .row{
    margin: unset;
  }
}
@media  only screen and (max-width:767px){
   .ussd-text{
     font-size: 40px !important;
     
   } 
  .data-box{
  flex-direction: column-reverse;
  align-items: center;
  justify-content: center;
    .video {
     max-width: 100%;
    }
    .ul-content{
      max-width: 100%;
    }
  }
  .card-container{
    padding: unset!important;;
    .row{
      display: block;
      width: 100% !important;
    }
  }
  .about-area{
    flex-direction: column-reverse;
    padding: unset !important;
  }
  .row{
    margin: unset;
  }
  }
  

</style>
