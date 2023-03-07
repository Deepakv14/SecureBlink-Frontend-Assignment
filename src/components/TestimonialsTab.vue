<template>
<p>Testimonials</p>
     <h4>Check out What Our Students Think About Us</h4>
    <div class="testimonials">
   <div class="card-row">
    <div class="card">
    <p>It's a comprehensive online learning platform for everyone looking to learn and course pro. provinding this platform which is very beneficial for practicals. Students can revise everything at home like dissection and slides</p>
    <span>Anshul Jain</span>
    <h6>Yesterday</h6>
    </div>

    <div class="card">
    <p>It's A Comprehensive Online Learning Platform For Everyone Looking To Learn And Course Pro. Provinding This Platform Which Is Very Beneficial For Practicals. Students Can Revise Everything At Home Like Dissection And Slides</p>
    <span>Rajkumar Jain</span>
    <h6>Yesterday</h6>
    </div></div>
    </div>
</template>

<script>
export default{
    name: 'TestimonialsTab',
}
</script>

<style scoped>

p{
    font-style:italic;
    color:#01CB63;
    font-size:2vw;
}
h4{
    font-weight: bold;
    font-size:2.5vw;
}
h6{
    font-size: 15px;
    font-weight: 100;
}
.card-row {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.card {
    width: 30vw;
    height:auto;
    margin: 3vmax;
    background-color: white;
    padding: 2vmax;
    cursor: pointer;
    transition: all 0.5s ease-in;
    box-shadow: 0px 6px 15px rgba(53, 53, 53, 0.353);
}
b{
    color:#545D7A;
    font-style:normal;
}

.card>p{
     font-style:italic;
    color:#545D7A;
}
.card:hover {
    box-shadow: 0px 6px 15px rgba(53, 53, 53, 0.353);
    transform: translateY(-0.4vmax);
}
span {
    color:black;
    font-weight: bold;
    font-size: 2vmax;

}
.card-row{
    margin:2rem;
}

@media only screen and (max-width: 600px){
.card {
    width: 40vw;
    height:auto;
}
 p{
    font-size: 3vw;
}
h4{

    font-size: 3.5vw;
}
}
</style>
