<template>
    <div class="refer">
      <p>Refer</p>
      <h4>How It's Work</h4>
      <img src="../assets/Refer/Path.svg" alt="">
    </div>
</template>

<script>
export default{
    name: 'ReferWork',
   
}
</script>

<style scoped>
p{
    font-style:italic;
    color:#01CB63;
    font-size: 1.8vw;
}
h4{
    font-weight: bold;
    font-size: 2.5vw;
}
img{
    width: 100%;
    height: 100%;
}
.refer{
  margin: 7vw;
  text-align: left;
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