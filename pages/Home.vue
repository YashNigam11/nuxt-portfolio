<template>
  <div class="portfolio-container" id="home">
    <h2>My Portfolio</h2>
    <img src="~assets/img/pic.jpeg" height="300" />
    <h2>Yash Nigam</h2>
    <p>Front End Developer, React Developer, UI/UX Developer</p>
    <p class="main-heading">
      I like to craft solid and scalable front end products with great user
      experience.
    </p>
    <button class="btn-download">
      <a href="~assets/resume/Yash_Nigam_Resume.pdf" download>Resume</a>
    </button>
  </div>
</template>

<style scoped>
.portfolio-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 20px;
  /* height: 100vh; */
}

img {
  padding: 20px;
  border-radius: 50%;
}
h2{
  font-size: 2rem;
  text-decoration: wavy;
}

.main-heading {
  font-size: 18px;
  color: white;
}

.btn-download {
  background-color: teal;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  font-size: 16px;
  margin-top: 20px;
  cursor: pointer;
}

.btn-download a {
  color: white;
  text-decoration: none;
}
</style>
