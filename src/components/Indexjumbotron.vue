<template>
<div>
<div class="jumbotron-top">
    <div class="container.fluid">
      <div class="box-eventi">
        <h2 class="mx-3">Upcoming Events</h2>
        <ul class="list-group">
            <li class="listaCittà" v-for="(element,index) in eventi" :key="index">
              <h3>{{element.città}}</h3>
              <p><i class="far fa-clock"></i>{{element.orario}}</p>
              <p><i class="fas fa-map-marker-alt"></i>{{element.luogo}}</p>
              <span>{{element.leggere}}</span>
              <div class="box-date text-center">
                <h5>07</h5>
                <p>jan 2022</p>
              </div>
            </li>
        </ul>
      </div>
    </div>
        <div class="arrow2 rounded-circle d-flex justify-content-center">
          <i class="fas fa-long-arrow-alt-up mt-2 "></i>
        </div>
  </div>

  <div class="jumbotron-bottom d-flex align-items-center">
    <div class="container">
      <div class="row p-5 ">
        <div class="col-6">
          <h1 class="fw-bold">Creative Leader</h1>
          <div class="line "></div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aut eaque nobis labore, exercitationem sit animi quisquam nam maxime tempora, hic distinctio earum repellat recusandae at doloremque, necessitatibus harum deleniti quos.</p>
          <span class="fw-bold">READ MORE</span>
        </div>
        <div class="col-6 p-3">
          <div class="dati d-flex justify-content-between">
            <h5 class="fw-bold">Mentorship</h5>
            <span>78%</span>
          </div>
          <div class="progress" style="height:3%">
                <div class="progress-bar bg-warning" role="progressbar" style="width: 78%" aria-valuenow="75" aria-valuemin="0" aria-valuemax="30"></div>
          </div>
          <div class="dati d-flex justify-content-between">
            <h5 class="fw-bold">Education</h5>
            <span>95%</span>
          </div>
          <div class="progress" style="height:3%">
                <div class="progress-bar bg-warning" role="progressbar" style="width: 95%" aria-valuenow="75" aria-valuemin="0" aria-valuemax="30"></div>
          </div>
          <div class="dati d-flex justify-content-between">
            <h5 class="fw-bold">Learning</h5>
            <span>65%</span>
          </div>
          <div class="progress" style="height:3%">
                <div class="progress-bar bg-warning" role="progressbar" style="width: 65%" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
          </div>
          <div class="dati d-flex justify-content-between">
            <h5 class="fw-bold">Motivation</h5>
            <span>83%</span>
          </div>
          <div class="progress" style="height: 3%">
                <div class="progress-bar bg-warning" role="progressbar" style="width: 83%" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
          </div>
        </div>
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
  name: 'IndexJumbotron',
  data:function(){
    return{
      eventi:[
        {
          città:"Melbourne Coaching",
          orario:"9:00am - 5:00pm,Jan 7,2022",
          luogo:"Cambridge,MA 02138,USA",
          leggere:"READ MORE"
        },
        {
          città:"New York Coaching",
          orario:"9:00am - 5:00pm,Jan 7,2022",
          luogo:"Cambridge,MA 02138,USA",
          leggere:"READ MORE"
        },
        {
          città:"London Coaching",
          orario:"9:00am - 5:00pm,Jan 7,2022",
          luogo:"Cambridge,MA 02138,USA",
          leggere:"READ MORE"
        },
      ]
      
    }
  }

}


</script>


<style scoped lang="scss">
.jumbotron-top{
  height: 100vh;
  background-image: url(../assets/img/h1-img-09.jpg);
  position: relative;

  .box-eventi{
    position: absolute;
    top:50%;
    left: 27%;
    transform: translate(-27%, - 50%);
    width: 26rem;
    height: 34rem;
    background-color: lightyellow;
    
    .listaCittà{
      position: relative;
      list-style-type: none;
      font-size: 0.8rem;
      margin-top: 1rem;
      margin-left: 5rem;
      &:hover{
        background-color: white;
      }
      i{
        color:red
      }

      .box-date{
        position: absolute;
        top: 30%;
        left: -20%;
        width: 60px;
        height: 60px;
        background-color: rgb(221, 63, 0) ;
        color: white;
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
}

.jumbotron-bottom{
  position: relative;
  height: 60vh;
  .line{
    width: 6%;
    height: 15px;
    border-top:2px solid rgb(221, 63, 0)
    
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
