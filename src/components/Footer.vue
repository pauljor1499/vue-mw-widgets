<template>
  <footer>
    <div class="footer-head">
      <div class="brands">
        <a href="#"><v-icon> mdi-facebook </v-icon></a>
        <a href="#"><v-icon> mdi-twitter </v-icon></a>
        <a href="#"><v-icon> mdi-instagram </v-icon></a>
        <a href="#"><v-icon> mdi-web </v-icon></a>
      </div>
    </div>

    <div class="footer-body">
      <div class="content">
        <div class="about">
          <h3>MATHWORLD</h3>
          <p>
            As a mission-driven organization, we're relentlessly pursuing our
            vision of a world where every learner can access education to unlock
            their potential, without the barriers of cost or location.
          </p>
        </div>
      </div>

      <div class="content"></div>

      <div class="content">
        <h3>COURSES</h3>
        <a href="#">Math</a>
        <a href="#">Science</a>
        <a href="#">English</a>
        <a href="#">History</a>
      </div>

      <div class="content">
        <h3>COMPANY</h3>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Courses</a>
        <a href="#">Community</a>
      </div>
    </div>

    <div class="footer-bottom">
      <div><i>&copy; 2022 by MathWorld Developers</i></div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  width: 100%;
}
footer .footer-head {
  overflow: hidden;
  background-color: #005380;
  padding: 10px;
}
footer .footer-head .brands {
  float: right;
  margin-right: 25px;
}
footer .footer-head .brands a {
  color: gray;
  padding: 15px;
}

.v-icon {
  color: #ffff;
}
footer .footer-body {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  /* column-gap: 100px; */
  padding: 50px;
  background-color: #003754;
  border-bottom: 0.5px solid #0091de;
}
footer .footer-body .content {
  width: 100%;
  color: white;
  text-align: left;
  /* border: 1px solid black; */
}
footer .footer-body .content h3 {
  margin-bottom: 20px;
}
footer .footer-body .content .about {
  text-align: justify;
  text-justify: inter-word;
}

footer .footer-body .content a {
  display: block;
  color: white;
  margin-top: 5px;
}

footer .footer-body .content a:hover,
footer .footer-head .brands .v-icon:hover {
  color: #0091de;
}

footer .footer-bottom {
  width: 100%;
  text-align: center;
  background-color: #021c2b;
}

footer .footer-bottom div {
  padding: 20px;
  color: white;
}
</style>
