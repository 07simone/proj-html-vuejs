<template>
  <div class="main">

<!-- contenitorespecialità -->

    <div class="contenitore1">
      <div class="container">
        <div class="row">
          <div class="col-12 text-center mt-4">
            <h1 class="fw-bold">Our specialties</h1>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
          </div>
        </div>
          <div class="row">
            <div class="col-12 ">
                <ul class="d-flex mt-5">
                  <li class="" v-for="(element,index) in specialità" :key=index>
                    <img class="d-flex justify-content-center" :src="element.img" alt=""> 
                    <h3 class="fw-bold mt-3 text-center">{{element.text}}</h3>
                    <p class="text-center">{{element.description}}</p>
                  </li>
              </ul>
            </div>
          </div>
      </div>
    </div>

<!-- contenitore secondario -->

    <div class="contenitore2">
      <div class="biographi">
        <img class="h-50 w-50" src="../assets/img/h1-img-01.jpg" alt=""> 
        <div class="box position-absolute">
          <div class="arrow position-relative">
              <i class="fas fa-long-arrow-alt-left mx-1"></i>
              <i class="fas fa-long-arrow-alt-right"></i>
          </div>
        
        </div>
      </div>
    </div>

  <!--  contenitoreFounder -->

    <div class="contenitore3 p-3">
        <div class="name">
            <h1 class="fw-bold fs-4"> Jason Bickford</h1>
            <p>founder and executive directon</p>
            <div class="line "></div>
        </div>
        
          <p class="lorem mt-1">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem quod animi nobis sit repellat porro nihil eaque in, repellendus totam doloremque, ut corrupti. Voluptatum dolorem aliqua..</p>
          <div class="social d-flex ">
            <i class="fab fa-facebook"></i>
            <i class="fab fa-linkedin mx-1"></i>
            <i class="fab fa-twitter"></i>
          </div>
    </div> 

    <!-- cambiaPagina -->
      <div class="changePage">
            <div class="arrow2 rounded-circle d-flex justify-content-center">
              <i class="fas fa-long-arrow-alt-up mt-2 "></i>
            </div>
            <div class="arrow3 rounded-circle d-flex justify-content-center">
              <i class="fas fa-long-arrow-alt-up mt-2 "></i>
            </div>
      </div>
    
  </div>
</template>

<script>
export default {
  name: 'IndexMain',
  data:function(){
    return{
      specialità:[
        {
          img:require('@/assets/img/logo-side-area-img-01-1.png'),
          text:"Knowing",
          description:"lorem ipsum dolor sit amet quis consect"
        },
        {
          img:require('@/assets/img/logo-side-area-img-01-1.png'),
          text:"Selling",
          description:"lorem ipsum dolor sit amet quis consect"
        },
        {
          img:require('@/assets/img/logo-side-area-img-01-1.png'),
          text:"Learning",
          description:"lorem ipsum dolor sit amet quis consect"
        },
        {
          img:require('@/assets/img/logo-side-area-img-01-1.png'),
          text:"Contact",
          description:"lorem ipsum dolor sit amet quis consect"
        },
      ]
      
    }
  }

}


</script>


<style scoped lang="scss">
.main{
  background-image:  url(../assets/img/rbt-placeholder.jpg);
  height: 100vh;
  position: relative;
.contenitore1{
  display: flex;
  position: absolute;
  left: 50%;
  transform: translate( - 50%);
  height: 500px;
  width: 1200px;
  background-color: rgb(81, 243, 189);
  margin-top: -2rem;
  
  ul{
    margin-left: 2rem;
    list-style-type: none;
    li{
      text-align:-moz-center
    }
  }

}
.contenitore2{
  position: absolute;
  bottom:10%;
  left:50%;
  transform: translate( -50%, - 10%);


  .box{
    position: absolute;
    bottom:0%;
    left: 0%;
    background-color: rgb(221, 63, 0);
    width: 5rem;
    height: 3rem;

    .arrow{
      top: 50%;
      left: 50%;
      transform: translate(-50%, - 50%);
      display: flex;
      justify-content: center;
      
    }
  }
}
.contenitore3{
  bottom:130px;
  right:450px;
  transform: translate( -23%, - 15%);
  position: absolute;
  height: 200px;
  width: 450px;
  background-color: white;

  .lorem{
    font-size: 0.6rem;
    color: rgb(175, 171, 171);
  }
.social{
  i{
    color:red
  }
}
  .line{
    width: 20%;
    height: 15px;
    border-top:2px solid rgb(221, 63, 0)
    
  }
} 
& .arrow2{
    position: absolute;
    height: 40px;
    width: 40px;
    right: 20px;
    bottom: 35px;
    background-color: lightsalmon;
  }
  & .arrow3{
    position: absolute;
    height: 40px;
    width: 40px;
    right: 20px;
    top: 80px;
    background-color: lightsalmon;
  }
}
</style>
