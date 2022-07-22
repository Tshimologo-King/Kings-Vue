<template>
  <div id="landing">
    <div class="container">
      <h1 style="color: white">Tshimologo King Mabena</h1>
      <div class="row">
        <div class="three_kings">
          <div class="aboutCard" style="margin: 5px">
            <router-link to="/about">
              <img src="https://picsum.photos/100" alt="" />
            </router-link>
          </div>
          <div class="projectCard" style="margin: 5px">
            <router-link to="/projects">
              <img src="https://picsum.photos/100" alt="" />
            </router-link>
          </div>
          <div class="testimonialCard" style="margin: 5px">
            <router-link to="/testimonials">
              <img src="https://picsum.photos/100" alt="" />
            </router-link>
          </div>
          <div class="contactCard" style="margin: 5px">
            <router-link to="/contact">
              <img src="https://picsum.photos/100" alt="" />
            </router-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#landing {
  background-color: black;
  height: 100vh;
  width: 100%;
}
h1 {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}

.three_kings {
  color: black;
  position: absolute;
  bottom: -40px;
  margin-inline: auto;
  display: flex;
  justify-content: space-evenly;
  width: 100%;
  flex-wrap: wrap;
}

.three_kings img {
  max-width: 250px;
  height: 100%;
}

.aboutCard,
.projectCard,
.testimonialCard,
.contactCard {
  width: auto;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  transform: scale(1.2) translate(1rem, 0) skew(-8deg, -4deg);
  margin-right: 10px;
}
.aboutCard {
  box-shadow: 29px 29px 58px #101ad6, -29px -29px 58px #3598ca;
}
.projectCard{
  box-shadow: 29px 29px 58px #cef700, -29px -29px 58px #dcca71;
}
.testimonialCard{
  box-shadow: 29px 29px 58px #b93939, -29px -29px 58px #ff0000;
}
.contactCard{
box-shadow: 29px 29px 58px #0c9111, -29px -29px 58px #5dff52;}

.aboutCard img:hover {
  padding: 5px;
  height: 100%;
  z-index: 100;
}
.projectCard img:hover {
  padding: 5px;
  height: 100%;
  transform: scale(1.1);
  z-index: 100;
}
.testimonialCard img:hover {
  padding: 5px;
  height: 100%;
  transform: scale(1.1);
  z-index: 100;
}
.contactCard img:hover {
  padding: 5px;
  height: 100%;
  transform: scale(1.1);
  z-index: 100;
}
</style>
