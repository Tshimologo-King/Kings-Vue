<template>
  <div id="Testimonial">
    <h2>Testimonials</h2>
    <div class="container">
      <div class="row">
        <div class="testimonials">
          <div class="card">
            Jason Wandrag
            <img src="https://picsum.photos/200/300?random=98" alt="" />
            <p class="TestimonialText">
              Lorem ipsum dolor sit amet consectetur, adipisicing elit.
            </p>
          </div>
          <div class="card">
            Ms Moritz
            <img src="https://picsum.photos/200/300?random=12" alt="" />
            <p class="TestimonialText">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
            </p>
          </div>
          <div class="card">
            Mr Khan
            <img src="https://picsum.photos/200/300?random=14" alt="" />
            <p class="TestimonialText">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </div>
          <div class="card">
            Ms Mntungwa
            <img src="https://picsum.photos/200/300?random=21" alt="" />
            <p class="TestimonialText">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </div>
          <div class="card">
            Mr G
            <img src="https://picsum.photos/200/300?random=23" alt="" />
            <p class="TestimonialText">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="navigationLinks">
        <div class="pageLinkPrev">
          <router-link to="/projects">
            <button>Projects</button>
          </router-link>
        </div>
        <div class="pageLinkNext">
          <router-link to="/contact">
            <button>Contact</button>
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

#Testimonial {
  height: 100vh;
  background-color: black;
  color: white;
}

.container {
  margin-inline: auto;
  position: absolute;
  top: 50%;
  left: 7%;
}

.testimonials {
  width: 100%;
  height: 100%;
  padding: 10px;
  border-radius: 10px;
  border: 1px solid white;
  margin-top: 100px;
  box-shadow: 5px 5px 5px grey;
  display: flex;
  justify-content: space-evenly;
}

.card {
  color: white;
  margin: 10px;
  padding: 10px;
  background-color: transparent;
  border-bottom: 1px solid white;
  border-left: 1px solid white;
  text-align: left;
  flex-grow: 1;
  transition: all 0.3s linear;
  flex-basis: 0;
}

.card img {
  max-width: 100px;
  max-height: 100px;
  transition: 1.5s ease-in-out;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 6px 12px -2px,
    rgba(0, 0, 0, 0.3) 0px 3px 7px -3px;
  border: 5px solid #fff;
}

.TestimonialText {
  display: none;
}

.card:hover {
  flex-basis: 5%;
  flex-grow: 1;
}
.card:hover .TestimonialText {
  display: block;
}

.card_one {
  border-radius: 15px 0 0 15px;
}

.card_five {
  border-radius: 0 15px 15px 0;
}
.navigationLinks{
  position: absolute;
  top: 100%;
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
