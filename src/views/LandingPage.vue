<template>
  <div class="container">
    <NavBar />
    <body>
      <div class="content">
        <div class="content-video"></div>
        <div class="title">
          <h1>Why Choose MathWorld?</h1>
        </div>
        <div class="grid">
          <div class="col">
            <div class="section1">
              <div class="circle"></div>
              <h2>Personalized Learning</h2>
              <p>
                Students practice at their own pace, first filling in gaps in
                their understanding and then accelerating their learning.
              </p>
            </div>
          </div>

          <div class="col">
            <div class="section2">
              <div class="circle"></div>
              <h2>Trusted Content</h2>
              <p>
                Created by experts, MathWorld’s library of trusted practice and
                lessons covers math. Always free for learners and teachers.
              </p>
            </div>
          </div>

          <div class="col">
            <div class="section3">
              <div class="circle"></div>
              <h2>Tools to Empower Teachers</h2>
              <p>
                With MathWorld, teachers can identify gaps in their students’
                understanding, tailor instruction, and meet the needs of every
                student.
              </p>
            </div>
          </div>
        </div>
        <div class="about">
          <div class="about-message">
            <h1>Explore the World of Math</h1>
            <p>
              Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit
              aut fugit, sed quia consequuntur magni dolores eos qui ratione
              voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem.
            </p>
          </div>
          <img
            src="https://img.freepik.com/free-photo/books-pencils-desk-by-blackboard_181624-47246.jpg?w=900"
            alt="knowledge"
          />
        </div>
        <div class="title">
          <h1>Why Choose MathWorld?</h1>
        </div>
        <div class="feedback">
          <v-carousel hide-delimiters>
            <v-carousel-item
              v-for="(item, i) in items"
              :key="i"
              :src="item.src"
            ></v-carousel-item>
          </v-carousel>

          <!-- <n-carousel autoplay>
            <div>
              <img
                class="carousel-img"
                src="https://cdn.now.howstuffworks.com/media-content/0b7f4e9b-f59c-4024-9f06-b3dc12850ab7-1920-1080.jpg"
              />
              <h3>Randell L. Cardwell</h3>
              <p>
                Thank you for your hard work in supporting my son as they
                develop. Your patience and commitment to supporting my child has
                mean a lot to our family.
              </p>
            </div>
            <div>
              <img
                class="carousel-img"
                src="https://thumbs.dreamstime.com/b/filipino-youth-thumbs-up-attractive-asian-person-158307375.jpg"
              />
              <h3>Keith A. Hand</h3>
              <p>
                With your guidance, our daughter has developed into a confident
                and capable child. Thank you for being such an important part in
                our child’s development.
              </p>
            </div>
            <div>
              <img
                class="carousel-img"
                src="https://www.incimages.com/uploaded_files/image/1920x1080/getty_481292845_77896.jpg"
              />
              <h3>Claude S. Black</h3>
              <p>
                Your expertise in teaching has put our minds at ease. We are so
                grateful to have you as our child’s teacher.
              </p>
            </div>
            <div>
              <img
                class="carousel-img"
                src="https://t4.ftcdn.net/jpg/02/26/67/23/360_F_226672340_FUInCFzn7Yyso0I1KNaekRg2JBqw4XC9.jpg"
              />
              <h3>Michelle F. Molina</h3>
              <p>
                It is clear that our child’s literacy and numeracy skills have
                developed considerably while under your care. Thank you for
                helping him to develop the skills and confidence that he will
                carry forward into the next school year.
              </p>
            </div>
          </n-carousel> -->
        </div>
      </div>
    </body>
    <Footer />
  </div>
</template>

<script>
import NavBar from "../components/NavBar.vue";
import Footer from "../components/Footer.vue";

export default {
  components: { NavBar, Footer },
};
</script>

<style scoped>
.content {
  padding: 70px;
}

.content .content-video {
  height: 500px;
  margin: auto;
  margin-bottom: 50px;
  border-radius: 25px;
  background-color: #cbefff;
}

.content .title {
  margin: auto;
  text-align: left;
  margin-top: 100px;
  margin-bottom: 50px;
}

.content .grid {
  margin: auto;
  margin-top: 100px;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  column-gap: 50px;
  margin-bottom: 100px;
}

.content .grid .col {
  text-align: center;
  margin: auto;
}

.content .grid .col .section1 {
  display: inline-block;
  padding: 0px 50px 50px 50px;
  border-radius: 25px;
  background-color: #8cd6ff;
}

.content .grid .col .section1 .circle {
  background: #0073b0;
  border-radius: 50%;
  border: 6px solid #8cd6ff;
  width: 100px;
  height: 100px;
  margin: auto;
  margin-top: -50px;
  margin-bottom: 25px;
}

.content .grid .col .section1 h2 {
  color: #0073b0;
}

.content .grid .col .section2 {
  display: inline-block;
  padding: 0px 50px 50px 50px;
  border-radius: 25px;
  background-color: #ffcdcd;
}

.content .grid .col .section2 .circle {
  background: #ff244c;
  border-radius: 50%;
  border: 6px solid #ffcdcd;
  width: 100px;
  height: 100px;
  margin: auto;
  margin-top: -50px;
  margin-bottom: 25px;
}

.content .grid .col .section2 h2 {
  color: #ff244c;
}

.content .grid .col .section3 {
  display: inline-block;
  padding: 0px 50px 50px 50px;
  border-radius: 25px;
  background-color: #a6f48a;
}

.content .grid .col .section3 .circle {
  background: #05893a;
  border-radius: 50%;
  border: 6px solid #a6f48a;
  width: 100px;
  height: 100px;
  margin: auto;
  margin-top: -50px;
  margin-bottom: 25px;
}

.content .grid .col .section3 h2 {
  color: #05893a;
}

.content .grid .col h2 {
  margin-bottom: 20px;
}

.content .grid .col button {
  float: left;
}

.about {
  margin: auto;
  border-radius: 25px;
  background-color: #ffc38b;
  padding: 100px;
  display: grid;
  grid-template-columns: 1fr 1fr;
}

.about-message {
  /* text-align: left; */
}

.about-message h1 {
  color: white;
  margin-bottom: 20px;
}

.about-message p {
  color: white;
  font-size: 1.2em;
  text-align: justify;
  text-justify: inter-word;
}

.about img {
  width: 85%;
  height: 240px;
  object-fit: cover;
  margin: 0px 80px 0px;
  box-shadow: 0px 5px 15px 0px #505050;
}

.feedback {
  border: 1px solid black;
  margin: auto;
  text-align: center;
}

.feedback h1 {
  margin: auto;
  width: 50%;
  text-align: center;
  /* margin-bottom: 50px; */
}

.feedback h3 {
}

.feedback p {
  margin: auto;
  width: 50%;
  text-align: center;
}

.feedback .n-carousel img {
  width: 50%;
  height: 240px;
  object-fit: cover;
  margin: auto;
}
</style>
