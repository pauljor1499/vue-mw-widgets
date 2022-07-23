<template>
  <div class="container">
    <NavBar />
    <body>
      <div class="content">
        <div class="banner">
          <div class="message">
            <h1>Lockdown Can’t Stop Your Learning</h1>
            <p>
              But you decide your timeline upgrade your skills to discover a
              Better job.
            </p>
            <v-btn color="#3FB25F" dark x-large> Join Now </v-btn>
          </div>
          <div class="image">
            <img
              src="https://www.yoloeducation.co.uk/wp-content/uploads/2019/03/stockport-home-tutor.png"
              alt=""
            />
          </div>
        </div>
        <div class="title">
          <span>Why choose &nbsp;</span>
          <h1>MathWorld?</h1>
        </div>
        <div class="grid">
          <div class="col">
            <div class="section1">
              <div class="circle">
                <img
                  src="https://bl3301files.storage.live.com/y4m7z-t4hdf0Za0QUBw7E00S0yuXKbj3rjDqpFf5ZMs5eY6xxJ-aXbw0xA4MfQkU-CsRuSnJak6kQ3bEikJoGokoN4pY4IlT1u4tK4EIJ-IHwRFUyX0s_aehMg3RKGXO_F3boXF5weSDy_7TWMWjwfefFogrb2_hZLkOoS8RvIR2y4xZFmvSqoxCMWzl0w6XO4i?width=200&height=200&cropmode=none"
                  alt=""
                />
              </div>
              <h2>Personalized Learning</h2>
              <p>
                Students practice at their own pace, first filling in gaps in
                their understanding and then accelerating their learning.
              </p>
            </div>
          </div>

          <div class="col">
            <div class="section2">
              <div class="circle">
                <img
                  src="https://bl3301files.storage.live.com/y4m2FpESxrT4vepGODp7C03rq0L1HwjynKiqRodIErurQ5yQMLAXMmZlx670Nt8-l7JfB5sUogJ2b9w55ippyvSCmfRsBOApNLyY3UDzl-NIsZl7YOCkzeW83QJIPor2vBkwGHt-ZfJv-jFtYVQyrBigia3hnUwzK9zpBLqeXfjDA7pwH6YqQ8COjPa1Ml73svu?width=376&height=376&cropmode=none"
                  alt=""
                />
              </div>
              <h2>Trusted Content</h2>
              <p>
                Created by experts, MathWorld’s library of trusted practice and
                lessons covers math. Always free for learners and teachers.
              </p>
            </div>
          </div>

          <div class="col">
            <div class="section3">
              <div class="circle">
                <img
                  src="https://bl3301files.storage.live.com/y4mzHf3X53JJD3m8Pv0mUoMpLAA69ps55rDNwaDEv8hDTKilJRjJaLJEhvl1seY11CdOjTbKS8p5bXbf8RWPpY0GdD4jV8MXzzhYayXo8oZZ_J4l9rTdAq709L9rz-EvI8iRqxBoqDLsEcMM9N4XKCngjxqtp5QcJa1MOxuAJ-n-8qXCIaR9LK7fLgLYCtMSiRD?width=548&height=562&cropmode=none"
                  alt=""
                />
              </div>
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
          <span>What do our students &nbsp;</span>
          <h1>say about us?</h1>
        </div>
        <div class="feedback">
          <v-carousel cycle height="400" hide-delimiters>
            <v-carousel-item v-for="(item, i) in items" :key="i">
              <div class="items">
                <div class="image">
                  <img :src="item.src" alt="" />
                </div>
                <div class="message">
                  <p>
                    Thank you for your hard work in supporting my son as they
                    develop. Your patience and commitment to supporting my child
                    has mean a lot to our family.
                  </p>
                  <h3>Randell L. Cardwell</h3>
                </div>
              </div>
            </v-carousel-item>
          </v-carousel>
        </div>
        <div class="join">
          <p>
            Create online classrooms and train your learners easily and
            effectively.
          </p>
          <v-btn color="#3FB25F" dark x-large> Create Now </v-btn>
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

  data() {
    return {
      items: [
        {
          src: "https://cdn.now.howstuffworks.com/media-content/0b7f4e9b-f59c-4024-9f06-b3dc12850ab7-1920-1080.jpg",
        },
        {
          src: "https://thumbs.dreamstime.com/b/filipino-youth-thumbs-up-attractive-asian-person-158307375.jpg",
        },
        {
          src: "https://www.incimages.com/uploaded_files/image/1920x1080/getty_481292845_77896.jpg",
        },
        {
          src: "https://t4.ftcdn.net/jpg/02/26/67/23/360_F_226672340_FUInCFzn7Yyso0I1KNaekRg2JBqw4XC9.jpg",
        },

        // {
        //   src: require("https://t4.ftcdn.net/jpg/02/26/67/23/360_F_226672340_FUInCFzn7Yyso0I1KNaekRg2JBqw4XC9.jpg"),
        // },
      ],
    };
  },
};
</script>

