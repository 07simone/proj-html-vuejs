<template>
  <div class="jumbotron">

    <div class="contenitore">
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
                    <img class=" d-flex justify-content-center" :src="element.img" alt=""> 
                    <h3 class="fw-bold mt-3 text-center">{{element.text}}</h3>
                    <p class="text-center">{{element.description}}</p>
                  </li>
              </ul>
            </div>
          </div>
      </div>
    </div>

    <div class="contenitore2">
      <div class="biographi">
        <img class="h-50 w-50" src="../assets/img/h1-img-01.jpg" alt=""> 
      </div>
    </div>
    <div class="contenitore3 p-3">
      <h1 class="fw-bold fs-4"> Jason Bickford</h1>
      <p>founder and executive directon</p>
      <p class="lorem mt-1">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem quod animi nobis sit repellat porro nihil eaque in, repellendus totam doloremque, ut corrupti. Voluptatum dolorem aliqua..</p>
      <div class="social d-flex ">
        <i class="fab fa-facebook"></i>
        <i class="fab fa-linkedin"></i>
        <i class="fab fa-twitter"></i>
      </div>
    
    </div> 
  </div>
</template>

<script>
export default {
  name: 'IndexJumbotron',
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
.jumbotron{
  background-image:  url(../assets/img/rbt-placeholder.jpg);
  height: 100vh;
  position: relative;
.contenitore{
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
}
.contenitore3{
  bottom:15%;
  right:23%;
  transform: translate( -23%, - 15%);
  position: absolute;
  height: 200px;
  width: 450px;
  background-color: white;

  .lorem{
    font-size: 0.8rem;
    color: rgb(175, 171, 171);
  }

  .social{
  
  } 
} 
}
</style>
