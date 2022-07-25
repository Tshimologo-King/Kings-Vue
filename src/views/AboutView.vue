<template>
  <div id="about">
    <h1>ABOUT</h1>
    <div class="aboutContent">
      <h2>Find about me</h2>
      <div v-if="showModal">
        <div class="backdrop">
          <div class="modal-content">
            <h2>Education History</h2>
            <h4>Springs Boys' High School</h4>
            <p>
              (2012-2016)<br />
              Matric Certificate Diploma
            </p>
            <h4>Star Schools</h4>
            <p>
              (2017-2018)<br />Matric Rewrite<br />
              Matric Certificate Bachelor
            </p>
            <h4>University of The Western Cape</h4>
            <p>
              (2018-2020)<br />Bachelor of Commerce<br />
              Majors: Economics & Finance
            </p>
            <h4>Udemy: Online Learning</h4>
            <p>
              (2019-2022)<br />
              Python: Data Science <br />[Statistics, Mathematics, Python,
              Machine Learning, Deep Learning]
            </p>
            <h4>Life Choices Academy</h4>
            <p>
              (2022 - Present)<br />
              Web Development
            </p>
            <button class="closeButton" @click="toggleModal">
              Close Modal
            </button>
          </div>
        </div>
      </div>
      <button class="openButton" @click="toggleModal" id="EduHistory">
        Education History
      </button>
      <div v-if="showModalWork">
        <div class="backdrop">
          <div class="modal-contentWork">
            <h2>Work Experience</h2>
            <h4>GDE: Markers Assistant</h4>
            <p>(2017 December 1st - 14th)</p>
            <h4>Self-Employed</h4>
            <p>
              (2019-2020)<br />
              Gadget Reseller<br />(2020-2021)<br />King' Bin Cleaning Service
            </p>
            <h4>Kwa-Thema Primary School</h4>
            <p>
              Government Initiative(2021 Mar - June)<br />
              [Teachers' Assistant, Ground Staff]
            </p>
            <h4>Rebone Business Enterprise CC.</h4>
            <p>
              Construction Company<br />
              (5th July 2021 - 25th March 2022)<br />
              Administrative Officer
            </p>
            <button class="closeButton" @click="toggleModalWork">
              Close Modal
            </button>
          </div>
        </div>
      </div>
      <button class="openButton" @click="toggleModalWork" id="WorkHistory">
        Work History
      </button>
      <div v-if="showModalSoft">
        <div class="backdrop">
          <div class="modal-contentSkills">
            <h2>Soft Skills</h2>
            <p>Strong Communication Skills</p>
            <p>Team-Work</p>
            <p>Problem-Solving</p>
            <p>Grit</p>
            <p>Leadership</p>
            <button class="closeButton" @click="toggleModalSoft">
              Close Modal
            </button>
          </div>
        </div>
      </div>
      <button class="openButton" @click="toggleModalSoft" id="SoftSkills">
        Soft Skills
      </button>
      <div v-if="showModalTechnical">
        <div class="backdrop">
          <div class="modal-contentTechnical">
            <h2>Technical Skills</h2>
            <h4>HTML</h4>
            <h4>CSS</h4>
            <h4>BOOTSRAP</h4>
            <h4>MySQL</h4>
            <h4>JAVASCRIPT</h4>
            <h4>NODE JS</h4>
            <h4>VUE JS</h4>
            <h4>MICROSOFT</h4>
            <button class="closeButton" @click="toggleModalTechnical">
              Close Modal
            </button>
          </div>
        </div>
      </div>
      <button class="openButton" @click="toggleModalTechnical" id="TechSkills">
        Technical Skills
      </button>
    </div>
    <div class="navigationLinks">
      <div class="pageLinkPrev">
        <router-link to="/">
          <button>Home</button>
        </router-link>
      </div>
      <div class="pageLinkNext">
        <router-link to="/projects">
          <button>Projects</button>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showModal: false,
      showModalWork: false,
      showModalSoft: false,
      showModalTechnical: false,
    };
  },
  methods: {
    toggleModal() {
      this.showModal = !this.showModal;
    },
    toggleModalWork() {
      this.showModalWork = !this.showModalWork;
    },
    toggleModalSoft() {
      this.showModalSoft = !this.showModalSoft;
    },
    toggleModalTechnical() {
      this.showModalTechnical = !this.showModalTechnical;
    },
  },
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: monospace;
}

.backdrop {
  height: 100%;
}

#about {
  background-color: black;
  height: 100vh;
  width: 100%;
  background-position: center;
  background-repeat: no-repeat;
}
h1 {
  color: black;
  text-shadow: -1px -1px 0 rgb(19, 2, 255), 1px -1px 0 rgb(67, 79, 255), -1px 1px 0 rgb(10, 0, 144), 1px 1px 0 rgb(64, 159, 242);
  font-size: 8rem;
  margin-inline: auto;
  animation: float 6s ease-in-out infinite;
}

