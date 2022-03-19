<template>
  <div class="Info">
    <div class="left">
      <div class="left-info">
        <div class="picture">
          <img src="./assets/jim.png" width="100%" height="100%">
        </div>
          <h3>Jim Charles M. Morales</h3>
      </div>

      <div class="contactInfo"></div>
        <h4 class="information"> Personal information</h4>
        <ul class="contact">
          <li>Name: Jim Charles M. Morales</li>
          <li>Age : 20</li>
          <li>Birthday : August 15, 2001</li>
          <li>Address : 43 Gordon st. New Banicain, Olongapo City</li>
        </ul>

        <div class="contactInfo"></div>
          <h4 class="information"> Contact information</h4>
          <ul class="contact">
            <li>Email : jimcharlesmorales15@gmail.com</li>
            <li>School Email : jmmorales@student.hau.edu.ph</li>
            <li>Contact No. : 09255064484</li>
          </ul>

        </div>

        <div class="right">
          <div class="about">
            <h2 class="title">Who is Jim Charles?</h2>
              <about-me></about-me>
          </div>
          <br>
          <div class="Skills">
              <h2 class="title">Skills</h2>
                <skills></skills>
          </div>
          <br>
          

            </div>
        </div>
</template>

<script>
//------------Imports--------------//
import AboutMe from './AboutMe.vue'
import Skills from './skills.vue'
//---------------------------------//
export default {
  //--------Components---------//
  components: { 
    AboutMe,
    Skills,
   
    
  },

  name: 'app',
  data () {
    return {
      msg: ''
    }
  }
}
</script>

<style>
*
{
    margin: 0;
    padding: 0;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}

body {
    background-color: rgb(255, 255, 255);
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
}

.Info {
    position: relative;
    width: 100%;
    max-width: 1000px;
    min-height: 1000px;
    margin: 50px;
    background-color: rgb(250, 250, 250);
    display: grid;
    grid-template-columns: 1fr 2fr;
    box-shadow: 0 35px 55px rgb(255, 255, 255);
}
/***************************************************/
.Info .left {
    position: relative;
    background: brown;
    padding: 40px;
}

.left-info{
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-bottom: 20px;
    border-bottom: 2px solid black;
}

.picture {
    position: relative;
    width: 200px;
    height: 200px;
    border-radius: 45%;
    overflow: hidden;
}

.left-info h3 {
    color: white;
    font-size: 1.5em;
    margin-top: 20px;
    text-transform: uppercase;
    text-align: center;
    font-weight: 600;
    line-height: 1.4em;
}

.contactInfo {
    padding-top: 40px;
}

.contact {
    color: white;
    font-weight: 300;
    font-size: 18px;
    display: inline-block;
    
}

.information {
    color: white;
    text-transform: uppercase;
    font-weight: 600;
    letter-spacing: 1px;
    margin-bottom: 20px;

}
/***************************************************/
.Info .right {
    position: relative;
    background: turquoise;
    padding: 40px;
}

.about {
    margin-bottom: 50px;
}

.title {
    color: whitesmoke;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 10px;
}

p {
    color: rgb(255, 253, 248);
}

ul {
    font-size: 20px;
    color: whitesmoke;
    font-weight: 300;
    letter-spacing: 1px;
    margin-bottom: 20px;
}
</style>