<style scoped>
.content {
  padding: 70px;
}

.content .banner {
  height: 500px;
  margin: auto;
  margin-bottom: 50px;
  border-radius: 25px;
  background-color: #cbefff;

  display: flex;
  justify-content: space-between;
}

.content .banner .message {
  width: 100%;
  padding: 5%;

  margin: auto;
}

.content .banner .message h1 {
  font-family: "Noto Serif", serif;
  line-height: 1;
  font-size: 3em;
}

.content .banner .message p {
  margin-top: 20px;
  line-height: 1;
  font-size: 1.5em;
}

.content .banner .message .v-btn {
  margin-top: 50px;
  width: 40%;
}

.content .banner .image {
  width: 100%;
  padding: 5%;

  display: flex;
  justify-content: center;
  align-items: center;
}

.content .banner .image img {
  width: 85%;
  height: 95%;
}

.content .title {
  margin: auto;
  text-align: left;
  margin-top: 100px;
  margin-bottom: 50px;
}

.content .title span {
  float: left;
  font-size: 2em;
}

.content .title h1 {
  color: #0073b0;
}

.content .grid {
  margin-top: 100px;
  margin-bottom: 100px;

  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  column-gap: 50px;
}

.content .grid .col {
  text-align: center;
}

.content .grid .col .section1 {
  height: 100%;
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

  display: flex;
  justify-content: center;
  align-items: center;
}

.content .grid .col .section1 .circle img {
  width: 50px;
}

.content .grid .col .section1 h2 {
  color: #0073b0;
}

.content .grid .col .section2 {
  height: 100%;
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

  display: flex;
  justify-content: center;
  align-items: center;
}

.content .grid .col .section2 .circle img {
  width: 50px;
}

.content .grid .col .section2 h2 {
  color: #ff244c;
}

.content .grid .col .section3 {
  height: 100%;
  display: inline-block;
  padding: 0px 50px 50px 50px;
  border-radius: 25px;
  background-color: #a6f48a;
}

.content .grid .col .section3 .circle {
  background: #05893a;
  border: 6px solid #a6f48a;
  border-radius: 50%;
  width: 100px;
  height: 100px;
  margin: auto;
  margin-top: -50px;
  margin-bottom: 25px;

  display: flex;
  justify-content: center;
  align-items: center;
}

.content .grid .col .section3 .circle img {
  width: 50px;
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
  width: 100%;
}

.feedback .v-carousel .items {
  height: 350px;
  margin: auto;
  padding: 0px 150px 0px 150px;

  display: flex;
  align-items: center;
  justify-items: center;
}

.feedback .v-carousel .image {
  float: left;
}

.feedback .v-carousel .image img {
  display: block;
  width: 200px;
  height: auto;
}

.feedback .v-carousel .message {
  display: block;
  float: right;
  padding-left: 10%;
  text-align: right;
}

.join {
  padding: 80px 200px 80px 200px;
  display: flex;
  justify-content: space-between;
  background-color: #f4f4f4;
  margin-top: 100px;
}

.join p {
  width: 65%;
  font-size: 1.5em;
}
</style>
