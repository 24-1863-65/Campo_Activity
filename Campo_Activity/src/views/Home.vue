src/views/Home.vue
<template>
  <main class="home">

    <section class="hero">


      <div class="hero-content">

        <div class="established">
          <span></span>
          ESTABLISHED 1905
        </div>

        <h1>
          Exemplary
          <em>Christian</em>
          <br />
          Education for Life.
        </h1>

        <div class="gold-line"></div>

        <p>
          A leading Christian institution in the Philippines.
          Central Philippine University nurtures intellectual growth
          and spiritual development through a commitment to
          <strong>Scientia et Fides</strong>
          (Science and Faith).
        </p>

        <div class="buttons">
          <button class="primary">
            Explore Academics
          </button>

          <button class="secondary">
            Request Information
          </button>
        </div>

  
        <div class="stats">

          <div>
            <h2>118+</h2>
            <p>Years of Excellence</p>
          </div>

          <div>
            <h2>20+</h2>
            <p>Academic Programs</p>
          </div>

          <div>
            <h2>5,000+</h2>
            <p>Active Students</p>
          </div>

          <div>
            <h2>20+</h2>
            <p>Partner Institutions</p>
          </div>

        </div>

      </div>



      <div class="hero-image">

        <div class="image-card">

          <img
            src="../assets/cpu-logo.png"
            alt="Central Philippine University"
          />

          <h2>
            Central Philippine<br />
            University
          </h2>

          <h4>SCIENTIA ET FIDES</h4>

          <div class="small-line"></div>

          <p>
            “A Heritage of Excellence,<br />
            A Future of Faith”
          </p>

        </div>

      </div>

    </section>

  </main>
</template>

<style scoped>

.home {
  min-height: calc(100vh - 90px);
}

.hero {
  min-height: 50vh;
  display: flex;
  align-items: center;
  padding: 40px 60px;
  gap: 50px;
  box-sizing: border-box;
}



.hero-content {
  width: 50%;
}

.established {
  color: #a38427;
  font-size: 14px;
  font-weight: bold;
  letter-spacing: 2px;
  display: flex;
  align-items: center;
  gap: 15px;
}

.established span {
  width: 45px;
  height: 2px;
  background: #b59a45;
}

h1 {
  color: #29106b;
  font-family: Georgia, serif;
  font-size: 55px;
  line-height: 1.05;
  margin: 35px 0 25px;
}

h1 em {
  color: #a88724;
  font-weight: normal;
}

.gold-line {
  width: 60px;
  height: 3px;
  background: #b89a3b;
  margin-bottom: 25px;
}

.hero-content > p {
  color: #4d4d4d;
  font-size: 17px;
  line-height: 1.8;
  max-width: 600px;
}

.hero-content strong {
  color: #29106b;
}

/* BUTTONS */

.buttons {
  display: flex;
  gap: 25px;
  margin-top: 25px;
}

.primary,
.secondary {
  padding: 17px 30px;
  font-size: 15px;
  font-weight: bold;
  border-radius: 5px;
  cursor: pointer;
}

.primary {
  background: #2c096c;
  color: white;
  border: none;
}

.secondary {
  background: white;
  color: #2c096c;
  border: 2px solid #aaa;
}



.stats {
  margin-top: 35px;
  padding: 20px;
  display: flex;
  justify-content: space-around;
  background: white;
  border-radius: 12px;
  box-shadow: 0 5px 20px rgba(0,0,0,0.08);
}

.stats div {
  text-align: center;
  padding: 0 20px;
  border-right: 1px solid #ddd;
}

.stats div:last-child {
  border-right: none;
}

.stats h2 {
  color: #28106a;
  margin: 0;
  font-size: 25px;
}

.stats p {
  margin: 8px 0 0;
  font-size: 12px;
  color: #555;
}



.hero-image {
  width: 50%;
  display: flex;
  justify-content: center;
}

.image-card {
  width: 85%;
  height: 500px;
  border-radius: 20px;
  background: linear-gradient(
    135deg,
    #f1c744,
    #fffdf3 45%,
    #f7f2df
  );

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  box-shadow: 0 8px 25px rgba(0,0,0,0.12);
  text-align: center;
}

.image-card img {
  width: 150px;
  height: 150px;
  object-fit: contain;
}

.image-card h2 {
  color: #29106b;
  font-family: Georgia, serif;
  font-size: 32px;
  line-height: 1.2;
}

.image-card h4 {
  color: #a88724;
  letter-spacing: 5px;
  margin: 5px;
}

.small-line {
  width: 70px;
  height: 2px;
  background: #a88724;
  margin: 20px;
}

.image-card p {
  font-family: Georgia, serif;
  font-style: italic;
  color: #444;
  font-size: 18px;
  line-height: 1.5;
}


@media (max-width: 1000px) {

  .navbar {
    padding: 15px 25px;
  }

  .nav-links {
    gap: 12px;
  }

  .hero {
    flex-direction: column;
  }

  .hero-content,
  .hero-image {
    width: 100%;
  }

  .hero-image {
    margin-top: 30px;
  }

}

</style>