<template>
  <div id="about">
    <div class="aboutContent">
      <h2>Find about me</h2>
      <div class="modal_button col-lg-4 col-md-6" id="something">
      <!-- Button trigger modal -->
      <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
        <div class="openButton">Work something</div>
      </button>
      <!-- Modal -->
      <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header" style="padding: 10px;">
            <h5 class="modal-title" id="exampleModalLabel">Education</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close" style="margin:5px"></button>
          </div>
          <div class="modal-body" style="background-color: grey; color:white">
            <h4>Springs Boys' High School</h4>
            <p>(2012-2016)<br>
            Matric Certificate Diploma</p>
            <h4>Star Schools</h4>
            <p>(2017-2018)<br>Matric Rewrite<br>
            Matric Certificate Bachelor</p>
            <h4>University of The Western Cape</h4><p>(2018-2020)<br>Bachelor of Commerce<br>
            Majors: Economics & Finance</p>
            <h4>Udemy: Online Learning</h4>
            <p>(2019-2022)<br>
            Python: Data Science <br>[Statistics, Mathematics, Python, Machine Learning, Deep Learning]</p>
            <h4>Life Choices Academy</h4>
            <p>(2022 - Present)<br>
            Web Development</p>
          </div>
          <div class="modal-footer" style="padding: 10px">
            <button type="button" class="btn btn-secondary" data-bs-dismiss="modal" style="margin: 5px; padding: 5px;">Close</button>
          </div>
        </div>
      </div>
      </div>                     
      </div>
      <div class="modal_button col-lg-4 col-md-6" id="something">
      <!-- Button trigger modal -->
      <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
        <div class="openButton">Work Experience</div>
      </button>
      <!-- Modal -->
      <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header" style="padding: 10px;">
            <h5 class="modal-title" id="exampleModalLabel">Education</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close" style="margin:5px"></button>
          </div>
          <div class="modal-body" style="background-color: grey; color:white">
            <h4>Springs Boys' High School</h4>
            <p>(2012-2016)<br>
            Matric Certificate Diploma</p>
            <h4>Star Schools</h4>
            <p>(2017-2018)<br>Matric Rewrite<br>
            Matric Certificate Bachelor</p>
            <h4>University of The Western Cape</h4><p>(2018-2020)<br>Bachelor of Commerce<br>
            Majors: Economics & Finance</p>
            <h4>Udemy: Online Learning</h4>
            <p>(2019-2022)<br>
            Python: Data Science <br>[Statistics, Mathematics, Python, Machine Learning, Deep Learning]</p>
            <h4>Life Choices Academy</h4>
            <p>(2022 - Present)<br>
            Web Development</p>
          </div>
          <div class="modal-footer" style="padding: 10px">
            <button type="button" class="btn btn-secondary" data-bs-dismiss="modal" style="margin: 5px;padding: 5px;">Close</button>
          </div>
        </div>
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

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
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
    box-shadow:  29px 29px 58px #2c2c2c,-29px -29px 58px #969696;
}

#something{
  color: white;
  width: 100%;
  margin-inline: auto;
}
.openButton{
  padding: 10px;
  text-align: center;
}
</style>
