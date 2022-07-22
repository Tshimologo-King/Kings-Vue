<template>
    <div id="ContactMe">
        <h2 style="margin-bottom: 2rem; margin-top">Contact Me</h2>
        <div class="contactMeDetails">
            <form action="https://formspree.io/f/xoqrkjrq" method="post">
                <div class="col-lg-12 mt-4 mb-3">
                    <input type="text" style="width: 50%; height: 50px" placeholder="Full Name" name="name" required>
                </div>
                <div class="col mt-4">
                    <input type="text" style="width: 50%; height: 50px" placeholder="name@gmail.com" name="name" required>
                </div>
                <div class="mb-3 mt-4">
                    <input type="text" style="width: 50%; height: 50px;" placeholder="Subject" name="name" required>
                </div>
                <div class="form-group col-lg-12 md-12 mt-4">
                    <textarea id="enquires" style="height: 10vh; width: 50%; margin-bottom:2rem;" placeholder="Enquiries..."></textarea>
                </div>
                <div class="button text-center">
                    <button type="submit" style="height: 5vh; width:25%; border-radius: 25px">submit</button>
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