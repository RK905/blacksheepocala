<template>
  <div class="about">
    <section class="about-section">
      <h1 class="about-section-title">OUR HISTORY</h1>
      <p class="about-section-desc">Much More Than Your Regular Gastropub</p>
      <p class="about-section-content">
        The Black Sheep on Broadway is an established Gastropub that aims to
        build community by providing drinks that bring people together and an
        atmosphere that is a hub for local entertainment. Our approach to
        delivering only the finest service to our customers starts and ends with
        our constant desire to exceed expectations. Come join us to see what
        we’re all about.
      </p>
    </section>
    <section class="about-section">
      <div class="about-owner">
        <div class="about-owner-image"></div>
        <div class="about-owner-desc">
          <h2 class="about-owner-title">The Owners</h2>
          <p class="about-owner-content">
            Amy & Meigan met in 2011, both working in downtown Ocala at 2 local
            bars. Their love for the service industry gave them the idea to come
            together to open a gastropub where everyone is welcome and can enjoy
            their experience. "We love our staff & our customers. We thrive to
            bring a comfortable and fun environment at the Black Sheep"
          </p>
        </div>
      </div>
    </section>
  </div>
</template>
<style scoped>
.about {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 2rem;
}

.about-section {
  margin-bottom: 3rem;
}

.about-section-title {
  font-size: 40px;
  text-align: center;
  text-transform: uppercase;
}

.about-section-desc {
  font-size: 18px;
  line-height: 1.75em;
  text-align: center;
  margin-top: 2rem;
  margin-bottom: 1rem;
}

.about-section-content {
  font-size: 15px;
  line-height: 1.875em;
  text-align: center;
}

.about-owner {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.about-owner-image {
  background-image: url("https://static.wixstatic.com/media/6b30aa_b130b7ffeec14252990991e23339f600~mv2.jpg/v1/fill/w_1277,h_1117,fp_0.50_0.50,q_85,enc_auto/6b30aa_b130b7ffeec14252990991e23339f600~mv2.jpg");
  background-size: cover;
  background-position: center;
  width: 490px;
  height: 560px;
  max-width: 100%;
  aspect-ratio: 16/9;
  margin-right: 2rem;
}

.about-owner-desc {
  flex: 1;
  display: flex;
  flex-direction: column;
}

.about-owner-title {
  font-size: 20px;
  line-height: 1.67em;
  text-align: center;
  margin-bottom: 1rem;
}

.about-owner-content {
  font-size: 15px;
  line-height: 1.875em;
  text-align: center;
}
</style>
