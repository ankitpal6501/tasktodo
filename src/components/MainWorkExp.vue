<template>
    <div class="main-work-experience">
        <div class="main-work-exp-heading">
            <h1>Work Experience</h1>
            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. 
                Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                 when an unknown printer took a galley of type and scrambled it to make a type specimen book</p>
        </div>
    </div>
    <div class="main-exp-bottom">
        <div class="designre-data">
            <p> <span> June 2012-2016 </span></p>
            <h4>UI/UX Designer</h4>
            <p>Adobe Inc</p>
            <p class="details">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                 when an unknown printer took a galley of type and scrambled it to make a type specimen book</p>
        </div>
        <div class="designre-data">
            <p> <span> June 2012-2016 </span></p>
            <h4>Product Designer</h4>
            <p>Adobe Inc</p>
            <p class="details">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                 when an unknown printer took a galley of type and scrambled it to make a type specimen book</p>
        </div>
        <div class="designre-data">
            <p> <span> June 2012-2016 </span></p>
            <h4>Graphic Designer</h4>
            <p>Adobe Inc</p>
            <p class="details">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                 when an unknown printer took a galley of type and scrambled it to make a type specimen book</p>
        </div>
    </div>
</template>
<script>
    export default{
        name:"MainWorkExp"
    }
</script>
<style>
    .main-work-exp-heading h1{
        margin-bottom: 25px;
}
    .main-work-exp-heading p{
        margin: 0px;
        color: darkgray;
}
.main-work-experience{
    padding: 0px 30px;
    background-color: rgb(244, 244, 244);
    text-align: center;
}
.main-work-exp-heading{
    padding-top: 20px;
}
.main-exp-bottom{
    padding: 70px 30px;
    background-color: rgb(244, 244, 244);
    display: flex;
    justify-content: space-around;
}
.designre-data{
    background-color: #ffffff;
    border: 1px solid rgb(227, 223, 223);
    padding: 20px;
}
.designre-data p{
    color: darkgray;
    margin: 0;
    margin-bottom: 7px;
}
.designre-data p {
    margin:0;
    margin-bottom: 7px;
}
.designre-data h4{
    margin: 10px 0px;
}
.designre-data .details{
    margin: 12px 0px;
}
@media screen and (max-width: 767px) {
    /* .main-exp-bottom{
        flex-wrap: wrap;
  } */
}
</style>