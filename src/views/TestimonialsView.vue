<template>
  <div id="Testimonial">
    <h1>Testimonials</h1>
    <div class="container">
      <div class="row">
        <div class="testimonials">
          <div class="card">
            Mr Wandrag
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
            <img src="https://picsum.photos/200/300?random=20" alt="" />
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
          <div class="card">
            Mr Goliath
            <img src="https://picsum.photos/200/300?random=24" alt="" />
            <p class="TestimonialText">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </div>
        </div>
        <marquee behavior="scroll" direction="left" style="margin-top: 1rem;">
          <img src="https://picsum.photos/200/300?random=98" alt="Mr Wandrag" width="100" height="100">
          <img src="https://picsum.photos/200/300?random=8" alt="Mr Wandrag" width="100" height="100">
          <img src="https://picsum.photos/200/300?random=9" alt="Mr Wandrag" width="100" height="100">
          <img src="https://picsum.photos/200/300?random=1" alt="Mr Wandrag" width="100" height="100">
          <img src="https://picsum.photos/200/300?random=14" alt="Mr Wandrag" width="100" height="100">
          <img src="https://picsum.photos/200/300?random=12" alt="Mr Wandrag" width="100" height="100">
        </marquee>
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
  top: 49.5%;
  left: 4.5%;
}

.testimonials {
  width: 100%;
  height: 100%;
  padding: 10px;
  border-radius: 10px;
  border: 1px solid rgb(0, 0, 0);
  box-shadow: 29px 29px 58px #b81c1ca2, -29px -29px 58px #ff0303a8;
  display: flex;
  justify-content: space-evenly;
}
h1 {
  color: black;
  text-shadow: -1px -1px 0 rgb(255, 2, 2), 1px -1px 0 rgb(255, 0, 93), -1px 1px 0 rgb(255, 149, 149), 1px 1px 0 rgb(114, 0, 0);
  font-size: 5rem;
  margin-inline: auto;
  animation: float 6s ease-in-out infinite;
}
@keyframes float {
	0% {
		box-shadow: 0 5px 15px 0px rgba(0,0,0,0.6);
		transform: translatey(0px);
	}
	50% {
		box-shadow: 0 25px 15px 0px rgba(0,0,0,0.2);
		transform: translatey(-20px);
	}
	100% {
		box-shadow: 0 5px 15px 0px rgba(0,0,0,0.6);
		transform: translatey(0px);
	}
}

.card {
  color: white;
  margin: 10px;
  padding: 10px;
  background-color: transparent;
  border-bottom: 1px solid rgb(255, 115, 115);
  border-left: 1px solid rgb(122, 0, 0);
  text-align: left;
  flex-grow: 1;
  transition: all 0.3s linear;
  flex-basis: 0;
  display: flex;
}

.card img {
  max-width: 100px;
  max-height: 100px;
  transition: 1.5s ease-in-out;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 6px 12px -2px,
    rgba(0, 0, 0, 0.3) 0px 3px 7px -3px;
  border: 1px solid #fff;
  border-radius: 50%;
  aspect-ratio: 1;
}

.TestimonialText {
  display: none;
}

marquee{
  display: none;
}

.card:hover {
  flex-basis: 5%;
  flex-grow: 1;
}
.card:hover .TestimonialText {
  display: block;
  flex-wrap: wrap;
}

.card_one {
  border-radius: 15px 0 0 15px;
}

.card_five {
  border-radius: 0 15px 15px 0;
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

/* media queries */
@media screen and (max-width: 800px) {
  .testimonials {
    display: inline-block;
    margin-top: 10px;
  }
  .container {
    margin-inline: auto;
    position: inherit;
  }
  .card {
    max-height: 100px;
    text-align: center;
    transition: all linear;
  }
  .card img {
    display: none;
  }
  marquee{
    display: block;
    margin-bottom: 5px;
  }
}
</style>
