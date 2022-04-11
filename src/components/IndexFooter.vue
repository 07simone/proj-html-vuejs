<template>
  <div>
                                                      
    <!-- footertop -->
<div class="footer-top mt-5">
      <div class="container">
        <div class="row ">
          <div class=" about col-3 mt-5">
            <ul>
                <li v-for="(element,index) in about" :key=index>
                  <h3>{{element.name}}</h3>
                  <div class="line "></div>
                  <p>{{element.paragrafo}}</p>
                  <div class="imgSocial d-flex">
                  <img :src="element.img1" alt="">
                  <img class="mx-1" :src="element.img2" alt="">
                  <img :src="element.img3" alt="">
                  </div>
                  
                </li>                           
            </ul>
          </div>
          <div class=" twitter col-3 mt-5 ">
            <ul>
              <li v-for="(element, index) in twitter" :key=index>
                <h3>{{element.name}}</h3>
                <div class="line "></div>
                <img class="socialTwitter " :src="element.img1" alt="">
                <p>{{element.paragrafo}}</p>
                <img class="socialTwitter" :src="element.img2" alt="">
                <p>{{element.paragrafo2}}</p>
              </li>
            </ul>
          </div>
          <div class="links col-3 mt-5">
            <ul>
              <li v-for="(element,index) in links" :key=index>
                <h3>{{element.name}}</h3>
                <div class="line "></div>
                <p>{{element.text1}}</p>
                <p>{{element.text2}}</p>
                <p>{{element.text3}}</p>
                <p>{{element.text4}}</p>
                <p>{{element.text5}}</p>
              </li>
            </ul>
          </div>
          <div class="contatti col-3 mt-5">
            <ul>
              <h3>Contact me</h3>
              <div class="line "></div>
                <li><i class="fas fa-map-marker-alt"> </i><span>437 bigBlue street, NY 10013</span> </li>  
                <li><i class="fas fa-phone-alt"></i> <span>(315)5512-2579</span> </li>  
                <li><i class="fas fa-map-marker-alt"></i> <span>everlead@mikido.com</span>  </li>  
                <div class="name d-flex justify-content-between align-items-center mt-5">
                  <h6>Your Name</h6>
                  <span class="text-white">SUBSCRIBE</span>
                </div>
              <hr class="enter">
            </ul>
          </div>
        </div>
      </div>
    </div>

    <!-- footerbottom -->
    <div class="footer-bottom">
      <div class="container">
        <div class="row">
          <div class="col-12 text-center">
            <p>copyrigth EverleadMikadoThemes</p>
          </div>
        </div>
      </div>
      <div class="arrow rounded-circle d-flex justify-content-center">
        <i class="fas fa-long-arrow-alt-up mt-2 "></i>
      </div>
    </div>
  </div>
    
  
</template>

<script>
export default {
  name: 'IndexFooter',
  data:function(){
    return{
    about:[
      {
        name:"About",
        paragrafo:"Lorem ipsum dolor sit amet consectetur adipisicing elit. At ipsum numquam doloremque libero.",
        img1:require('@/assets/img/linkedin.png'),
        img2:require('@/assets/img/fb.png'),
        img3:require('@/assets/img/twitter.jpg'),
      }
    ],
      twitter:[
      {
        name:"twitter",
        paragrafo:"Lorem ipsum dolor sit amet consectetur adipisicing elit. At ipsum numquam doloremque libero.",
        img1:require('@/assets/img/twitter.jpg'),
        paragrafo2:"Lorem ipsum dolor sit amet consectetur adipisicing elit. At ipsum numquam doloremque libero.",
        img2:require('@/assets/img/twitter.jpg'),
      }
    ],
      links:[
      {
        name:"Important links",
        text1:"About me",
        text2:"About me",
        text3:"Language packs",
        text4:"Become a coach",
        text5:"Monthly events",
      }
    ],
  }

          
}
}
</script>


<style scoped lang="scss">
.footer-top{
  height:50vh ;
  background-color: black;

  & .imgSocial, .socialTwitter{
    width: 2rem;
    height: 2rem;

  }

  & .enter{
    border-bottom: 1px solid white;
    }

  &  ul li{
    list-style-type: none;
  }
  & h3, p,span{
    color: white;

  }
  & .line{
    width: 6%;
    height: 15px;
    border-top:2px solid rgb(221, 63, 0)
    
  }

  & i{
    color: orangered;
  }
}

.footer-bottom{
  position: relative;
  background-color: orangered;
  height: 5vh;

  & .arrow{
    position: absolute;
    height: 40px;
    width: 40px;
    right: 20px;
    bottom: 35px;
    background-color: white;
    
  /*   & i{
      position: absolute;
      top: 50px;
      left: 50px;
    } */
  
  }
}
</style>
