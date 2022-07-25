<template>
  <div id="Projects">
    <div class="container">
      <div class="row">
        <div class="projects">
          <h1>Projects</h1>
          <div class="col-md-12" id="projectsContent">
            <h2>Projects</h2>
            <p>Top 5 Best Projects</p>
            <div class="card">
              <div class="content">
                <div class="front"><p>Project 1: My Holiday Adventure</p></div>
                <div class="back">
                <p>http://127.0.0.1:5502/index.html</p></div>
              </div>
            </div>
            <div class="card">
              <div class="content">
                <div class="front"><p>Project 2: Cultural Cuisine (Group)</p></div>
                <div class="back"><p>"https://github.com/AbuBakrKhan24/Project_1.git"</p>
                <p>"https://comfy-axolotl-4c4a89.netlify.app"</p></div>
              </div>
            </div>
            <div class="card">
              <div class="content">
                <div class="front"><p>Project 3: End Of Module King</p></div>
                <div class="back"><p>http://127.0.0.1:5501/index.html</p>
                <p></p></div>
              </div>
            </div>
            <div class="card">
              <div class="content">
                <div class="front">
                  <p>Project 4: Mental Health Blog Site (Group)</p>
                </div>
                <div class="back"><p></p>
                <p></p></div>
              </div>
            </div>
            <div class="card">
              <div class="content">
                <div class="front"><p>Project 5: Project WYZE</p></div>
                <div class="back"><p>Coming Soon...</p></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="navigationLinks">
      <div class="pageLinkPrev">
        <router-link to="/about">
          <button>About</button>
        </router-link>
      </div>
      <div class="pageLinkNext">
        <router-link to="/testimonials">
          <button>Testimonials</button>
        </router-link>
      </div>
    </div>
  </div>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#Projects {
  height: 100vh;
  width: 100%;
  background-color: black;
}
h1 {
  color: black;
  text-shadow: -1px -1px 0 rgb(238, 238, 39), 1px -1px 0 rgb(139, 126, 45), -1px 1px 0 rgb(229, 229, 131), 1px 1px 0 rgb(188, 155, 11);
  font-size: 5rem;
  display: flex;
  margin-inline: auto;
}

h2{
  animation: pulsate 2.5s infinite alternate
}

.projects {
  display: flex;
  justify-content: flex-end;
  align-content: flex-end;
  margin-top: 50px;
}
#projectsContent {
  color: white;
  background-color: rgb(10, 10, 10);
  width: 400px;
  gap: 40px;
  padding: 20px;
  border-radius: 32px;
  background: #333333;
  box-shadow: 29px 29px 58px #faff5a, -29px -29px 58px #ddff00;
  margin-top: 10rem;
  margin-inline: auto;
}

@media screen and (max-width: 1400px) {
  #projectContent {
    max-width: 500px;
    max-height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 5px;
    margin: 2px;
  }
  .content {
    width: 100%;
    font-size: 12px;
  }
}
@media screen and(max-width:700) {
  #projectContent {
    max-width: 500px;
    margin-top: 2rem;
  }
  .content {
    width: 100%;
    font-size: 12px;
    overflow:hidden;
  }
  .card{
    margin-top: 2rem;
  }
}

.card {
  width: 100%;
  height: 50px;
  perspective: 500px;
  margin-inline: auto;
  margin: 10px;
}

.content {
  max-width: 500px;
  height: 100%;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
  transition: transform 1s;
  transform-style: preserve-3d;
}

.card:hover .content {
  transform: rotateY(180deg);
  transition: transform 0.5s;
}

.front,
.back {
  position: absolute;
  height: 100%;
  width: 100%;
  background: rgb(0, 0, 0);
  line-height: 50px;
  color: #feffa5;
  text-align: left;
  font-size: 14px;
  border-radius: 5px;
  backface-visibility: hidden;
}

.back {
  background: #000000;
  color: white;
  transform: rotateY(180deg);
}
.back p{
  color: #ddff00;
  font-size: 10px;
}
.navigationLinks {
  position: absolute;
  top: 98%;
  width: 100%;
  display: flex;
  justify-content: space-between;
  margin-top: 2rem;
  padding: 10px;
}
.pageLinkPrev button {
  padding: 5px 10px;
  border-radius: 25px;
}
.pageLinkNext button {
  padding: 5px 10px;
  border-radius: 25px;
}

@keyframes pulsate {
  100% {
    /* Larger blur radius */
    text-shadow:
      0 0 4px #fff,
      0 0 11px #fff,
      0 0 19px #fff,
      0 0 40px rgb(255, 247, 0),
      0 0 80px rgb(251, 192, 54),
      0 0 90px rgb(227, 248, 43),
      0 0 100px rgb(240, 245, 90),
      0 0 150px rgb(255, 234, 0);
  }
  0% {
    /* Smaller blur radius */
    text-shadow:
      0 0 2px #fff,
      0 0 4px #fff,
      0 0 6px #fff,
      0 0 10px rgb(173, 175, 18),
      0 0 45px rgb(139, 139, 7),
      0 0 55px rgb(253, 255, 137),
      0 0 70px rgb(199, 221, 54),
      0 0 80px rgb(225, 255, 2);
  }
}
</style>
