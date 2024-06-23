<template>
  <v-row class="justify-center lee5" id="contact">
    <v-container>
      <v-col class="d-flex justify-center align-center">
        <v-card class="card" elevation="5">
          <v-card-item>
            <v-row class="card-div1 justify-space-between align-center">
              <v-col cols="5" class="contact-div col-12 col-md-5">
                <p class="contact-txt">CONTACT</p>
                <p class="talk mb-8">Let's talk</p>
                <div class="purple-div-ctn">
                  <div class="d-flex justify-start align-bottom mb-7">
                    <div class="contact-icon mr-5 ping">
                      <svg class="" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512" width="24px" ><!--!Font Awesome Free 6.5.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="#957cf2" d="M215.7 499.2C267 435 384 279.4 384 192C384 86 298 0 192 0S0 86 0 192c0 87.4 117 243 168.3 307.2c12.3 15.3 35.1 15.3 47.4 0zM192 128a64 64 0 1 1 0 128 64 64 0 1 1 0-128z"/></svg>
                    </div>
                    <div class="bsd-icon pt-4">
                      <p>Email Address</p>
                      <p>contact@web3learner.org</p>
                    </div>
                  </div>
                  <div class="d-flex justify-start align-bottom mb-7">
                    <div class="contact-icon mr-5 ping">
                      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" width="24px"><!--!Font Awesome Free 6.5.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="#957cf2" d="M48 64C21.5 64 0 85.5 0 112c0 15.1 7.1 29.3 19.2 38.4L236.8 313.6c11.4 8.5 27 8.5 38.4 0L492.8 150.4c12.1-9.1 19.2-23.3 19.2-38.4c0-26.5-21.5-48-48-48H48zM0 176V384c0 35.3 28.7 64 64 64H448c35.3 0 64-28.7 64-64V176L294.4 339.2c-22.8 17.1-54 17.1-76.8 0L0 176z"/></svg>
                    </div>
                    <div class="bsd-icon pt-4">
                      <p>Telephone</p>
                      <p>+234 123 4567 89</p>
                    </div>
                  </div>
                  <div class="d-flex justify-start align-bottom mb-7">
                    <div class="contact-icon mr-5 ping">
                      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" width="24px"><!--!Font Awesome Free 6.5.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="#957cf2" d="M164.9 24.6c-7.7-18.6-28-28.5-47.4-23.2l-88 24C12.1 30.2 0 46 0 64C0 311.4 200.6 512 448 512c18 0 33.8-12.1 38.6-29.5l24-88c5.3-19.4-4.6-39.7-23.2-47.4l-96-40c-16.3-6.8-35.2-2.1-46.3 11.6L304.7 368C234.3 334.7 177.3 277.7 144 207.3L193.3 167c13.7-11.2 18.4-30 11.6-46.3l-40-96z"/></svg>
                    </div>
                    <div class="bsd-icon pt-4">
                      <p>Our Location</p>
                      <p>Lagos State, Nigeria</p>
                    </div>
                  </div>
                </div>
              </v-col>
              <v-col cols="6" class="contact-us col-md-6 col-12 col-md-6">
                <div class="success" v-if="showSuccess"><p>Success!</p></div>
                <v-form>
                  <v-row class="justify-space-between align-center py-7">
                    <v-col cols="6">
                      <label for="First Name">First Name</label>
                      <input name="First Name" class="input" v-model="firstname"/>
                    </v-col>
                    <v-col cols="6">
                      <label for="Last Name">Last Name</label>
                      <input label="Last Name" class="input" v-model="lastname"/>
                    </v-col>
                  </v-row>
                  <v-row class="justify-space-between align-center py-7">
                    <v-col cols="6">
                      <label for="Email Address">Email Address</label>
                      <input name="Email Address" class="input" v-model="email" type="email"/>
                    </v-col>
                    <v-col cols="6">
                      <label for="Phone">Phone</label>
                      <input label="Phone" class="input" v-model="phone" type="tel"/>
                    </v-col>
                  </v-row>
                  <v-row class="justify-space-between align-center py-7">
                    <v-col cols="12">
                      <label for="Message">Message</label>
                      <textarea name="Message" class="input" v-model="message"/>
                    </v-col>
                  </v-row>
                  <v-row>
                    <v-col>
                      <v-btn class="btn" color="#6366f1" @click="submitForm">Send Message</v-btn>
                    </v-col>
                  </v-row>
                </v-form>
              </v-col>
            </v-row>
          </v-card-item>
        </v-card>
      </v-col>
    </v-container>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      firstname: '',
      lastname: '',
      email: '',
      phone: '',
      message: '',
      showSuccess: false
    }
  },
  methods: {
    submitForm(e) {
    e.preventDefault()
    this.showSuccess = true
    setTimeout(() => {
      this.showSuccess = false
    }, 3000);
    this.firstname = ''
    this.lastname = ''
    this.email = ''
    this.phone = ''
    this.message = ''
  },
  },
}
</script>

<style scoped>
.lee5 {
  padding: 5vh 0 15vh;
  background: #fff;
}
.card {
  background: #fff;
  border-radius: 30px;
  width: 100%;
  padding: 3vh 2vw;
}
.card-div1 {
  padding: 3vh 4vw;
}
.contact-div {
  background: #4f46e5;
  color: #fff;
  border-radius: 25px;
  padding: 5vh 3vw;
}
.contact-txt {
  font-size: 1.1em;
}
.talk {
  font-size: 2.5em;
  font-weight: 700;
  padding: 0;
  margin: 0;
}
.contact-icon {
  border: 1px solid #fff;
  /* z-index: 10; */
  width: 60px;
  height: 60px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
}
.bsd-icon p:first-child {
  font-size: 1.7em;
  font-weight: 700;
  line-height: 4px;
}
.input{
  border-bottom: 1px solid #c1c3c5;
  display: block;
  width: 100%;
  outline: none;
}
.contact-us {
  color: #374151;
  /* background-color: #000000 !important; */
}
.btn {
  color: #fff;
}
.success {
  background: rgb(80, 109, 36);
  color: #fff;
  width: fit-content;
  margin-left: auto;
  padding: 2vh 2vw 0.5vh;
  font-weight: bold;
}
@media screen and (max-width: 768px) {
    .contact-icon {
      display: none;
    }
  }
@media screen and (max-width: 590px) {
  .card-div1 {
    flex-direction: column;
  }
  .contact-div {
    flex-basis: 100%;
    width: 100%;
  }
  .purple-div-ctn {
    display: flex;
    flex-direction: row;
    flex-flow: wrap;
  }
  .purple-div-ctn > div {
    flex-basis: 50%;
  }
}
@media screen and (max-width: 400px) {
.purple-div-ctn > div {
    flex-basis: 100%;
  }
}
</style>