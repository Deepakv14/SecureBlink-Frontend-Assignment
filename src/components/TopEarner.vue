<template>
<div>
    <p>Top Earners</p>
    <h4>Transformng your ideas into reality</h4>

    <div class="earners">
        <div class="card">
            <img src="../assets/Earners/luis-villasmil-hh3ViD0r0Rc-unsplash.png" alt="" id="images">
            <div class="base">
                <span>₹8,00,000</span></div>
        </div>

        <div class="card">
            <img src="../assets/Earners/craig-mckay-jmURdhtm7Ng-unsplash.png" alt="" id="images">
            <div class="base">
                <span>₹6,00,000</span></div>
        </div>

        <div class="card">
            <img src="../assets/Earners/christopher-campbell-rDEOVtE7vOs-unsplash.png" alt="" id="images">
            <div class="base">
                <span>₹5,00,000</span></div>
        </div>

        <div class="card">
            <img src="../assets/Earners/jonas-kakaroto-mjRwhvqEC0U-unsplash.png" alt="" id="images">
            <div class="base">
              
                <span>₹4,50,000</span></div>
        </div>

    </div>
</div>
</template>

<script>
export default {
    name: 'TopEarner',
}
</script>

<style scoped>
 p{
    font-style:italic;
    color:#01CB63;
    font-size: 2vw;
}
h4{
    font-weight: bold;
    font-size: 2.5vw;
}
.card {
    width: auto;
    border:none;
    height: 35vh;
    display: flex;
    flex-direction: column;
    margin: 2vmax;
    cursor: pointer;
}

.earners {
    display: flex;
    flex-wrap: wrap;
    width: 90vw;
    margin: auto;
    justify-content: center;
}

.base {
    display: flex;
    flex-direction: row;
    float: left;
}
span{
     border-left: 6px solid green;
     font-size: 0.8rem;
     font-weight: bold;
     padding: 1rem;
}


#images {
    width: 100%;
    height: 30vh;
    padding-bottom: 0.2rem;
    object-fit: cover;
}
@media only screen and (max-width: 600px){
.card {
    width: auto;
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
