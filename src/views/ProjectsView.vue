<template>
  <div id="Projects">
    <div class="container">
      <div class="row">
        <div class="projects">
          <div class="col-md-12" id="projectsContent">
            <h2>Projects</h2>
            <p>Top 5 Best Projects</p>
            <div class="card">
              <div class="content">
                <div class="front"><p>project 1: My Holiday Adventure</p></div>
                <div class="back">
                <p>http://127.0.0.1:5502/index.html</p></div>
              </div>
            </div>
            <div class="card">
              <div class="content">
                <div class="front"><p>project 2: Cultural Cuisine (Group)</p></div>
                <div class="back"><p>"https://github.com/AbuBakrKhan24/Project_1.git"</p>
                <p>"https://comfy-axolotl-4c4a89.netlify.app"</p></div>
              </div>
            </div>
            <div class="card">
              <div class="content">
                <div class="front"><p>project 3: End Of Module King</p></div>
                <div class="back"><p>http://127.0.0.1:5501/index.html</p>
                <p></p></div>
              </div>
            </div>
            <div class="card">
              <div class="content">
                <div class="front">
                  <p>project 4: Mental Health Blog Site (Group)</p>
                </div>
                <div class="back"><p></p>
                <p></p></div>
              </div>
            </div>
            <div class="card">
              <div class="content">
                <div class="front"><p>project 5: Project WYZE</p></div>
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
  margin-top: 3rem;
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
@media screen and(max-width:790) {
  #projectContent {
    max-width: 500px;
  }
  .content {
    width: 100%;
    font-size: 12px;
    overflow:hidden;
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
  background: white;
  line-height: 50px;
  color: #03446a;
  text-align: left;
  font-size: 20px;
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
</style>
