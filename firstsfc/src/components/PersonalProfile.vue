<template>
  <div>
    <header>
      <nav id="navbar">
        <div class="nav-container">
          <div class="logo">Neicha's Portfolio</div>
          <button class="hamburger" id="hamburger" aria-label="Toggle navigation">
            <span></span>
            <span></span>
            <span></span>
          </button>
          <ul class="nav-menu" id="navMenu">
            <li><a href="#about" class="nav-link active">About Me</a></li>
            <li><a href="#education" class="nav-link">Education</a></li>
            <li><a href="#hobbies" class="nav-link">Hobbies</a></li>
            <li><a href="#goals" class="nav-link">Goals</a></li>
            <li><a href="#experience" class="nav-link">IT Experience</a></li>
            <li><a href="#gallery" class="nav-link">Photo Gallery</a></li>
          </ul>
        </div>
      </nav>
    </header>

    <main>
      <!-- About Section -->
      <section id="about" class="section">
        <div class="container">
          <div class="intro-banner">
            <img
              src="https://i.pinimg.com/736x/e7/65/f1/e765f197d8a553179dfe01b4b1af6621.jpg"
              alt="Collage of Neichaela Padilla"
              class="intro-banner-image"
            />
            <div class="intro-banner-text">
              <h1>Welcome to My Portfolio!</h1>
            </div>
          </div>

          <div class="content-card">
            <div class="intro-text-block">
              <p class="intro-text">Hello! I'm Neichaela Padilla</p>
              <p>
                I am a second-year student pursuing a career in the IT industry...
              </p>
            </div>
          </div>
        </div>
      </section>

      <!-- Education Section -->
      <section id="education" class="section section-alt">
        <div class="container">
          <h2 class="section-title">Education</h2>
          <div class="content-card">
            <!-- Education items here -->
          </div>
        </div>
      </section>

      <!-- Continue with hobbies, goals, experience, gallery, references... -->
    </main>

    <footer>
      <div class="container">
        <p>&copy; 2026 Neichaela Padilla. All rights reserved.</p>
        <p class="footer-note">Built with HTML, CSS, and JavaScript</p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'PersonalProfile',
  mounted() {
    // If you had JS in js/script.js (like hamburger menu toggle),
    // move that logic here:
    const hamburger = document.getElementById('hamburger');
    const navMenu = document.getElementById('navMenu');

    if (hamburger && navMenu) {
      hamburger.addEventListener('click', () => {
        navMenu.classList.toggle('active');
      });
    }
  }
}
</script>

<script>
export default {
  name: 'PersonalProfile',
  mounted() {
    const hamburger = document.getElementById('hamburger');
    const navMenu = document.getElementById('navMenu');
    const navLinks = document.querySelectorAll('.nav-link');
    const sections = document.querySelectorAll('.section');

    // Toggle hamburger menu
    if (hamburger && navMenu) {
      hamburger.addEventListener('click', () => {
        hamburger.classList.toggle('active');
        navMenu.classList.toggle('active');
      });
    }

    // Close menu on nav link click
    navLinks.forEach(link => {
      link.addEventListener('click', () => {
        hamburger.classList.remove('active');
        navMenu.classList.remove('active');
      });
    });

    // Highlight active nav link on scroll
    const setActiveNavLink = () => {
      let currentSection = '';
      const scrollPosition = window.scrollY + 100;

      sections.forEach(section => {
        const sectionTop = section.offsetTop;
        const sectionHeight = section.offsetHeight;
        const sectionId = section.getAttribute('id');

        if (scrollPosition >= sectionTop && scrollPosition < sectionTop + sectionHeight) {
          currentSection = sectionId;
        }
      });

      navLinks.forEach(link => {
        link.classList.remove('active');
        const href = link.getAttribute('href').substring(1);
        if (href === currentSection) {
          link.classList.add('active');
        }
      });
    };

    window.addEventListener('scroll', setActiveNavLink);
    window.addEventListener('load', setActiveNavLink);

    // Animate cards on scroll
    const observer = new IntersectionObserver(
      (entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.style.opacity = '1';
            entry.target.style.transform = 'translateY(0)';
          }
        });
      },
      {
        threshold: 0.1,
        rootMargin: '0px 0px -50px 0px'
      }
    );

    const cards = document.querySelectorAll('.content-card, .hobby-card, .experience-card, .gallery-item');
    cards.forEach(card => {
      card.style.opacity = '0';
      card.style.transform = 'translateY(20px)';
      card.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
      observer.observe(card);
    });
  }
}
</script>


<style src="./css/personalprofile.css"></style>