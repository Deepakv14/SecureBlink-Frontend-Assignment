<template>
    <div class="contact">
    <p>Contact Us</p>
    <h4>Reach Out With Any Question You Have</h4>
    <ContactPart/>
    </div>
</template>
<script>
import ContactPart from './ContactPart.vue';
export default{
    name: 'ContactUs',
    components: {
        ContactPart,
    }
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

@media only screen and (max-width: 600px){

 p{
    font-size: 3vw;
}
h4{

    font-size: 3.5vw;
}
}
</style>
