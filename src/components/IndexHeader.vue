<template>
  <div class="header">
    <section class="nav">
          <img class="logo" src="../assets/img/logo-img-01.png" alt="" > 
              <ul>
                <li v-for="(element, index) in listaMenu" :key=index>
                  <a :href="element.url"></a>
                  <h5>{{element.name}}</h5>
                  <a href="#"></a>
                </li>
                <i class="fas fa-search"></i>
                <i class="fas fa-list-ul"></i>
              </ul>
    </section>
    <section class="information">
        <div class="container-fluid">
          <div class="row">
            <div class="col-6">
              <img src="../assets/img/logo-img-01.png" alt="">
              <p class="mt-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate odio sint, accusantium minima illum deleniti veniam iste 
                aliquam quaerat nemo, beatae sapiente earum. Consequuntur animi autem architecto quidem natus reprehenderit.</p>
                <div class="bottoni">
                    <button type="button" class="btn btn-white btn-light fw-bold">READ MORE | <i class="fas fa-long-arrow-alt-right"></i> </button>
                    <button type="button" class="btn btn-light fw-bold">PURCHASE | <i class="fas fa-long-arrow-alt-right"></i></button>
                </div>
              
            </div>
          </div>
        </div>
    </section>
    
  </div>
</template>

<script>
export default {
  name: 'IndexHeader',
  data:function(){
    return{
      listaMenu:[
        {
          name: "HOME",
          url:"#"
        },
        {
          name: "PAGES",
          url:"#"
        },
        {
          name: "BLOG",
          url:"#"
        },
        {
          name: "SHOP",
          url:"#"
        },
        {
          name: "EVENTS",
          url:"#"
        },
        {
          name: "ELEMENTS",
          url:"#"
        },
      ]
    }
  }
}


</script>


<style scoped lang="scss">
.header{
  background-image: url(../assets/img/rev-slider-main-home-img-03.jpg);
  height: 100vh;
.nav{
  justify-content: space-between;
  display: flex;
.logo{
  height: 50px;
  margin-left: 2rem;
}
  ul{
    height: 100%;
    align-items: center;
    display: flex;
    justify-content: end;
  }

  li{
    list-style-type: none;
    padding: 0.8rem;
    text-transform: uppercase;
    font-size: 0.8rem;
    align-self: center;
    line-height: 12vh;
    margin-right: 2rem;

    &:hover{
      color: rgb(221, 63, 0)

    }
  }
  a{
      text-decoration: none;
      color: black;
    }
  i{
    margin-right: 1.5rem;
  }
}
  .information{
    padding: 25rem  10rem
  }
  .btn{
      margin-right: 2rem;
      &:hover{
        background-color: rgb(221, 63, 0);
        color: white;
        
      }
    }
}
</style>
