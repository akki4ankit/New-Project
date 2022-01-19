<template>
  <div id="app" style="backgroundColor:black">
    <!--  <h1>{{ msg }}</h1> -->

     <div id ="center">
        <!-- <img src="./assets/userimage.png" > -->
        <EmployeeList />
     </div>
     <div class="container">
          <MicroPhoneOffIcon :size="40" style="color:#fff; "/>
          <VideoOffOutlineIcon :size="40" style="color:#fff"/>
          <PhoneHangUpIcon :size="40" style="color:#fff" />
          <CogIcon :size="40" style="color:#fff" />

        </div>
      <VideoOffOutlineIcon :size="40" style="color:#fff" paddingTop="10px" />
      <MicroPhoneIcon :size="40" style="color:#fff" paddingTop="10px"/>

  </div>
</template>

<script>
import Home from './components/Home.vue'
import Form1 from  './components/Form1.vue'
import UI from './components/UI.vue'
import VideoOffOutlineIcon from 'vue-material-design-icons/VideoOffOutline.vue'
import MicroPhoneIcon from 'vue-material-design-icons/MicroPhone.vue'
import MicroPhoneOffIcon from 'vue-material-design-icons/MicroPhoneOff.vue'
import PhoneHangUpIcon from 'vue-material-design-icons/PhoneHangUp.vue'
import CogIcon from 'vue-material-design-icons/Cog.vue'
import EmployeeList from './components/EmployeeList.vue'

export default {
  components: { Home,Form1,UI,VideoOffOutlineIcon,MicroPhoneIcon,MicroPhoneOffIcon,PhoneHangUpIcon,CogIcon,EmployeeList },
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'

    }
  }
}
</script>

<style>
*{
  padding:0 !important;
  margin:0 !important;
  box-sizing: border-box;


}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #502c40;
  margin-top: 50px;
  padding: 0;
  margin: 0;
  width: 100%;
  min-height: 100vh;
  text-align: end;

}

img{
height: 250px;
width: 250px;
border-radius: 50%;
}

#center {
  text-align: center;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 18px;
}
.container {

  width: 1240px;
  height: 60px;
  border: 1px ;
  box-sizing: border-box;
  background-color: #383637;
  position: absolute;
  bottom: 0px;
  text-align: center;
  word-spacing: 30px;
  padding-top: 100px;
}

</style>
