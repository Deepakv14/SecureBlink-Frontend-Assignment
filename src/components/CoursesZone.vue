<template>
<div class="courses">
    <p>Courses</p>
    <h4 >Our Most Popular Courses</h4>
        <div class="card-row">
        <div class="card">
            <img src="../assets/Career/career1.jpeg" alt="" id="images">
            <p>Ultimate Business Intelligence Analyst A to Z Course 2021</p>
            <p class="number">46,995 <span>Student</span></p>
            <div class="data">
                <div class="left">
                    <img src="../assets/watch.svg" alt="" class="svg-icons watch">
                    <p>11 hr 20 mins</p>
                </div>
                <div class="right">
                    <img src="../assets/date_range-24px.svg" alt="" class="svg-icons date">
                    <p>44 Lectures</p>
                </div>
            </div>
            <div class="Line"></div>
            <div class="User">
            <img src="../assets/Earners/christopher-campbell-rDEOVtE7vOs-unsplash.png" alt="">
            <p>Christopher Campbell</p>
            <span>₹2000</span>
            </div>
        </div>

        <div class="card">
            <img src="../assets/Career/career2.jpeg" alt="" id="images">
            <p>Adobe Photoshop Training: From Beginner to Pro</p>
            <p class="number">6,995 <span>Student</span></p>
           <div class="data">
                <div class="left">
                    <img src="../assets/watch.svg" alt="" class="svg-icons watch">
                    <p>11 hr 20 mins</p>
                </div>
                <div class="right">
                    <img src="../assets/date_range-24px.svg" alt="" class="svg-icons date">
                    <p>44 Lectures</p>
                </div>
            </div>
             <div class="Line"></div>
            <div class="User">
            <img src="../assets/Earners/jonas-kakaroto-mjRwhvqEC0U-unsplash.png" alt="">
            <p>Jonas Kakaroto</p>
            <span>₹2000</span>
            </div>
        </div>

        <div class="card">
            <img src="../assets/Career/career3.jpeg" alt="" id="images">
            <p>Social Media Marketing - A to Z Content Marketing class 2021</p>
            <p class="number">46,995 <span>Student</span></p>
            <div class="data">
                <div class="left">
                    <img src="../assets/watch.svg" alt="" class="svg-icons watch">
                    <p>11hrs 20 mins</p>
                </div>
                <div class="right">
                    <img src="../assets/date_range-24px.svg" alt="" class="svg-icons date">
                    <p>44 Lectures</p>
                </div>
            </div>
             <div class="Line"></div>
            <div class="User">
            <img src="../assets/Earners/luis-villasmil-hh3ViD0r0Rc-unsplash.png" alt="">
            <p>Luis Villasmil</p>
            <span>₹2000</span>
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
p{
    color:#01CB63;
    font-style:italic;
    font-size: 1.2rem;
}
h4{
     font-size: 1.5rem;
     font-weight:bold;
}
span {
    font-weight: 100;
    font-style: italic;
}

.data {
    display: flex;
    flex-direction: row;
    line-height: 1px;
}
.left{
    margin-right: 5rem;
    display: flex;
    flex-direction: row;
    align-items: center;
}
.right{
     display: flex;
    flex-direction: row;
    align-items: center;
}
.left >p{
   font-size:0.6rem;
    line-height: 0.5rem;
    padding:1rem;
}
.left >img{
    transform: scale(1);
}
.right >img{
    transform: scale(1);
}
.right >p{
       font-size:0.6rem;
    line-height: 0.5rem;
    padding:1rem;
}
.Line{
    border: 1px solid #E6E6E6;
    width:90%;
}
.User{
    display:flex;
    padding:0;
    align-items: center;
}
.User>p{
    font-weight:100;
    font-size: 0.8rem;
}
.User>span{
   padding:2rem;
   color:#01CB63;
   font-weight:bold;
   font-style: normal;
}
.User img{
    width:30px;
    height:30px;
  border-radius:50%;
  padding:4px;
}

.number {
    margin-top:-1rem;
    font-size: 1rem;
}

.card p {
    font-style: normal;
    text-align: left;
    font-weight: bold;
    color: black;
    padding: 0.2rem;
    text-align: center;
}

.card-row{
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.card {
    width: 40vmin;
    height: auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-repeat: no-repeat;
    margin: 1.5rem;
    cursor: pointer;
    border: 2px solid #f1f1f1;
    border-radius: 10px;
}

.svg-icons {
    transform: scale(1.3);
}

#images {
    width: 100%;
    height: 100%;
    object-fit: cover;

}

@media only screen and (max-width: 600px) {
    .card {
        width: auto;
        height: auto;
    }
    p{
    color:#01CB63;
    font-style:italic;
    font-size: 0.8rem;
}
h4{
     font-size: 1rem;
     font-weight:bold;
}
}
@media only screen and (max-width: 992px) {
    .card {
        width: auto;
        height: auto;
    }
    .User>p{
    font-weight:100;
    font-size: 0.8rem;
}
}

</style>
