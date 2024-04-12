<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-content">

        <!-- Footer navigation -->
        <div>
          <h2>Embedded Developer Community</h2>
          <nav class="footer-navigation">
            <ul>
              <li><router-link to="/">HOME</router-link></li>
              <li><router-link to="/login">LOGIN</router-link></li>
              <li><router-link to="/projects">PROJECTS</router-link></li>
              <li><router-link to="/team">OUR TEAM</router-link></li>
              <li><router-link to="/contact">CONTACT US</router-link></li>
            </ul>
          </nav>
        </div>
        <!-- Footer text -->
        <div class="right">
        <p class="footer-text">&copy; 2024 Embedded Developer Community.</p>
        <br>
        <p class="footer-text">All Right Reserved.</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'footerSection'
}
</script>

<style scoped>
.right  {
    align-items: flex-end;
}
.footer {
  background-color: #0241ac;
  min-height: 0px;
}

.container {
  max-width: 1301px;
  margin: 0 auto;
  padding: 45px 25px;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.footer-navigation ul {
  list-style: none;
  flex-direction: column;
  display: flex;
  color: #fff;
  font-family: Quicksand, san-serif;
  font-weight: bold;
  flex-direction: right;
}

.footer-navigation ul li {
  margin-right: 20px;
  padding-bottom: 20px;

}

.footer-navigation ul li:last-child {
  margin-right: 0;
}

.footer-navigation ul li a {
  text-decoration: none;
  color: white;
}

.footer p {
  font-size: 14px;
  font-family: 'Quicksand', sans-serif;
}
.footer-text{
  color: white;
  font-size: 15px;
}
h2, p{
  font-family: Quicksand, san-serif;
}
h2{
  color: white; 
  font-size: 1.5rem;
}
</style>