.aboutContent {
  color: white;
  background-color: rgba(2, 2, 2, 0.667);
  display: flex;
  justify-content: space-evenly;
  flex-direction: column;
  border: 1px solid rgb(47, 47, 47);
  float: right;
  padding: 30px;
  margin-inline: 110px;
  margin-top: 6rem;
  height: 50vh;
  border-radius: 10px;
  border-radius: 32px;
  background: #333333;
  box-shadow: 29px 29px 58px #04033e, -29px -29px 58px #264689;
}

.modal-content {
  background-color: rgb(0, 0, 0);
  padding: 50px;
  height: 500px;
  width: 500px;
  border-radius: 25px;
  animation: pulsate 2.5s infinite alternate; 
}
.modal-contentWork {
  background-color: rgb(0, 0, 0);
  padding: 50px;
  height: 500px;
  width: 500px;
  border-radius: 25px;
  animation: pulsate 2.5s infinite alternate;
}
.modal-contentSkills {
  padding: 30px;
  height: 300px;
  width: 300px;
  text-align: center;
  background-color: rgb(0, 0, 0);
  border-radius: 25px;
  animation: pulsate 2.5s infinite alternate;
}
.modal-contentTechnical {
  padding: 30px;
  height: 300px;
  width: 300px;
  text-align: center;
  background-color: rgb(0, 0, 0);
  border-radius: 25px;
  animation: pulsate 2.5s infinite alternate;
}
.modal-contentSkills p,
h2 {
  margin-bottom: 10px;
}
.backdrop {
  top: 15%;
  left: 30%;
  position: fixed;
  background: rgba(0, 0, 0, 0.5);
  width: 100%;
  height: 100%;
}
.modal-content h2 {
  margin-bottom: 20px;
  font-size: 23px;
}

.modal-content h4 {
  font-size: 14px;
}

.modal-content p {
  font-size: 12px;
}
.modal-contentWork h2 {
  margin-bottom: 20px;
  font-size: 23px;
}
.modal-contentWork h4 {
  font-size: 21px;
}
.modal-contentWork p {
  font-size: 14px;
  margin-bottom: 10px;
}
.modal-contentTechnical h2 {
  margin-bottom: 5px;
  font-size: 23px;
}
.modal-contentTechnical h4 {
  font-size: 18px;
  margin-bottom: 5px;
}

.modal-contentTechnical p {
  font-size: 14px;
  margin-bottom: 10px;
}
.openButton {
  padding: 5px 10px;
  border-radius: 25px;
}

.closeButton {
  padding: 10px;
  line-height: 20px;
  border-radius: 25px;
}

#something {
  color: white;
  width: 100%;
  margin-inline: auto;
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
  box-shadow: 29px 29px 58px #04033e, -29px -29px 58px #264689;

}
.pageLinkNext button {
  padding: 5px 10px;
  border-radius: 25px;
  box-shadow: 29px 29px 58px #04033e, -29px -29px 58px #264689;
}
@media screen and(max-width: 900px) {
  .modal-contentTechnical h4 {
    font-size: 14px;
  }
}

/* mediaQueries */
@media screen and (max-width: 800px) {
  .modal-content {
    max-width: 350px;
    max-height: 500px;
    margin-inline: -50px;
    margin-top: -2.5rem;
  }
  .modal-content h2 {
    margin-top: -2rem;
  }
  .modal-content h4 {
    margin-top: 3px;
    font-weight: bold;
    text-decoration-line: underline;
    font-size: 15px;
  }
  .modal-content button {
    margin-top: 10px;
  }
  .modal-contentWork {
    max-width: 405px;
    max-height: 405px;
    margin-inline: -75px;
    margin-top: 2.5rem;
    padding: 5px;
  }
  .modal-contentWork h2 {
    margin-top: -5px;
    font-size: 25px;
  }
  .modal-contentWork h4 {
    margin-top: -5px;
    font-weight: bold;
    text-decoration-line: underline;
    font-size: 14px;
  }
  .modal-contentWork button {
    margin-top: -5px;
    font-size: 15px;
    width: 50%;
  }

  .modal-contentTechnical {
    max-height: 500px;
  }
  .modal-contentTechnical h2 {
    margin-top: -1rem;
  }
  .modal-contentTechnical h4 {
    font-size: 15px;
  }
}

@media screen and (max-width: 700px) {
  .modal-content {
    max-width: 350px;
    max-height: 500px;
    position: relative;
    margin-inline: -50px;
    margin-top: -2.5rem;
  }
  .modal-content h2 {
    margin-top: -2rem;
  }
  .modal-content h4 {
    margin-top: 3px;
    font-weight: bold;
    text-decoration-line: underline;
    font-size: 14px;
  }
  .modal-content button {
    margin-top: 10px;
  }
  .modal-contentWork {
    max-width: 405px;
    max-height: 405px;
    margin-inline: -75px;
    margin-top: 2.5rem;
    padding: 5px;
  }
  .modal-contentWork h2 {
    margin-top: -5px;
    font-size: 25px;
  }
  .modal-contentWork h4 {
    margin-top: -5px;
    font-weight: bold;
    text-decoration-line: underline;
    font-size: 14px;
  }
  .modal-contentWork button {
    margin-top: -5px;
    font-size: 15px;
    width: 50%;
  }
  .modal-contentTechnical h4 {
    font-size: 14px;
  }
}

