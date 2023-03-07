<template>
<div class="container">
    <div class="Info">
        <div class="info1">
            <h4>Contact Information</h4>
            <div>
                <img src="../assets/Contact/Mail.png" alt="">
                <p>contact@coursepro.com</p>
           
                <img src="../assets/Contact/Telephone.png" alt="">
                <p>1800-562-895, 1800-869-877</p>
            
                <img src="../assets/Contact/Location.png" alt="">
                <p>102 Street, India</p>
            </div>
        </div>
        <br/>
        <div class="info2">
            <h4>Social Media Channel</h4>
            <div>
              <img src="../assets/SocialMedia/Facebook.svg" alt="">
                <img src="../assets/SocialMedia/Github.svg" alt="">
                <img src="../assets/SocialMedia/Linkedin.svg" alt="">
                <img src="../assets/SocialMedia/Twitter.svg" alt="">
            </div>
        </div>
    </div>
    <div class="form">
        <p>Fill up the form and our team will get back to you within 24 hours</p>
        <div class="details">
            <div class="details1">
                <label for="name"></label>
                <input type="text" placeholder="Name" id="name">
                <label for="email"></label>
                <input type="email" placeholder="Email" id="email">
                <label for="phone"></label>
                <input type="tel" placeholder="Phone" id="phone">
                <label for="subject"></label>
                <input type="text" placeholder="Subject" id="subject"></div>
            <div class="details2">
                <label for="message"></label>
                <textarea name="message" placeholder="Message" cols="43" rows="5"></textarea>
            </div>
            <button class="btn">Submit</button>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'ContactPart',
}
</script>

<style scoped>
.container {
    width: auto;
    background: #F8F9FB;
    display: grid;
    grid-template-columns: 1fr 1fr;
    flex-wrap: wrap;
    padding: 6vmax;
}
p, h4{
    font-weight: bold;
}



.details2 {
    margin: 2vmax;
    display: flex;
    flex-direction: column;
}

.form input {
     width: 60%;
    outline: none;
    border: none;
    font-style: italic;
    border-bottom: 2px solid #01CB63;
    background: #F8F9FB;
    margin: 1rem;
}

.form textarea {
    width: 80%;
    outline: none;
    border: 2px solid #01CB63;
    font-style: italic;
    background: #F8F9FB;
    margin: 2rem;
    padding: 1rem;
}

.form button {
    border: none;
    outline: none;
    width: 8rem;
    height: auto;
    background-color: #1F2532;
    color: white;
    padding: 0.6vmax;
    font-size: 1.2rem;
    font-style: italic;

}

img {
    transform: scale(0.8);
}

@media only screen and (max-width: 600px) {
    .container {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        padding: 1vmax;
    }

    .info>div {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
    }

    img {
        transform: scale(0.5);
    }

    input {
        font-size: 4vw;
    }
    .form textarea {
    width: 60%;
    }
  
}
</style>
