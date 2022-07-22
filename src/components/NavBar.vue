<template>
  <header class="header">
    <div class="logo">
      <router-link :to="'/navbar'">
        <span>MathWorld</span>
      </router-link>
    </div>
    <ul class="main-nav">
      <li>
        <router-link :to="'/'">
          <span>Home</span>
        </router-link>
      </li>
      <li>
        <router-link :to="'/'">
          <span>About</span>
        </router-link>
      </li>
      <li>
        <router-link :to="'/'">
          <span>Courses</span>
        </router-link>
      </li>
      <li>
        <router-link :to="'/'">
          <span>Community</span>
        </router-link>
      </li>
      <div class="buttons">
        <button>
          <router-link :to="'/'">
            <span>Log In</span>
          </router-link>
        </button>
        <button>
          <router-link :to="'/'"><span>Register</span></router-link>
        </button>
      </div>
    </ul>
  </header>
</template>

<style scoped>
span {
  color: black;
}

.header {
  display: flex;
  justify-content: space-between;

  font-family: "Lato", sans-serif;
  padding: 0px 5% 0px 5%;
  border-bottom: 1px solid #e0e0e0;
  box-shadow: 0px 0px 14px 0px rgba(0, 0, 0, 0.05);
}

.logo {
  display: flex;
  align-items: center;

  font-size: 2.2em;
}

.main-nav {
  display: flex;
}

.main-nav li {
  font-size: 1.2em;
  padding: 35px 20px 35px 20px;
  text-align: center;
  border-bottom: 2px solid white;
}

.main-nav .buttons {
  margin: auto;
}

.main-nav button {
  height: 45px;
  margin: 5px;
  padding: 10px;
}

.main-nav button span {
  font-size: 1.2em;
}

.main-nav li:hover {
  background-color: #e7f7ff;
  border-bottom: 2px solid #0091de;
}

/* @media (min-width: 769px) {
  .header,
  .main-nav {
    display: flex;
  }
  .header {
    flex-direction: column;
    align-items: center;
  }
}

@media (min-width: 1025px) {
  .header {
    flex-direction: row;
    justify-content: space-between;
  }
} */
</style>
