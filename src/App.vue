<template>
  <div id="app">
    <header>
      <img
        class="logo"
        src="https://static.wixstatic.com/media/6b30aa_ad918f60e0484e94ae0cfc23b827035b~mv2.jpg/v1/fill/w_160,h_160,al_c,q_80,usm_0.66_1.00_0.01,enc_auto/66499974_491157081693748_528303961925484.jpg"
        alt="Logo"
      />
    </header>
    <nav class="nav-bar">
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/menu">Menu</router-link></li>
        <li><router-link to="/contact">Contact</router-link></li>
        <li><router-link to="/events">Events</router-link></li>
        <li><router-link to="/about">About Us</router-link></li>
        <li><router-link to="/instagram">Instagram</router-link></li>
      </ul>
    </nav>
    <router-view />
    <section class="hours">
      <h2>Hours</h2>
      <ul>
        <li>Monday - Closed</li>
        <li>Tuesday - Thursday: 11am - Midnight</li>
        <li>Friday & Saturday: 11am - 2am</li>
        <li>Sunday - 11am - 10pm</li>
      </ul>
    </section>
  </div>
</template>

<style>
.home-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}

.nav-bar {
  display: flex;
  justify-content: center;
  background-color: #f8f8f8;
  padding: 10px;
  margin-bottom: 20px;
}

.nav-bar ul {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}

.nav-bar li {
  margin-right: 20px;
}

.nav-bar li:last-child {
  margin-right: 0;
}

.logo {
  display: block;
  margin: 0 auto;
  width: 80px;
  height: 80px;
}
.hours {
  margin: 20px 0;
}

.hours h2 {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}

.hours ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.hours li {
  font-size: 18px;
  margin-bottom: 5px;
}
</style>
