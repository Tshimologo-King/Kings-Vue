<template>
  <div id="about">
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
              (2019-Present)<br />
              Python: Data Science <br />[Statistics, Mathematics, Python,
              Machine Learning, Deep Learning]
            </p>
            <h4>Life Choices Academy</h4>
            <p>
              (2022 - Present)<br />
              Web Development
            </p>
            <button class="closeButton" @click="toggleModal">Close Modal</button>
          </div>
        </div>
      </div>
      <button class="openButton" @click="toggleModal">Education History</button>
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
            <button class="closeButton" @click="toggleModalWork">Close Modal</button>
          </div>
        </div>
      </div>
      <button class="openButton" @click="toggleModalWork">Work History</button>
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
      <button class="openButton" @click="toggleModalSoft">Soft Skills</button>
      <div v-if="showModalTechnical">
        <div class="backdrop">
          <div class="modal-contentTechnical">
            <h2>Technical Skills</h2>
            <h4>HTML</h4>
            <h4>CSS</h4>
            <h4>BOOTSRAP</h4>
            <h4>MySQL</h4>
            <h4>NODE JS</h4>
            <h4>VUE JS</h4>
            <h4>MICROSOFT</h4>
            <button class="closeButton" @click="toggleModalTechnical">
              Close Modal
            </button>
          </div>
        </div>
      </div>
      <button class="openButton" @click="toggleModalTechnical">Technical Skills</button>
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
    toggleModalTechnical(){
      this.showModalTechnical = !this.showModalTechnical;
    }
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

#about {
  background-color: black;
  height: 100vh;
  width: 100%;
  background-position: center;
  background-repeat: no-repeat;
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
  margin-top: 14rem;
  height: 50vh;
  border-radius: 10px;
  border-radius: 32px;
  background: #333333;
  box-shadow: 29px 29px 58px #2c2c2c, -29px -29px 58px #969696;
}

.modal-content {
  background-color: white;
  color: black;
  padding: 50px;
  height: 500px;
  width: 500px;
  border-radius: 25px;
}
.modal-contentWork {
  background-color: white;
  color: black;
  padding: 50px;
  height: 500px;
  width: 500px;
  border-radius: 25px;
}
.modal-contentSkills {
  padding: 30px;
  height: 300px;
  width: 300px;
  text-align: center;
  background-color: white;
  color: black;
  border-radius: 25px;
}
.modal-contentTechnical{
  padding: 30px;
  height: 300px;
  width: 300px;
  text-align: center;
  background-color: white;
  color: black;
  border-radius: 25px;
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
.modal-contentTechnical h2{
  margin-bottom: 5px;
  font-size: 23px;
}
.modal-contentTechnical h4{
  font-size: 18px;
  margin-bottom: 5px;
}

.modal-contentTechnical p{
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
}
.pageLinkNext button {
  padding: 5px 10px;
  border-radius: 25px;
}
</style>
