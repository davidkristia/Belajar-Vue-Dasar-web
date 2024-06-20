<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <img alt="University logo" class="logo" src="./assets/image.png" />
    <nav>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#departments">Departments</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="intro">
      <HelloWorld msg="Welcome to the DEL institute Technology!" />
    </section>
    <section class="welcome">
      <TheWelcome />
    </section>
  </main>

  <footer>
    <p>&copy; 2024 University Name. All rights reserved.</p>
  </footer>
</template>

<style scoped>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
}

header {
  background-color: #2a85e0;
  color: white;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
}

.logo {
  width: 100px;
  height: auto;
}

nav {
  flex-grow: 1;
}

.nav-links {
  list-style: none;
  display: flex;
  justify-content: flex-end;
  margin: 0;
  padding: 0;
}

.nav-links li {
  margin-left: 2rem;
}

.nav-links a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

.nav-links a:hover {
  text-decoration: underline;
}

.intro, .welcome {
  padding: 2rem;
  margin: 0 auto;
  max-width: 1200px;
}

.intro {
  background-color: white;
  text-align: center;
  margin-bottom: 2rem;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.welcome {
  background-color: #e9ecef;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

footer {
  background-color: #004080;
  color: white;
  text-align: center;
  padding: 1rem 0;
  /* position: fixed; */
  width: 100%;
  bottom: 0;
  left: 0;
}
</style>
