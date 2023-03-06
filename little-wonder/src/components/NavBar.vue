<template>
 <div>
    <img src="../assets/Logo Little Wonders.png" class="train-png" @click="$router.push('/home')"> 
    <div class="topnav" id="myTopnav">
        <router-link to="/contact">Contact</router-link>

        <router-link to="/about">About</router-link>
        <router-link to="/home">Home</router-link>
    </div>
    <img src="../assets/PngItem_45261.png" class="monkey-png">
</div>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.monkey-png{
  width: 15%;
    height: 180px;
    float: right;
    position: absolute;
    z-index: 3;
    left: 86%;
}
.topnav {
  border-radius: 20px;
  background-color: #79443B;
  overflow: hidden;
  margin-top: 20px;
  z-index: 10;
  width: 75%;
  margin-left: 25%;
}

.train-png {
  width: 20%;
  height: 80px;
  float: left;
}

.topnav a {
  float: right;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 7%;
  text-decoration: none;
  font-size: 17px;
}

.topnav div {
  float: left;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;

}

.topnav a:hover {
  color: #efc043;
}

.topnav a.active {
  text-decoration: underline;
  color: white;
}

.topnav .icon {
  display: none;
}



</style>
