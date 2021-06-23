<template>
<footer>
  <!-- footer top -->
  <div class="footer-top">
    <!-- contenitore rientrato -->
    <div class="wrapper">
      <!-- footer top sinistra -->
      <div class="logo-footer">
        <img :src="require('../assets/img/' + logoFooter)" alt="">
      
        <p>
          Start working with Landrick that can provide everything you need to generate awareness, drive traffic, connect.
        </p>
        <div class="social">
          <i class="uil uil-facebook-f"></i>
          <i class="uil uil-instagram"></i>
          <i class="uil uil-twitter-alt"></i>
          <i class="uil uil-linkedin-alt"></i>
        </div>
        
      </div>
      <!-- footer top sinistra -->

      <!-- lista centrale footer 1 -->
      <div class="lista-footer">
        <h2>
          Company
        </h2>
        <ul>
          <li v-for="elemento,indicatore in listaFooterSinistra" :key='indicatore'>
            <a href="" >
              <i class="fas fa-chevron-right"></i>{{elemento}}
            </a>
          </li>
        
        </ul>
      </div>
      <!-- lista centrale footer 1 -->

      <!-- lista centrale footer 2 -->
      <div class="lista-footer">
        <h2>
          Usefull Links
        </h2>
        <ul>
          <li v-for="elemento,indicatore in listaFooterDestra" :key='indicatore'>
            <a href="" >
              <i class="fas fa-chevron-right"></i>{{elemento}}
              </a>
          </li>
        </ul>
      </div>
      <!-- /lista centrale footer 2 -->

      <!-- div destra footer top -->
      <div class="email-footer">
        <h2>Newsletter</h2>
          <p>
            Sign up and receive the lates tips via email.
          </p>
          <div class="scrivi-email">
            <span> Write your email  </span> 
            <span class="color-red">*</span>
            <input type="text" class="input-email" placeholder="  Your email :">
            <button class="bottone bottone-background" >Subscribe</button>
          </div>
      </div>
      <!-- /div destra footer top -->
    </div>
    <!-- /contenitore rientrato -->
  </div>
  <!-- footer top -->

  <!-- footer bottom -->
  <div class="footer-bottom wrapper">

    <div class="footer-bottom-sinistra">
      &copy; 2020 Landrick. Design with <span class="color-red"> &#10084; </span> by Shreethemes.
    </div>

    <div class="footer-bottom-destra">
      <img src="../assets/img/american-ex.png" alt="">
      <img src="../assets/img/discover.png" alt="">
      <img src="../assets/img/master-card.png" alt="">
      <img src="../assets/img/paypal.png" alt="">
      <img src="../assets/img/visa.png" alt="">
    </div>
    
  </div>
  <!-- /footer bottom -->

  <!-- freccia che riporta a inizio pagina -->
  <div class="hook-inizio-pagina">
    <a href="" @click.prevent="inizioPagina"><i class="uil uil-arrow-up"></i> </a> 
  </div>
  <!-- /freccia che riporta a inizio pagina -->
</footer>
</template>

<script>
export default {
  name:'Footer',
  props:{
    listaFooterSinistra:Array,
    listaFooterDestra:Array,
    logoFooter:String,
  },
  methods:{
    inizioPagina() {
      window.scrollTo(0,0);
    }
  }
}
</script>

<style lang='scss' scoped>
.color-red {
  color: red;
}

footer {
  position: relative;
  padding-top: 60px;
  padding-bottom: 60px;
  background-color: #202942;

  .footer-top {
    padding-bottom: 50px;
    border-bottom: 1px solid #273251;

    .wrapper {
      display: flex;

      h2 {
      font-weight: 500;
      margin-bottom: 20px;
      font-size: 20px;
      color: white;
      }
      p{
        color: #a4acb5;
      }

      img {
        margin: 2px 0px 30px 0px;
        width: 120px;
      }
      
      .logo-footer {
        margin-right: 20px;
        width:30%;
        padding-right: 40px;
        display: flex;
        flex-direction: column;
        p {
          line-height: 23px;
          font-weight: 600;
          font-size: 15px;
        }
        .social {
          cursor: pointer;
          margin-top: 30px;
          font-size: 20px;
          color: #a4acb5;

          i {
            border-radius: 5px;
            padding: 2px 8px;
            margin-right: 10px;
            border: 1px solid #a4acb5;

            &:hover {
              color: #202942;
              background-color: #a4acb5;
            }
          }
        } 
      }
      .lista-footer {
        width: 20%;
        
        ul {
          list-style: none;

          li {
            font-size: 15px;
            font-weight: 600;
            margin: 15px 15px 15px 0px;

            i {
              font-size: 10px;
              margin-right: 10px;
            }
          }
          a {
            text-decoration: none;
            color: #a4acb5;
            
            &:hover {
              color: #dbdeeb;
            }
          }
        }
      } 
      
      .email-footer {
        margin-left: 20px;
        width: 22%;

        .scrivi-email {
          margin-top: 20px;
          font-weight: 700;
          color: #a4acb5;

            .bottone {
              width: 100%;
              margin: 20px 0px 20px 0px;
              font-family: 'Nunito', sans-serif;
              border: none;
              border-radius: 5px;
              padding: 10px 20px;
              font-size: 15px;
              font-weight: 700;
              cursor: pointer;
            }
            .bottone-background {
              box-shadow: 0px 0px #4b5fa0,  0 3px px #334a96;
              background-color: #222e51;
              color: #2f55d4;
              
              &:hover {
                box-shadow: 0px 0px;
                color: white;
                background-color: #2f55d4;
              }
            }
        }
        .input-email {
          margin-top: 20px;
          border: none;
          border-radius: 5px;
          width: 100%;
          padding: 15px 45px;
          background-image: url('../assets/img/envelope.svg');
          background-size: 20px 20px;
          background-position: 10px center;
          background-repeat: no-repeat;
          background-color: #27314f;
          color:#a4acb5;

          &::placeholder {
            color: #a4acb5;
          }
          
          &:focus {  
            outline: none;
          }
        }        
      }
    }
  }
  .footer-bottom {
    position: relative;
    display: flex;
    align-items: center;
    margin-top: 40px;
    
    .footer-bottom-sinistra {
      width: 50%;
      color: #a4acb5;
    }

    .footer-bottom-destra {
      width: 46%;
      text-align:right;
      
      img {
        cursor: pointer;
        margin-left: 8px;
        width: 35px;
      }
    }

    
  }

  .hook-inizio-pagina {
    position: absolute;
    right: 30px;
    bottom: 59px;
    padding: 4px 8px;
    border-radius: 5px;
    transition: 5s;
    background-color: #2b48aa;

    i {
      font-size: 20px;
      color: white;
    }
  }  
}
</style>