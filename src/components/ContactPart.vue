<template>
<div class="container">
    <div class="Info">
    <h4>Contact Information</h4>
        <div class="info1">
                <img src="../assets/Contact/Mail.png" alt="">
                <p>contact@coursepro.com</p>
          </div>

          <div class="info1">
                <img src="../assets/Contact/Telephone.png" alt="">
                <p>1800-562-895, 1800-869-877</p>
           </div>

           <div class="info1">
                <img src="../assets/Contact/Location.png" alt="">
                <p>102 Street, India</p>
        </div>
         <h4>Social Media Channel</h4>
        <div class="info2">
           
            
                <img src="../assets/SocialMedia/Facebook.svg" alt="">
                <img src="../assets/SocialMedia/Github.svg" alt="">
                <img src="../assets/SocialMedia/Linkedin.svg" alt="">
                <img src="../assets/SocialMedia/Twitter.svg" alt="">
           
        </div>
    </div>
    <div class="form">
        <p>Fill up the form and our team will get back to you within 24 hours</p>
        <form v-on:submit="SubmitForm">
            <div class="details1">
                <label for="name"></label>
                <input type="text" placeholder="Name" id="name">
                <label for="email"></label>
                <input name="email" :class="{ valid: isValidEmail, invalid: !isValidEmail}" v-model="email" type="email" id="email" placeholder="Email" @keyup=" ValidateEmail" />
                <div class="invalid-warning" v-if="!isValidEmail">
                    Invalid Email!
                </div>
                <label for="phoneNumber"></label>
                <input name="phoneNumber" :class="{ valid: isValidPhoneNumber, invalid: !isValidPhoneNumber }" v-model="phoneNumber" type="text" id="phoneNumber" placeholder="Phone Number" @keyup="validatePhoneNumber" />
                <div class="invalid-warning" v-if="!isValidPhoneNumber">
                    Invalid phone number!
                </div>
                <label for="subject"></label>
                <input type="text" placeholder="Subject" id="subject">

                <label for="message"></label>
                <textarea name="message" placeholder="Message" rows="5"></textarea>
            </div>
            <button type="submit" class="btn">Submit</button>
        </form>
    </div>
</div>
</template>

<script>
export default {
    name: 'ContactPart',
    data() {
        return {
            email: "",
            isValidEmail: true,
            phoneNumber: "",
            isValidPhoneNumber: true,
        };
    },
    validator() {
        return {
            name: {
                required: true,
            },
            email: {
                required: true,
                email: true
            },
            phoneNumber: {
                required: true,
                length: 10
            }
        }
    },
    methods: {
        validatePhoneNumber() {
            const validationRegex = /^\d{10}$/;
            if (this.phoneNumber.match(validationRegex)) {
                this.isValidPhoneNumber = true;
            } else {
                this.isValidPhoneNumber = false;
            }
        },
        ValidateEmail() {
            // eslint-disable-next-line
            var mailformat = /^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/;
            if (this.email.match(mailformat)) {
                this.isValidEmail = true;
            } else {

                this.isValidEmail = false;
            }
        },
        SubmitForm() {
            if (this.isValidEmail && this.isValidPhoneNumber) {
                alert("Form Submitted Successfully");
            } else {
                alert("Please enter valid details");
            }
        }
    },
}
</script>

<style scoped>
.container {
    width: auto;
    background: #F8F9FB;
    display: grid;
    grid-template-columns: 1fr 1fr;
    flex-wrap: wrap;
    padding: 0.5vmax;
}


.info1{
    align-items: center;
display: flex;
flex-wrap: wrap;
flex-direction: row;
}

p,
h4 {
    font-weight: bold;
}
h4{
    font-size: 1.5rem;
}
.invalid-warning {
    font-size: 1rem;
    color: red;
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
    font-size: 1rem;
}

.form textarea {
    width: 60%;
    outline: none;
    border: 2px solid #01CB63;
    font-style: italic;
    background: #F8F9FB;
    margin: 2rem;
    padding: 1rem;
    font-size: 1rem;
}

.form button {
    border: none;
    outline: none;
    width: 8rem;
    height: auto;
    background-color: #1F2532;
    color: white;
    padding: 0.8vmax;
    font-size: 1.2rem;
    font-style: italic;
    border-radius: 5px;

}

img {
    transform: scale(0.7);
}

@media only screen and (max-width: 600px) {
    .container {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        padding: 1vmax;
    }
    .info1{
         display: flex;
        flex-direction: column;
        flex-wrap: wrap;
    }
  
    .form input {
        font-size: 4vw;
    }

    .form textarea {

        font-size: 4vw;
    }

    .invalid-warning {
        margin: 1px;
        color: red;
         font-size: 4vw;
    }
    .info1 >p{
      font-size: 0.5rem;
    }

}
</style>
