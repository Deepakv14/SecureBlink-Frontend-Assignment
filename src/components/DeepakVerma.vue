<template>
<div class="topnav">
  <a  href=""><img src="../assets/Group3.png" alt=""></a>
  <div class="topnav-right">
    <a href="">Login</a>
    <a href="" class="active">Register</a>
  </div>
</div>
</template>

<script>
export default {
    name: 'DeepakVerma',
   
}
</script>

<style scoped>
img{
    transform: scale(0.7);
}

.topnav {
    position: sticky;
    top:0;
  overflow: hidden;
  background-color: white;
}

.topnav a {
  float: left;
  color: black;
  text-align: center;
  padding: 0.2rem;
  text-decoration: none;
  font-size: 17px;
}

.topnav-right {
  float: right;
  margin:2rem;
  padding-right: 0.5rem;
}
.active {
    background-color: #01CB63;
    border-radius: 5px;
}


@media only screen and (max-width: 600px){
img{
    transform: scale(0.6);
}
.topnav a {
  font-size: 15px;
}
.topnav-right {
  margin-top:-3rem;
}
}
@media only screen and (min-width: 412px){
img{
    transform: scale(0.6);
}
.topnav a {
  font-size: 15px;
}
.topnav-right {
  margin-top: 1.1rem;
}
}
@media only screen and (max-width: 308px){
img{
    transform: scale(0.5);
    margin-left:-2rem;
}
.topnav a {
  font-size: 12px;
}
.topnav-right {
  margin-top:-2.6rem;
}
}
</style>
