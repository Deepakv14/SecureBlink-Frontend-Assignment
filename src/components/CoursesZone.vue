<template>
   <div ><p>Courses</p>
    <h4>Our Most Popular Courses</h4>
     <div class="courses">
    <div class="card">
    <img src="../assets/Career/career1.jpeg" alt="" id="images">
    <p>Ultimate Business Intelligence Analyst A to Z Course 2021</p>
    <p class="number">46,995 <span>Student</span></p>
    <div class="data">
    <img src="../assets/watch.svg" alt="" class="svg-icons watch">
     <p>11 hr 20 mins</p>
    </div>
   <div class="data">
    <img src="../assets/date_range-24px.svg" alt="" class="svg-icons date">
     <p>44 Lectures</p>
    </div>
    </div>

    <div class="card">
    <img src="../assets/Career/career2.jpeg" alt=""  id="images">
    <p>Adobe Photoshop Training: From Beginner to Pro</p>
    <p class="number">6,995 <span>Student</span></p>
    <div class="data">
    <img src="../assets/watch.svg" alt="" class="svg-icons watch">
     <p>6 hr 20 mins</p>
    </div>
    <div class="data">
    <img src="../assets/date_range-24px.svg" alt="" class="svg-icons date">
     <p>24 Lectures</p>
    </div>
    </div>

     <div class="card">
    <img src="../assets/Career/career3.jpeg" alt=""  id="images">
    <p>Social Media Marketing - A to Z Content Marketing class 2021</p>
    <p class="number">46,995 <span>Student</span></p>
   <div class="data">
    <img src="../assets/watch.svg" alt="" class="svg-icons watch">
     <p>11 hr 20 mins</p>
    </div>
   <div class="data">
    <img src="../assets/date_range-24px.svg" alt="" class="svg-icons date">
     <p>44 Lectures</p>
    </div>
    </div>
    </div>
    </div>
    
</template>

<script>
export default {
    name: 'CoursesZone',
}
</script>

<style scoped>
span{
    font-weight: 100;
    font-style: italic;
}

.data{
    display: flex;
    flex-direction: row;
     line-height: 1px;
}
.number{
      line-height: 1px;
}
.data>p{
    margin-top:1rem;
}
p{
    font-style:italic;
    color:#01CB63;
    font-size:2vw;
}
h4{
    font-weight: bold;
    font-size:2.5vw;
}
.card p{
     font-style:normal;
     text-align: left;
     font-weight: bold;
    color:black;
    padding:0.2rem;
    text-align: center;
}

.courses{
     display: flex;
     justify-content: center;
     flex-wrap: wrap;
}
.card{
     width: 40vmin;
    height: auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-repeat: no-repeat;
    margin:1.5rem;
    cursor: pointer;
    border:2px solid #f1f1f1;
    border-radius: 10px;
}
.svg-icons{
    transform: scale(1.3);
}
#images{
    width: 100%;
    height: 100%;
   
}
@media only screen and (max-width: 600px){
.card {
    width: auto;
    height:auto;  
}
}
</style>