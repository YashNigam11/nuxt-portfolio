<template>
  <div class="about-me" id="about">
    <h1>About Me</h1>
    <div class="card">
      <p>{{ description }}</p>
    </div>
    <h3>Qualifications details</h3>
    <table class="data-table">
      <thead>
        <tr>
          <th>Class 10</th>
          <th>Class 12</th>
          <th>B.Tech</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="qualification in qualifications" :key="qualification">
          <td>{{ qualification.class10 }}</td>
          <td>{{ qualification.class12 }}</td>
          <td>{{ qualification.btech }}</td>
        </tr>
      </tbody>
    </table>
    <div class="buttons">
      <button class="btn-primary">Hire Me</button>
      <button class="btn-secondary">
        <a href="~assets/resume/Yash_Nigam_Resume.pdf" download>
          Download Resume
        </a>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      description:
        "I am a passionate Front End Web and Mobile Application Developer with a strong background in HTML, CSS, SCSS, Bootstrap, and React.js with Redux. I have a knack for crafting cutting-edge applications that combine exceptional user experiences with high efficiency. With my B.TECH degree and industry experience, I am eager to bring my expertise to an organization and contribute as a valuable asset.My approach to development is driven by innovation. I constantly seek out new technologies, trends, and design patterns to create immersive and engaging user interfaces. By leveraging my extensive knowledge of front-end technologies, I excel at building responsive, performant, and visually appealing applications that meet the highest standards.Through my passion for web and mobile development, I strive to push the boundaries of what is possible, creating intuitive and seamless user interactions. I am committed to delivering elegant solutions that not only meet client requirements but also exceed user expectations.",
      qualifications: [
        { class10: "Grade A", class12: "Grade B", btech: "Grade A" },
        { class10: "75%", class12: "57%", btech: "75%" },
        {
          class10: "First Class",
          class12: "First Class",
          btech: "Distinction",
        },
      ],
    };
  },
};
</script>

<style scoped>
.about-me {
  /* height: 100vh; */
  text-align: center;
  padding: 25px;
}

h1 {
  font-size: 2.25rem;
}

.card {
  margin: 25px;
  padding: 25px;
}

h3 {
  padding: 20px;
  font-size: 1.25rem;
  text-decoration: underline;
}

.data-table {
  margin: 0 auto;
  border-collapse: collapse;
  width: 100%;
  max-width: 600px;
}

.data-table th,
.data-table td {
  padding: 10px;
  border: 1px solid #ccc;
}

.buttons {
  padding: 25px;
}

.btn-primary,
.btn-secondary {
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  font-size: 1rem;
  margin-top: 10px;
  cursor: pointer;
}
.btn-primary {
  background-color: red;
}
.btn-secondary {
  background-color: yellowgreen;
}
.btn-secondary a {
  color: white;
  text-decoration: none;
}
</style>
