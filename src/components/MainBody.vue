<template>
    <div class="main-wrapper">
        <div class="main-latest-work">
            <div class="main-latest-work-upper">
                <div class="main-latest-work-heading">
                    <h1>Latest Works</h1>
                    <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book</p>
                </div>
                <div class="latest-items">
                    <ul>
                        <li class="listing active">All</li>
                        <li class="listing">Branding Goals</li>
                        <li class="listing">Photography</li>
                        <li class="listing">True Perfection</li>
                        <li class="listing">Web desiging</li>
                    </ul>
                    <div class="app-container">
                        <div class="row">
                            <div class="column">
                                <a href="#">
                                    <img src="../assets/1.jpg" >
                                </a>
                                </div>
                                <div class="column">
                                    <a href="#">
                                        <img src="../assets/2.jpg" >
                                    </a>
                                </div>
                                <div class="column">
                                    <a href="#">
                                        <img src="../assets/3.jpg" >
                                    </a>
                                </div>
                                <div class="column">
                                    <a href="#">
                                        <img src="../assets/4.jpg" >
                                    </a>
                                </div>
                                <div class="column">
                                    <a href="#">
                                        <img src="../assets/5.jpg" >
                                    </a>
                                </div>
                                <div class="column">
                                    <a href="#">
                                        <img src="../assets/6.jpg" >
                                    </a>
                                </div>
                                <div class="column">
                                    <a href="#">
                                        <img src="../assets/7.jpg" >
                                    </a>
                                </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
       <MainWorkExpVue/>
    </div>
</template>
<script>
    import MainWorkExpVue from './MainWorkExp.vue';
    export default{
        name:"Mainbody",
        components:{
            MainWorkExpVue
        },
      mounted(){
        let listselected=[...document.querySelectorAll(".listing")]
        listselected.forEach((list)=>{
            list.addEventListener("click",()=>{
                listselected.forEach(li=>li.classList.remove("active"))
                list.classList.add("active")
            })
        })
      }
    }
</script>
<style>
    .main-wrapper{
        float: left;
        margin: 0px;
    }
    .main-latest-work{
        padding: 0px 30px;
    }
.main-latest-work-heading p{
    margin-bottom: 50px;
    color: darkgray;
}
.main-latest-work-upper{
    margin-top: 50px;
    text-align: center;
}
.main-latest-work-heading h1{
    margin-bottom: 25px;
}
.app-container{
    padding-bottom: 40px;
}
.latest-items ul{
    margin: 0%;
    padding: 0%;
    margin-bottom: 25px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
.latest-items{
    margin-top: 40px;
    font-weight: 700;
}
.latest-items ul li{
    cursor: pointer;
    list-style: none;
    padding: 0 20px;
    font-size: 21px;
    color: rgb(107, 104, 104);
}
.active{
    color:rgb(255, 255, 3) !important;
    border-bottom: 2px solid yellow;
}
.row {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-wrap: wrap; 
  flex-wrap: wrap;
  padding: 0 4px;
}

.column {
    box-sizing: border-box;
  -ms-flex: 25%; 
  flex: 25%;
  padding: 0 4px;
}

.column img {
  margin-top: 8px;
  vertical-align: middle;
  width: 100%;
}

@media screen and (max-width: 767px) {
  .column {
    -ms-flex: 50%;
    flex: 50%;
    max-width: 50%;
  }
}

@media screen and (max-width: 600px) {
  .column {
    -ms-flex: 100%;
    flex: 100%;
    max-width: 100%;
  }
}
</style>