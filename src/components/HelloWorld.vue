<template>
  <div id="landing">
    <div class="container">
      <h1 style="color: white">Tshimologo King Mabena</h1>
      <div class="row">
        <div class="three_kings">
          <div class="aboutCard" style="margin:5px">
            <router-link to="/about">
              <img src="https://picsum.photos/100" alt=""/>
            </router-link>
          </div>
          <div class="projectCard" style="margin: 5px;">
            <router-link to="/projects">
              <img src="https://picsum.photos/100" alt=""/>
            </router-link> 
          </div>
          <div class="testimonialCard" style="margin: 5px;">
          <router-link to="/testimonials">
              <img src="https://picsum.photos/100" alt=""/>
            </router-link> 
          </div>
          <div class="contactCard" style="margin: 5px;">
          <router-link to="/contact">
              <img src="https://picsum.photos/100" alt=""/>
            </router-link> 
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#landing{
  background-image: url(../assets/blank.jpg);
  background-position: center;
  background-size: cover;
  height: 100vh;
  width: 100%;
  margin-inline: auto;
}


.three_kings {
  color: black;
  position: absolute;
  bottom: -70px;
  margin-inline: auto;
  display: flex;
  justify-content: space-evenly;
  width: 100%;
  flex-wrap: wrap;
}

.three_kings img{
  min-width: 200px;
  max-width: 400px;
  height: 100%;
}

.aboutCard, .projectCard, .testimonialCard, .contactCard{
border-radius: 32px;
background: #616161;
box-shadow:  29px 29px 58px #2c2c2c,
             -29px -29px 58px #969696;
}

.aboutCard img:hover{
  border: 1px solid yellow;
  padding: 5px;
  height: 100%;
  transform: scale(1.1);
}
.projectCard img:hover{
  border: 1px solid yellow;
  padding: 5px;
  height: 100%;
  transform: scale(1.1);
}
.testimonialCard img:hover{
  border: 1px solid yellow;
  padding: 5px;
  height: 100%;
  transform: scale(1.1);
}
.contactCard img:hover{
  border: 1px solid yellow;
  padding: 5px;
  height: 100%;
  transform: scale(1.1);
}






</style>
