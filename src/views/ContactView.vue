<template>
    <div id="ContactMe">
        <h1 style="margin-bottom: 2rem; margin-top">Contact Me</h1>
        <div class="contactMeDetails">
            <form action="https://formspree.io/f/xoqrkjrq" method="post">
                <div class="col-lg-12 mt-4 mb-3">
                    <input type="text" style="width: 50%; height: 50px; border-radius: 15px; padding: 10px" placeholder="Full Name" name="name" required>
                </div>
                <div class="col mt-4">
                    <input type="text" style="width: 50%; height: 50px; border-radius: 15px; padding: 10px" placeholder="name@gmail.com" name="name" required>
                </div>
                <div class="mb-3 mt-4">
                    <input type="text" style="width: 50%; height: 50px; border-radius: 15px; padding: 10px" placeholder="Subject" name="name" required>
                </div>
                <div class="form-group col-lg-12 md-12 mt-4">
                    <textarea id="enquires" style="height: 10vh; width: 50%; margin-bottom:2rem;border-radius: 15px; padding: 10px" placeholder="Enquiries..."></textarea>
                </div>
                <div class="button text-center">
                    <button type="submit" style="height: 6vh; width:20%; border-radius: 25px; padding: 10px">submit</button>
                </div>
            </form>
        </div>
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

h1 {
  color: black;
  text-shadow: -1px -1px 0 rgb(127, 163, 0), 1px -1px 0 rgba(105, 147, 55, 0.505), -1px 1px 0 rgb(17, 255, 0), 1px 1px 0 rgba(69, 223, 102, 0.286);
  font-size: 5rem;
  display: flex;
  align-items: center;
  justify-content: center;
  animation: float 6s ease-in-out infinite;
}

.contactMeDetails{
   width: 50%;
  padding: 10px;
  border-radius: 10px;
  border: 1px solid rgb(0, 0, 0);
  margin-inline: auto;
  box-shadow: 29px 29px 58px #44ff00a2, -29px -29px 58px #31ff0397;
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