<template>
  <div>
    <headerSection/>
    <div class="about-us">
      <section class="mission-vision">
        <div class="container">
          <h2 class="section-title">Our Mission</h2>
          <p class="section-description">To create a supportive space where like-minded individuals can come together to share knowledge, collaborate on projects, and foster meaningful connections.</p>
          
          <h2 class="section-title">Our Vision</h2>
          <p class="section-description">To become a premier platform for students and professionals in our industry known for its vibrant knowledge-sharing ecosystem and its positive impact on the careers and lives of our members.</p>
        </div>
      </section>

      <section class="core-values">
        <div class="container">
          <h2 class="section-title">Our Core Values</h2>
          <div class="values">
            <!-- Your core values here -->
            <div class="value">
              <h3>Inclusivity</h3>
              <p>We welcome diverse perspectives and backgrounds, fostering an environment where everyone feels valued and respected.</p>
            </div>
            <div class="value">
              <h3>Knowledge Sharing</h3>
              <p>We believe in freely sharing knowledge and expertise to help each other grow and learn.</p>
            </div>
            <div class="value">
              <h3>Community Support</h3>
              <p>We support one another in achieving our goals, offering assistance and encouragement when needed.</p>
            </div>
            <div class="value">
              <h3>Integrity</h3>
              <p>We uphold high ethical standards and expect members to act honestly and in all interactions.</p>
            </div>
            <div class="value">
              <h3>Collaboration</h3>
              <p>We encourage collaboration and teamwork to achieve collective and individual success.</p>
            </div>
            <div class="value">
              <h3>Continuous Learning</h3>
              <p>We promote a culture of lifelong learning and personal development.</p>
            </div>
            <div class="value">
              <h3>Positive Engagement</h3>
              <p>We maintain a positive and constructive tone in our discussions and interactions.</p>
            </div>
            <div class="value">
              <h3>Innovation</h3>
              <p>We embrace new ideas and technologies to drive progress and adapt to changing needs.</p>
            </div>
          </div>
        </div>
      </section>

      <!-- Interested in joining us -->
      <section class="join-team">
  <div class="container">
    <h1 class="join-team-title" ref="typed"></h1>
    <a class="router-button" href="/register">Register</a>
  </div>
</section>
    </div>
    <footerSection/>
  </div>
</template>

<script>
import headerSection from '@/components/header.vue';
import footerSection from '@/components/footer.vue';
import Typed from 'typed.js';

export default {
  name: "AboutUs",
  components: {
    headerSection,
    footerSection
  }, 

  //Typed js
  mounted() {
    new Typed(this.$refs.typed, {
      strings: ['Interested in joining us? |'],
      typeSpeed: 50,
      loop: true, 
      showCursor: false, 
      autoInsertCss: true, 
    });
  }
}


</script>

<style scoped>
/* Font Family */
body, .section-title, .section-description, .value h3, .value p, .join-team-title {
  font-family: 'Quicksand', sans-serif;
}

/* Font Size */
.container,
.section-title,
.section-description,
.value p,
.value h3,
.join-team-title {
  font-size: 1.2rem;
}

/* Core Value Card */
.values {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.value {
  flex: 1 1 calc(33% - 20px);
  padding: 20px;
  border-radius: 8px;
  background-color: #f9f9f9;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.value:hover {
  transform: rotate(3deg);
}

/* Container */

.about-us {
  max-width: 100%; 
  margin: 0 auto;
  padding: 20px; 
  background-color: #f1f1f1;
}
.typed-cursor{
  display: inline-block;
  vertical-align: middle;
    }
/* Section Title */
.section-title {
  font-size: 2rem;
  margin-bottom: 20px;
  color: #333;
}

/* Section Description */
.section-description {
  margin-bottom: 30px;
  line-height: 1.5;
}

/* Join Team Section */
.join-team {
  text-align: center;
}

.join-team .container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.join-team-title {
  font-size: 2rem;
  height: 60px;
  overflow: hidden;
  margin-bottom: 20px;
}

.router-button {
  font-size: 14px;
  text-decoration: none;
  background-color: #0241ac;
  transition: all .5s ease;
  cursor: pointer;
  padding: 10px 20px;
  color: #fff;
  border-radius: 20px;
  border: none;
  text-transform: uppercase;
  width: 150px; 
}




</style>