@media screen and (max-width: 600px) {
  .modal-content {
    max-width: 300px;
    max-height: 500px;
    position: relative;
    margin-inline: -50px;
    margin-top: -2.5rem;
  }
  .modal-content h2 {
    margin-top: -2rem;
  }
  .modal-content h4 {
    margin-top: -3px;
    font-weight: bold;
    text-decoration-line: underline;
  }
  .modal-contentWork {
    max-width: 400px;
    max-height: 400px;
    margin-inline: -75px;
    margin-top: 2.5rem;
    padding: 5px;
  }
  .modal-contentWork h2 {
    margin-top: -5px;
    font-size: 25px;
  }
  .modal-contentWork h4 {
    margin-top: -5px;
    font-weight: bold;
    text-decoration-line: underline;
    font-size: 16px;
  }
  .modal-contentWork button {
    margin-top: -5px;
    font-size: 15px;
    width: 50%;
  }
  .modal-contentTechnical h4 {
    font-size: 15px;
  }
}
@media screen and (max-width: 500px) {
  .aboutContent {
    width: 250px;
  }
  .aboutContent button {
    width: 200px;
  }
  .modal-content {
    max-width: 350px;
    max-height: 450px;
    position: relative;
    margin-inline: -75px;
    margin-top: -2.5rem;
  }
  .modal-content h2 {
    margin-top: -2rem;
  }
  .modal-content h4 {
    margin-top: -2px;
    font-weight: bold;
    text-decoration-line: underline;
  }
  .modal-content button {
    margin-top: 10px;
    height: 25px;
    line-height: 2px;
    font-size: 15px;
    width: 50%;
    margin-inline: auto;
  }
  .modal-contentWork {
    max-width: 300px;
    max-height: 450px;
    margin-inline: -75px;
    margin-top: -1rem;
    padding: 5px;
  }
  .modal-contentWork h2 {
    margin-top: 2rem;
    font-size: 20px;
  }
  .modal-contentWork h4 {
    margin-top: -1rem;
    font-weight: bold;
    text-decoration-line: underline;
    font-size: 18px;
  }
  .modal-contentWork button {
    margin-top: -5px;
    font-size: 15px;
    width: 50%;
  }
  .modal-contentSkills {
    max-width: 300px;
    max-height: 300px;
    margin-inline: -65px;
  }
  .modal-contentTechnical {
    max-width: 400px;
    max-height: 450px;
    margin-inline: -50px;
  }
  .modal-contentTechnical h4 {
    font-size: 15px;
  }
}
@media screen and (max-width: 400px) {
  .aboutContent {
    width: 200px;
    padding: 10px 10px;
  }
  .aboutContent button {
    width: 100%;
  }
  .modal-content {
    max-width: 350px;
    max-height: 450px;
    position: relative;
    margin-inline: -75px;
    margin-top: -2.5rem;
  }
  .modal-content h2 {
    margin-top: -2rem;
  }
  .modal-content h4 {
    margin-top: -2px;
    font-weight: bold;
    text-decoration-line: underline;
  }
  .modal-content button {
    margin-top: 10px;
    height: 20px;
    font-size: 15px;
    width: 50%;
    margin-inline: auto;
  }

  .modal-contentWork {
    max-width: 300px;
    max-height: 450px;
    margin-inline: -75px;
    margin-top: 3rem;
    overflow: hidden;
    padding: 5px;
  }
  .modal-contentWork h2 {
    margin-top: 2rem;
    font-size: 25px;
  }
  .modal-contentWork h4 {
    margin-top: -1rem;
    font-weight: bold;
    text-decoration-line: underline;
    font-size: 18px;
  }
  .modal-contentWork button {
    margin-top: -5px;
    font-size: 15px;
    width: 50%;
  }
  .modal-contentSkills {
    max-width: 300px;
    max-height: 300px;
    margin-inline: -75px;
  }
  .modal-contentTechnical {
    max-width: 400px;
    max-height: 450px;
    margin-inline: -80px;
  }
  .modal-contentTechnical h4 {
    font-size: 15px;
  }
}
@keyframes pulsate {
  100% {
    /* Larger blur radius */
    text-shadow:
      0 0 4px #fff,
      0 0 11px #fff,
      0 0 19px #fff,
      0 0 40px #0fa,
      0 0 80px #0fa,
      0 0 90px #0fa,
      0 0 100px #0fa,
      0 0 150px #0fa;
  }
  0% {
    /* Smaller blur radius */
    text-shadow:
      0 0 2px #fff,
      0 0 4px #fff,
      0 0 6px #fff,
      0 0 10px rgb(0, 68, 255),
      0 0 45px rgb(49, 98, 163),
      0 0 55px rgb(9, 27, 107),
      0 0 70px rgb(0, 26, 255),
      0 0 80px rgb(12, 66, 95);
  }
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
</style>
