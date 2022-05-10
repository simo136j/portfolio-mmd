<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/portfolio-logo.png" style="height: 60px;">
    <HelloWorld msg=""/>


  <p-1>Om mig:</p-1>
  <div class="om-mig">
    <img src="../assets/cv-billede.jpg" alt="" style="height: 500px;">
    <p-11>Mit navn er Simone, og jeg er 20 år gammel. Jeg bor i Esbjerg, og til dagligt studerer jeg Multimediedesign på Erhvervsakademi Sydvest. I min fritid kan jeg godt lide at tegne, specielt fotorealistiske farvetegninger, eller læse en god bog. Jeg har et bredt interessefelt, og derfor læser jeg meget forskelligt – både faglitteratur og skønlitteratur.</p-11>
  </div>

  <p-2>Art:</p-2>
  <div class="art">
    <img src="../assets/lemons.jpeg" alt="" style="height: 500px">
    <p-21>✨Lemons 🍋✨</p-21>
    <img src="../assets/happyholidays.jpeg" alt="" style="height: 500px">
    <p-22>✨Happy Holidays ✨</p-22>
  </div>

  <p-3>Photography:</p-3>
  <div class="photography">
    <img src="../assets/city-lights.jpg" alt="" style="height: 500px;">
    <p-31>City Lights.</p-31>
    <img src="../assets/michele1.jpg" alt="" style="height: 250px;">
    <img src="../assets/michele2.jpg" alt="" style="height: 250px;">
    <p-32>Michele.</p-32>
  </div>

  <div class="videoCV">
    <p-4>CV:</p-4>
   <!--  <iframe width="100%" height="500"
    src="https://youtu.be/ghKWkfOOVXA" frameborder="0">
    </iframe> -->

    <video src="https://youtu.be/ghKWkfOOVXA" controls>
    <source :src="videoCV" type="video/mp4">
    </video>
    <img src="../assets/cv.jpg" alt="" style="height: 700px">
  </div>

  <div class="cv">
    <img src="" alt="" style="height">
  </div>

  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import {ref} from "vue"

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },

  setup () {
    let videoCV = ref("https://youtu.be/ghKWkfOOVXA")
    
    return {
      videoCV
    }
  }
}
</script>

<style lang="scss">

body{
  background-color: #F5F5DC;
}

.home{
  background-color: white;
  margin-top: 20px;
  margin-left: 20px;
  margin-right: 20px;
  margin-bottom: 20px;
  padding-left: 200px;
  padding-right: 200px;
  padding-bottom: 100px;
}

img{
  margin-top: 5px;
}

p-1{
  font-size: 25px;
  color: black;
  display: flex;
  margin-top: 50px;
  justify-content: center;
}

p-11{
  color: black;
  display: flex;
  width: 495px;
  margin-bottom: 70px;
}

.om-mig{
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  align-items: center;
}

p{
  display: flex;
  color: black;
}

p-2{
  font-size: 25px;
  color: black;
  margin-top: 50px;
}

p-21{
  color: black;
  margin-bottom: 25px;
}
p-22{
  margin-bottom: 70px;
  color: black;
}

.art{
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  align-items: center;
}

p-3{
  font-size: 25px;
  color: black;
  margin-top: 50px;
}

p-31{
  display: flex;
  margin-right: 296px;
  margin-bottom: 25px;
  color: black;

}

p-32{
  display: flex;
  margin-right: 317px;
  color: black;
}

.photography{
  display: flex;
  flex-direction: column;
  align-items: center;
}

p-4{
  font-size: 25px;
  color: black;
  margin-top: 50px;
}

.videoCV{
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 25px;
}

video {
  width: 600px;
  height: 360px;
  display: flex;

  
}




@media only screen and (max-width: 600px) {

}
</style>
