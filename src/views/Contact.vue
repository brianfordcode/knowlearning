<template>
<div class="container">

  <div class="text-wrapper">
    <p class="title">Contact Us!</p>
    <p class="text">KnowLearning invites you to contact us if you are interested in our services, want to participate or contribute, have a question, or have something interesting to share.</p>
  </div>

  <form ref="form" @submit.prevent="sendEmail">
    <div>
        <input placeholder="Name" type="text" name="user_name" v-model="user_name" required>
    </div>
    
    <div>
        <input placeholder="Email" type="email" name="user_email" v-model="user_email" required>
    </div>
    
    <div>
        <textarea placeholder="Message" name="message" class="text-area" v-model="message" required></textarea>
    </div>
    
    <input class="send-btn" type="submit" value="Send" >
    <div class="success" v-if="success">Message Has Been Sent!</div>
    
  </form>

</div>
</template>

<script>
import emailjs from 'emailjs-com';
export default {
    data() {
        return {
            user_name: '',
            user_email: '',
            message: '',
            success: false
        }
    },
  methods: {
    sendEmail() {
        emailjs.sendForm('service_6m1g8u1', 'template_orguy3b', this.$refs.form, 'user_6KhsAEBx838OAJBfNW81i')
            .then((result) => {
                console.log('SUCCESS!', result.text);
            }, (error) => {
                console.log('FAILED...', error.text);
            });
            setTimeout(()=> {
                this.user_name = ''
                this.user_email = ''
                this.message = ''
                this.success = true
            }, 900)
            }
  }
}
</script>

<style scoped>

  .container {
      display: flex;
      margin: 0 auto;
      align-items: flex-start;
      justify-content: space-around;
      max-width: 900px;
      padding: 100px 50px 100px 50px;
      min-height: calc(100vh - 328px);
  }

  .title {
      font-size: 36px;
      padding-bottom: 20px;
  }

  p {
      width: 80%;
      font-size: 18px
  }

  form {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      width: min-content;
      height: min-content;
      /* border: 1px solid black; */
      color: white;
  }

  form div {
      display: flex;
      flex-direction: column;
      margin-bottom: 15px;
  }

  form div input {
      width: 400px;
      padding: 15px;
      border: none;
      outline: none;
      font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  }

  input {
      border-radius: 10px;
      box-shadow: 0px 0px 33px -20px #000000;
  }

  .text-area {
      box-shadow: 0px 0px 33px -20px #000000;
      border-radius: 10px;
      min-width: 400px;
      max-width: 100px;
      max-height: 300px;
      min-height: 100px;
      outline: none;
      padding: 15px;
      border: none;
      font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  }

  .send-btn {
      padding: 10px 30px;
      font-size: 15px;
      border: none;
      color: black;
      cursor: pointer;
      transition: .15s ease-in-out;
      margin-top: 5px;
  }

  .send-btn:hover {
      transform: scale(1.1);
    }

    .success {
        color: black;
        margin: 0 auto;
        padding: 10px;
    }

    @media screen and (max-width: 768px) {

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
            padding: 30px 50px 50px 50px;
            min-height: calc(100vh - 208px);
        }

        .title {
            padding-bottom: 10px;
        }

        p {
            width: 100%;
        }

        .text-wrapper {
            margin-bottom: 20px;
            text-align: center;
        }

        form div input {
            width: 200px;
        }

        .text-area {
            min-width: 200px;
            max-width: 200px;
            max-height: 100px;
            min-height: 100px;
        }
    }
</style>