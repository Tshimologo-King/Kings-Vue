<template>
    <div id="Projects">
        <div class="container">
            <div class="row">
                <div class="projects">
                    <div class="col-md-4" id="projectsContent">
                            <h2>Projects</h2>
                            <p>Top 5 Best Projects</p>
                            <div class="card">
                                <div class="content">
                                    <div class="front">
                                        project 1: My Holiday Adventure
                                    </div>
                                    <div class="back">
                                        Lorem
                                    </div>
                                </div>
                            </div>
                            <div class="card">
                                <div class="content">
                                    <div class="front">
                                        project 2: Cultural Cuisine (Group)
                                    </div>
                                    <div class="back">
                                        Lorem
                                    </div>
                                </div>
                            </div>
                            <div class="card">
                                <div class="content">
                                    <div class="front">
                                        project 3: End Of Module King
                                    </div>
                                    <div class="back">
                                        Lorem
                                    </div>
                                </div>
                            </div>
                            <div class="card">
                                <div class="content">
                                    <div class="front">
                                        project 4: Mental Health Blog Site (Group)
                                    </div>
                                    <div class="back">
                                        Lorem
                                    </div>
                                </div>
                            </div>
                            <div class="card">
                                <div class="content">
                                    <div class="front">
                                        project 5: Project WYZE
                                    </div>
                                    <div class="back">
                                        Lorem
                                    </div>
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
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

#Projects{
    height: 100vh;
    width: 100%;
    background-color: black;
}

.projects{
    display: flex;
    justify-content: flex-end;
    align-content: flex-end;
    margin-top: 50px;
}
#projectsContent{
    color: white;
    background-color: rgb(10, 10, 10);
    padding: 5px;
    display: flex;
    flex-direction: column;
    gap: 40px;
    padding: 20px;
    border-radius: 32px;
    background: #333333;
    box-shadow:  29px 29px 58px #2c2c2c,-29px -29px 58px #969696;
}

.card{
    width: 400px;
    height: 50px;
    perspective: 500px;
    margin-inline: auto;
}

.content {
  width: 100%;
  height: 100%;
  box-shadow: 0 0 15px rgba(0,0,0,0.1);
  transition: transform 1s;
  transform-style: preserve-3d;
}


.card:hover .content{
  transform: rotateY( 180deg ) ;
  transition: transform 0.5s;
}


.front,
.back {
  position: absolute;
  height: 100%;
  width: 100%;
  background: white;
  line-height: 50px;
  color: #03446A;
  text-align: center;
  font-size: 20px;
  border-radius: 5px;
  backface-visibility: hidden;
}

.back{
  background: #03446A;
  color: white;
  transform: rotateY( 180deg );
}
.navigationLinks{
  position: absolute;
  top: 98%;
  width: 100%;
  display: flex;
  justify-content: space-between;
  margin-top: 2rem;
  padding: 10px;
}
.pageLinkPrev button{
  padding: 5px 10px;
  border-radius: 25px;
}
.pageLinkNext button{
  padding: 5px 10px;
  border-radius: 25px;
}


</style>