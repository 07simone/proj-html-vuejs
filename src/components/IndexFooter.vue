<template>
  <div>

    <!-- footertop -->

<div class="footer-top mt-5">
      <div class="container">
        <div class="row ">
          <div class="col-3 mt-5">
            <ul>
              <h3>About</h3>
              <div class="line "></div>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. At ipsum numquam doloremque libero.</p>
              <div class="social-icons">
                <i class="fab fa-linkedin"></i>
                <i class="fab fa-facebook mx-2"></i>
                <i class="fab fa-twitter"></i>
              </div>
            </ul>
          </div>
          <div class="col-3 mt-5">
            <ul>
              <h3>Twitter</h3>
              <div class="line "></div>
              <div class="social-twitter d-flex">
                <ul>
                  <li>
                    <i class="fab fa-twitter "> </i>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ipsa consectetur</p>
                  </li>
                  <li>
                    <i class="fab fa-twitter "> </i>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ipsa consectetur</p>
                  </li>
                </ul>
              </div>
            </ul>
          </div>
          <div class="col-3 mt-5">
            <ul>
              <h3>Important links</h3>
              <div class="line "></div>
              <li>About me</li>
              <li>About me</li>
              <li>language packs</li>
              <li>become a coach</li>
              <li>monthli events</li>
            </ul>
          </div>
          <div class="col-3 mt-5">
            <ul>
              <h3>Contact me</h3>
              <div class="line "></div>
                <li><i class="fas fa-map-marker-alt"> </i> 437 bigBlue street, NY 10013</li>  
                <li><i class="fas fa-phone-alt"></i> (315)5512-2579</li>  
                <li><i class="fas fa-map-marker-alt"></i> everlead@mikido.com </li>  
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
    
  }

}
}

</script>


<style scoped lang="scss">
.footer-top{
  height:50vh ;
  background-color: black;

  & .enter{
    border-bottom: 1px solid white;
    }

  &  ul li{
    list-style-type: none;
  }
  & h3{
    color: white;
  }
  & .line{
    width: 6%;
    height: 15px;
    border-top:2px solid rgb(221, 63, 0)
    
  }
  & .social-icons i{
    color: white;
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
