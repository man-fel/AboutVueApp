<template>
  <header class="header">
    <div class="container">
      <!-- Logo -->
      <div class="logo">
        <img src="" alt="Africa LoRa-LoRaWAN">
      </div>
      
      <!-- Navigation items -->
      <nav class="navigation">
        <ul>
          <li><router-link to="/"><strong>HOME</strong></router-link></li>
          <li><router-link to="/about"><strong>ABOUT</strong></router-link></li>
          <li><router-link to="/team"><strong>OUR TEAM</strong></router-link></li>
          <li><router-link to="/projects"><strong>PROJECTS</strong></router-link></li>
          <li><router-link to="/login"><strong>LOGIN</strong></router-link></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'headerSection'
}
</script>

<style scoped>
.header {
  height: 80px;
  box-shadow: 0 4px 6px -1px rgba(0,0,0,.1), 0 2px 4px -1px rgba(0,0,0,.06);
  z-index: 99;
  }
.container {
  max-width: 1211px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.navigation ul {
  list-style: none;
  display: flex;
  align-items: center;
  font-family: Quicksand, san-serif;
}

.navigation ul li {
  margin-right: 32px !important;
  padding-top: 15px;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

.navigation ul li:last-child {
  margin-right: 0;
}

.navigation ul li a {
  font-family: 'Quicksand', sans-serif;
  text-decoration: none;
  color: #333;
  font-size: 1rem;
}

.navigation ul li:not(:last-child) {
  margin-right: 15px;
}
</style>
