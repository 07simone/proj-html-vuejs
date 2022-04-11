<template>
<div>
  <!-- thumbtop -->

    <div class="thumbTop">
      <div class="container mt-5">
      <div class="row">
        <div class="col-12 text-center">
          <div class="titolo mt-5">
          <h1>Latest News</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
          <div class="line"></div>
          </div>
        </div>
      </div>
      <div class="row justify-content-center ">
        <div class="col-12 ">
          <ul class="d-flex mt-5">
            <li class=" col-4 mx-3" v-for="(element, index) in business" :key=index>
              <div class="immagine">
                <img class=" d-flex justify-content-center img-fluid" :src="element.img" alt=""> 
                <button  type="button" class="btn"> <i class="fas fa-tag"></i>Business Leading</button>
              </div>
                <p  class=" mt-3 text-start"> <i class="far fa-clock"></i> {{element.date}}</p>
                <h3 class="text-start fw-bold">{{element.titolo}}</h3>
                <p class="text-start">{{element.description}}</p>
                <p class="text-start fw-bold">{{element.write}}</p>
            </li>
          </ul>
        </div>
      </div>
      <div class="arrow2 rounded-circle d-flex justify-content-center">
          <i class="fas fa-long-arrow-alt-up mt-2 "></i>
      </div>
    </div>
      <div class="slide-left">
          <i class="fas fa-long-arrow-alt-left"></i>
        </div>
        <div class="slide-right">
          <i class="fas fa-long-arrow-alt-right"></i>
        </div>
    </div>

<!-- thumbcenter -->
    <div class="thumbCenter">
      <div class="container">
        <div class="row">
          <div class="col-12 text-center align-items-center">
            <div class="testimonials">
                <img class="img-fluid" src="../assets/img/h3-img-07.png" alt="">
                <h2>Cyntia Clark</h2>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quidem, exercitationem! Facere temporibus laborum molestiae perspiciatis soluta quod est.</p>
                  <div class="sliderWrapper">
                    <div>01</div>
                      <div class="slideTot">
                          <div class="slide"></div>
                      </div>
                    <div>03</div> 
                  </div>
            </div>
            <div class="arrow2 rounded-circle d-flex justify-content-center">
              <i class="fas fa-long-arrow-alt-up mt-2 "></i>
            </div>
          </div>
        </div>
      </div>
        <div class="slide-left">
          <i class="fas fa-long-arrow-alt-left"></i>
        </div>
        <div class="slide-right">
          <i class="fas fa-long-arrow-alt-right"></i>
        </div>
    </div>

    <!-- thumbbottom -->


    <div class="thumbBottom">
        <div class="icons-player">
          <i class="fas fa-play"></i>
        </div>
          <div class="box1 position-absolute">
            <div class="arrow position-relative d-flex justify-content-center align-items-center">
              <i class="fas fa-shopping-cart "></i>
            </div>
          </div>
        <div class="box2 position-absolute">
            <div class="arrow position-relative d-flex justify-content-center">
              <img class="" src="../assets/img/ajax-loader.gif" alt="">
            </div>
        </div>
        <div class="arrow2 rounded-circle d-flex justify-content-center">
          <i class="fas fa-long-arrow-alt-up mt-2 "></i>
        </div>
  </div>
</div>





</template>

<script>


export default {
  name: 'IndexThumbnails',


  data:function(){
    return{
    business:[
          {
            img:require('@/assets/img/h1-blog-img-03.jpg'),
            date:"May 5,2019 Amanda Doe",
            titolo:"Next investment",
            description:"lorem ipsum dolor sit amet,consectetur adipiscing elit,sed eius mas tellus dolor...",
            write:"READ MORE"
          },
          {
            img:require('@/assets/img/h1-blog-img-02.jpg'),
            date:"May 5,2019 Amanda Doe",
            titolo:"Team Building",
            description:"lorem ipsum dolor sit amet,consectetur adipiscing elit,sed eius mas tellus dolor...",
            write:"READ MORE"
        },
          {
            img:require('@/assets/img/h1-blog-img-01.jpg'),
            date:"May 5,2019 Amanda Doe",
            titolo:"New Business Day",
            description:"lorem ipsum dolor sit amet,consectetur adipiscing elit,sed eius mas tellus dolor...",
            write:"READ MORE"
        },
    ]
    
    }
  }

}


</script>


<style scoped lang="scss">
.thumbTop{
  background-image: url(../assets/img/rbt-placeholder.jpg);
  position: relative;
  & ul{
    list-style-type: none;

    & i{
      color: orange;
    }
  }
.titolo{
  position: relative;
  & .line{
    position: absolute;
    top: 130%;
    left: 55%;
    transform: translate(-130%, -55%);
    width: 6%;
    text-align: center;
    height: 15px;
    border-top:2px solid rgb(221, 63, 0)
    
  }
}
  .immagine{
    position: relative;

    & .btn{
      position: absolute;
      right: 5%;
      bottom: -5%;
      background-color: rgb(221, 63, 0);
      color: rgb(221, 221, 221);
      font-size: 0.9rem;
      & i{
        color: rgb(221, 221, 221);
      }
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
   & .slide-left{
      position: absolute;
      top:50%;
      left: 100px;
      font-size: 2rem;
  }
  & .slide-right{
    position: absolute;
    top:50%;
    right: 100px;
    font-size: 2rem;

}
}
.thumbCenter{
  height: 50vh;
  background-color: black;
  position: relative;
  & .testimonials{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);

    & .sliderWrapper{
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    
    .slideTot{
        width: 30%; 
        height: 3px;
        background-color: gray;
        border-radius: 5px;

      & .slide{
          width: 25%;
          height: 100%;
          border-radius: 5px;
          background-color: rgba(255, 255, 255, 0.6) ;
      }
    }
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
  & .slide-left{
      position: absolute;
      top:50%;
      left: 100px;
      font-size: 2rem;
      color: white;
  }
  & .slide-right{
    position: absolute;
    top:50%;
    right: 100px;
    font-size: 2rem;
    color: white;
}
}

.thumbBottom{
  height: 90vh;
  background-image: url(../assets/img/h1-img-04.jpg);
  position: relative;
    & .icons-player{
      position: absolute;
      top:50%;
      left: 50%;
      transform: translate(-50%, - 50%);
      & i{
        color: white;
        font-size: 2rem;
      }
    }
    & .box1{
      position: absolute;
      right:0%;
      top: 2.5%;
      background-color: white;
      width: 2rem;
      height: 2rem;
    }
    & .box2{
      position: absolute;
      right:0%;
      top: -2%;
      background-color: red;
      width: 2rem;
      height: 2rem;
    }
    & .arrow2{
    position: absolute;
    height: 40px;
    width: 40px;
    right: 20px;
    bottom: 35px;
    background-color: lightsalmon;
  }
}

</style>
