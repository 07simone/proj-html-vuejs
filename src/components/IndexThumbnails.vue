<template>
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
        <li class="mx-3" v-for="(element, index) in business" :key=index>
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
}

</style>
