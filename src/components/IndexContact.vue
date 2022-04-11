<template>

    
  <div class="jumbotron-bottom d-flex align-items-center">
    <div class="container">
      <div class="row p-5 ">
        <div class="col-6 position-relative">
          <img src="../assets/img/h1-contact-rev-01.png" alt="">
          <div class="segnaposti1">
            <img src="../assets/img/h1-contact-rev-02.png" alt="">
          </div>
          <div class="segnaposti2">
            <img src="../assets/img/h1-contact-rev-02.png" alt="">
          </div>
          <div class="segnaposti3">
            <img src="../assets/img/h1-contact-rev-02.png" alt="">
          </div>
          <div class="boxCity text-start p-3">
            <h3 class="fs-6 fw-bold">New York Coaching </h3>
            <span class="fw-bold">READ MORE</span>
          </div>
        </div>
        <div class="col-6 p-3">
          <h1 class="fw-bold">Creative Leader</h1>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
          <div class="line "></div>

          <div class="contact d-flex justify-content-around flex-wrap">
              <div class="mb-1">
                <label for="exampleInputName1" class="form-label">Your Name</label>
                <input type="text" class="form-control">
              </div>
              <div class="mb-1">
                <label for="exampleInputName1" class="form-label">Your Email</label>
                <input type="text" class="form-control">
              </div>
            
          </div>
          <div class="wrapper">
              <label for="exampleInputName1" class="form-label mt-5">Write a message...</label>
              <div class="input-group mt-3">
                  <textarea class="testo form-control" aria-label="With textarea"></textarea>
                </div>
          </div>
          <button type="button" class="btn btn-white btn-light fw-bold mt-4 P-3">SEND | <i class="fas fa-long-arrow-alt-right"></i> </button>
            
        </div>
      </div>
        <div class="row row-cols-5  ">
            <ul class="d-flex justify-content-between ">
              <li style="list-style-type: none" v-for="(element,index) in client" :key=index>
                <img  :src="element.img" alt="">
              </li>
            </ul>
        </div>
        <div class="arrow rounded-circle d-flex justify-content-center">
          <i class="fas fa-long-arrow-alt-up mt-2 "></i>
      </div>
    </div>
  </div>







</template>

<script>


export default {
  name: 'IndexContact',


  data:function(){
    return{
      client:[
        {
          img:require("../assets/img/h4-clients-img-03.png")
        },
        {
          img:require("../assets/img/h4-clients-img-05.png")
        },
        {
          img:require("../assets/img/h4-clients-img-07.png")
        },
        {
          img:require("../assets/img/h4-clients-img-09.png")
        },
        {
          img:require("../assets/img/h4-clients-img-01.png")
        },
      ]
    }

}
}

</script>


<style scoped lang="scss">
.jumbotron-bottom{
  position: relative;
  height: 60vh;
  .line{
    width: 6%;
    height: 15px;
    border-top:2px solid rgb(221, 63, 0)
    
  }
  & .form-control{
    border: none;
    border-bottom: 0.5px solid black;
    
    }
    .testo{
      height: 10px;
    }
    & .boxCity{
      position: absolute;
      top: 140px;
      left: 140px;
      height: 5rem;
      width: 15rem;
      background-color: white;
    }
    & .segnaposti1{
        position: absolute;
        top: 120px;
        left: 110px;
       /*  transform: translate(-40%, -30%); */
    
    }
     & .segnaposti2{
        position: absolute;
        top: 100px;
        left: 300px;
       /*  transform: translate(-40%, -30%); */
    
    }
     & .segnaposti3{
        position: absolute;
        top:220px;
        right: 70px;
       /*  transform: translate(-40%, -30%); */
    
    }

    & .btn{
      background-color: orangered;
      color: white;
    }
    & .arrow{
    position: absolute;
    height: 40px;
    width: 40px;
    right: 20px;
    bottom: 35px;
    background-color: lightsalmon;
  }
}

</style>
