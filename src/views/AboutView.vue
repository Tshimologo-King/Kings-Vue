<template>
  <div id="about">
    <div class="aboutContent">
      <h2>Find about me</h2>
      <div v-if="showModal">
        <div class="backdrop" @click="closeModal">
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
            <button @click="closeModal">Close Modal</button>
          </div>
        </div>
      </div>
      <button @click="toggleModal">Open Modal</button>
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
    };
  },
  methods: {
    toggleModal() {
      this.showModal = !this.showModal;
    },
    closeModal() {
      this.showModal == this.showModal;
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
  padding: 20px;
  height: 500px;
  width: 500px;
  border-radius: 25px;
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
  font-size: 21px;
}

.modal-content p {
  font-size: 14px;
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
