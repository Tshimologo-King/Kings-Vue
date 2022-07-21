<template>
    <div id="ContactMe">
        <h2>Contact Me</h2>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Et, delectus.



    <div class="navigationLinks">
        <div class="pageLinkPrev">
          <router-link to="/testimonials">
            <button>Testimonials</button>
          </router-link>
        </div>
        <div class="pageLinkNext">
          <router-link to="/">
            <button>Back To Home</button>
          </router-link>
        </div>
    </div>
    </div>
</template>
<style scoped>
*{
    padding: 0;
    margin:0;
    box-sizing: border-box;
}

#ContactMe{
    background-color: black;
    height: 100vh;
    width: 100%;
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