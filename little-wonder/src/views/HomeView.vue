<template>
  <div>
    <div style="position: relative; display: inline-flex; width: 100%;">
      <img alt="Vue logo" style="width: 100%;height: 500px ;margin-top: -37px;" src="../assets/pngegg.png">
      <v-carousel cycle hide-delimiters show-arrows-on-hover class="carousel" style="      height: 248px;">
        <v-carousel-item src="../assets/UN0292170_0.jpeg" cover> </v-carousel-item>
        <v-carousel-item src="../assets/stringio.jpeg" cover></v-carousel-item>
      </v-carousel>
    </div>
    <div>
      <div style="background-color: #DEB887; width: 100%; height: 30%; padding-bottom: 20px; font-size: 20px;">
        <h3 style="    padding-top: 20px; padding-bottom: 20px;">Little Wonders has provided great education for the past
          many years. Pupils have been prepared to face the world through quality education, activities that will help
          them to discover with accuracy and innovativeness in life</h3>
        <v-btn style="background-color: #DAA520; " color="primary" elevation="2" large
          @click="$router.push('/about')">Read More</v-btn>
      </div>
    </div>
    <div>
      <br>
      <div class="menu-bar">
        <div id="col-yellow">
          <div id="ladybug"></div>
          <!--<h2>About us</h2>
						<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut.</p>
            <v-btn style="background-color: #DAA520; " color="primary" elevation="2" large>Read More</v-btn>
						<div class="clearfix"><br></div>-->
          <h2>Working Hours</h2>
          <br>
          <p>Nursery: 9 - 11 am <br>
            Junior kg: 9 - 12 pm <br>
            Playgroup: 11:30 - 1:30 pm</p>
          <br>
          <v-btn style="background-color: #61cbe6; " color="primary" elevation="2" large  @click="$router.push('/mission')">SEE PROGRAM</v-btn>
        </div>
        <div id="col-yellow">
          <div id="butterfly"></div>
          <h2> Why choose us</h2>
          <br>
          <p>The school provides a separate library in each classroom. Interactive boards linked to the school server are
            provided in the classroom. The interactive board helps the students to understand the concepts through video
            clippings that help the teachers to explain easily to the students.</p>
          <br>
          <!--<v-btn style="background-color: #61cbe6; " color="primary" elevation="2" large
            @click="$router.push('/mission')">Read More</v-btn>-->
        </div>
      </div>

    </div>
    <div>
      <img alt="Vue logo" style="width: 108%; height: 67px; margin-bottom: -48px;
        left: 2px;
        margin-left: -40px;" src="../assets/grass cartoon png transparent.png">
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'HomeView',
  components: {
  }
}
</script>
<style>
.v-window__next {
  margin-left: 94%;
}

.carousel {
  height: 248px;
  position: absolute;
  width: 50%;
  z-index: 2;
  margin-top: 99px;
  margin-left: 22%;
}

#col-yellow {
  background: #efc043;
  border-color: #f29f34;
}

#col-yellow,
#col-green,
#col-orange {
  border-radius: 4px;
  border-width: 5px 0 24px 0;
  border-style: solid;
  padding: 15px 25px 25px 25px;
  position: relative;
  margin-bottom: 20px;
  width: 50%;
  margin-right: 20px;
  margin-left: 20px;
}

button.blue {
  background-color: #61cbe6;
}

.button {
  border-radius: 4px;
  box-shadow: 1px 1px 0 #7d7d7d;
  padding: 7px 10px;
  color: #fff;
  margin-bottom: 20px;
}

h2 {
  font: 28px 'dimbo-regular', 'Fira Sans', sans-serif;
  line-height: 30px;
  color: #fff;
}

.menu-bar {
  display: flex;
  width: 100%
}

#ladybug {
  width: 58px;
  height: 37px;
  background: url(../assets/ladybug.png) no-repeat;
  background-size: cover;
  position: absolute;
  top: -42px;
  left: 30px;
}

#butterfly {
  width: 63px;
  height: 57px;
  background: url(../assets/butterfly.png) no-repeat;
  background-size: cover;
  position: absolute;
  top: -40px;
  left: -30px;
}

@media screen and (max-width: 600px) {
  #col-yellow {
    width: 100%;
    margin-right: 0px;
    margin-left: 0px;
    /* The width is 100%, when the viewport is 800px or smaller */
  }

  .menu-bar {
    display: block;
    width: 100%
  }
}</style>
