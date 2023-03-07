<template>
<div class="banner">
    <div class="banner-left">
        <h2>Anytime, Anywhere<br />Learn On Your Schedule<br />From Any Device</h2>
        <p class="italics">We Believe everyone has the capcity to be creative <span class="span-text">Course Pro</span> is a place where people develop their own potential</p>
        <button class="italics">Let's Get Start</button>
    </div>
    <div class="banner-right"><img src="../assets/studybanner.jpg" alt="banner"></div>
</div>
</template>

<script>
export default {
    name: 'BannerHead',
}
</script>

<style scoped>



.banner{
    display: flex;
    flex-direction: row;
}
.banner-left{
    width:50%;
    height:auto;
    background: #01CB63;
    padding:2rem;
}
.banner-left h2{
    color:#FFFFFF;
    font-size: 2.5rem;
    text-align: left;
    padding:1rem;
}
.banner-left p{
    color:#1F2532;
    font-size: 1.2rem;
    text-align: left;
    padding:2rem;
}
.italics{
    font-style: italic;
}
.banner-right{
    width:50%;
    height:auto;
}
.banner-right>img{
    width:100%;
      height:100%;
}
.span-text{
    font-style: normal;
    font-weight: bold;
    color:white;
}
button{
    padding:12px;
    float:left;
    margin-left: 4rem;
    color:white;
    outline: none;
    border:none;
    border-radius: 5px;
    background-color: #000000;
}


@media screen and (max-width: 992px) {
 .banner {
   display: flex;
   flex-direction: row;
}
.banner-left{
    width:50%;
     height:auto;
}
.banner-right{
    width:50%;
    height:auto;
}

.banner-left h2{
    font-size: 1.5rem;
    text-align: left;
    padding:0.5rem;
}
.banner-left p{
    font-size: 14px;
    text-align: left;
    padding:0.8rem;
}
.banner-left button{
    font-size: 1vw;
    margin-left: 0.5rem;
    padding:0.5rem;
}
}

@media screen and (max-width: 600px) {
 .banner {
   display: flex;
   flex-direction: row;
   flex-wrap: wrap;
   justify-content: center;
}

.banner-left{
    width:100%;
     height:auto;
}
.banner-right{
    width:100%;
    height:auto;
}

.banner-left h2{
    font-size: 1.5rem;
    text-align:left;
    padding:0;
}
.banner-left p{
    font-size: 12px;
    text-align: left;
    padding:0;
}
.banner-left button{
    font-size: 10px;
    margin-left: 0.5rem;
}
}


</style>
