<template>
  <footer>
    <div class="footer-top">
      <div class="wrapper">
        <div class="logo-footer">
          <img src="../assets/img/logo-light.png" alt="">
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ex asperiores fugit adipisci perspiciatis. Unde nihil, deserunt mollitia molestiae neque nam.
          </p>
        </div>
        <div class="lista-footer">
          <h2>Company</h2>
          <ul>
            <li v-for="elemento,indicatore in listaFooterSinistra" :key='indicatore'>
              <a href="">
                <i class="fas fa-chevron-right"></i>{{elemento}}
              </a>
            </li>
          
          </ul>
        </div>
        <div class="lista-footer">
          <h2>Usefull Links</h2>
          <ul>
            <li v-for="elemento,indicatore in listaFooterSinistra" :key='indicatore'>
              <a href="">
                <i class="fas fa-chevron-right"></i>{{elemento}}
                </a>
            </li>
          
          </ul>
          
        </div>
        <div class="email-footer">
          <h2>Newsletter</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ex asperiores fugit adipisci perspiciatis. Unde nihil, deserunt mollitia molestiae neque nam.
            </p>
        </div>
      </div>
    </div>
    <div class="footer-bottom wrapper">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, voluptatum consectetur? Explicabo voluptate sunt, dolorem quo aut ducimus eius necessitatibus?
    </div>
  </footer>
  
</template>

<script>
export default {
  name:'Footer',
  props:{
    listaFooterSinistra:Array,
    listaFooterDestra:Array
  }
}
</script>

<style lang='scss' scoped>
   
  footer {
    padding-top: 60px;
    padding-bottom: 60px;
    background-color: #202942;
    .footer-top{
      border-bottom: 1px solid black;
      .wrapper{
      display: flex;
      
      
        div{
        
        }
      .lista-footer{
        width: 20%;
        ul{
       
        list-style: none;
        a{
          text-decoration: none;
          color: #adb5bd;
        }
      }
      } 
      .logo-footer{
        width:30%;
        display: flex;
        flex-direction: column;
        img{
          width: 120px;
        }
        
      }
      .email-footer{
        width: 30%;
        background-color: green;
      }
    }
    }

    
  }
</style>