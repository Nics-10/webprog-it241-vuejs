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
            <li><a href="#references" class="nav-link">References</a></li>
          </ul>
        </div>
      </nav>
    </header>

    <main>
      <section id="about" class="section">
        <div class="container">
          <div class="intro-banner">
            <img src="https://i.pinimg.com/736x/e7/65/f1/e765f197d8a553179dfe01b4b1af6621.jpg" alt="Collage of Neichaela Padilla" class="intro-banner-image" />
            <div class="intro-banner-text">
              <h1>Welcome to My Portfolio!</h1>
            </div>
          </div>
          <div class="content-card">
            <div class="intro-text-block">
              <p class="intro-text">Hello! I'm Neichaela Padilla</p>
              <p>
                I am a second-year student pursuing a career in the IT industry. One of my dreams is to work
                in the corporate world, where I can explore and improve myself in terms of both social and
                personal skills. I believe that this path will take me to many opportunities because as long
                as technology continues to evolve, IT professionals will always be in demand. I simply want
                to live my life to the fullest and be content with what I have.
              </p>
            </div>
          </div>
        </div>
      </section>

      <section id="education" class="section section-alt">
        <div class="container">
          <h2 class="section-title">Education</h2>
          <div class="content-card">
            <div class="education-item">
              <h3>College Degree</h3>
              <p class="subtitle">Asia Pacific College | 2024 – Present</p>
              <p>
                Currently pursuing a Bachelor of Science in Information Technology, where I am developing
                skills and knowledge in software development, networking, database management, and system
                administration.
              </p>
            </div>
            <div class="education-item">
              <h3>TESDA Certification</h3>
              <p class="subtitle">Computer System Servicing NC II</p>
              <p>
                Successfully completed the Computer System Servicing NC II certification, demonstrating
                proficiency in hardware troubleshooting, system maintenance, and technical support.
              </p>
            </div>
            <div class="education-item">
              <h3>Senior High School</h3>
              <p class="subtitle">SHS in San Nicholas III, Bacoor City, Cavite | 2022 – 2024</p>
              <p>
                Completed senior high school education under the Information and Communication Technology
                (ICT) – TVL Strand, gaining foundational training and academic preparation for higher studies
                in the field of Information Technology. Graduated with High Honors.
              </p>
            </div>
          </div>
        </div>
      </section>

      <section id="hobbies" class="section">
        <div class="container">
          <h2 class="section-title">Hobbies & Interests</h2>
          <div class="grid-container">
            <div class="hobby-card">
              <div class="hobby-icon">🏞️</div>
              <h3>Outdoor Adventure</h3>
              <p>Exploring nature and embracing the great outdoors through hiking and outdoor activities.</p>
            </div>
            <div class="hobby-card">
              <div class="hobby-icon">💃</div>
              <h3>Dancing</h3>
              <p>Expressing creativity and staying active through various dance styles and movements.</p>
            </div>
            <div class="hobby-card">
              <div class="hobby-icon">🎮</div>
              <h3>Online Gaming</h3>
              <p>Engaging in strategic and competitive online games, building teamwork and problem-solving skills.</p>
            </div>
            <div class="hobby-card">
              <div class="hobby-icon">🐱</div>
              <h3>Playing with My Cat</h3>
              <p>Spending quality time with my feline companion, enjoying the simple joys of pet companionship.</p>
            </div>
          </div>
        </div>
      </section>

      <section id="goals" class="section section-alt">
        <div class="container">
          <h2 class="section-title">Goals</h2>
          <div class="content-card">
            <blockquote class="goal-quote">
              "My goal is to live my life to the fullest so I won't live with regrets."
            </blockquote>
            <p>This quotes drives everything I do. I believe in:</p>
            <ul class="goal-list">
              <li>Never let someone else's opinion becomes your reality</li>
              <li>Every challenge has an opportunity hidden inside it</li>
              <li>Buhay ay 'di karera</li>
            </ul>
          </div>
        </div>
      </section>

      <section id="experience" class="section">
        <div class="container">
          <h2 class="section-title">IT Experience</h2>
          <div class="experience-grid">
            <div class="experience-card">
              <h3>Basic Programming Skills</h3>
              <p>Proficient in fundamental programming concepts and multiple programming languages, with the ability to develop functional applications and solve computational problems.</p>
            </div>
            <div class="experience-card">
              <h3>Networking</h3>
              <p>Understanding of network infrastructure, protocols, and configuration. Capable of setting up and maintaining network systems for optimal performance.</p>
            </div>
            <div class="experience-card">
              <h3>Troubleshooting</h3>
              <p>Strong diagnostic skills in identifying and resolving hardware and software issues. Systematic approach to problem-solving in various IT environments.</p>
            </div>
            <div class="experience-card">
              <h3>Computer System Servicing</h3>
              <p>TESDA NC II certified in computer system servicing, with hands-on experience in hardware maintenance, system installation, and technical support.</p>
            </div>
          </div>
        </div>
      </section>

      <section id="gallery" class="section section-alt">
        <div class="container">
          <h2 class="section-title">Photo Gallery</h2>
          <div class="gallery-grid">
            <div class="gallery-item">
              <img src="https://i.pinimg.com/736x/68/cb/7c/68cb7c5cf6f468f6a7801aef529be863.jpg" alt="My Cats" loading="lazy" />
            </div>
            <div class="gallery-item">
              <img src="https://i.pinimg.com/736x/5a/42/1b/5a421b327d4229bf02a95df9000df648.jpg" alt="My Friends" loading="lazy" />
            </div>
            <div class="gallery-item">
              <img src="https://i.pinimg.com/736x/2c/17/3d/2c173d25154b1e0a2261dab7b2e7f780.jpg" alt="My Family" loading="lazy" />
            </div>
            <div class="gallery-item">
              <img src="https://i.pinimg.com/736x/f0/e5/35/f0e5357b3fb50d64c8eb87a51a1f0c18.jpg" alt="BINI" loading="lazy" />
            </div>
            <div class="gallery-item">
              <img src="https://i.pinimg.com/736x/06/4c/cc/064ccc2bf3094fd15354941d13f5b6e2.jpg" alt="BlackPink" loading="lazy" />
            </div>
          </div>
        </div>
      </section>

      <section id="references" class="section references-section">
        <div class="container">
          <h2 class="section-title">References & Credits</h2>
          <div class="references-grid">
            <div class="reference-card">
              <h3>Fonts</h3>
              <p>Inter from Google Fonts</p>
            </div>
            <div class="reference-card">
              <h3>Images</h3>
              <p>All images are owned by the developer</p>
            </div>
            <div class="reference-card">
              <h3>Icons</h3>
              <p>Unicode emoji characters</p>
            </div>
            <div class="reference-card">
              <h3>Code Validation</h3>
              <p>W3C HTML Validator and CSS Validator</p>
            </div>
            <div class="reference-card">
              <h3>Development Tools</h3>
              <p>Visual Studio Code, modern web browsers for testing</p>
            </div>
            <div class="reference-card">
              <h3>AI Usage Documentation</h3>
              <p>This website was assisted with AI technology. The AI helped in fixing the format for a cleaner experience for viewers. The creative direction, content, and personal input were entirely provided by the website owner.</p>
            </div>
          </div>
        </div>
      </section>
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
    const hamburger = document.getElementById('hamburger');
    const navMenu = document.getElementById('navMenu');
    const navLinks = document.querySelectorAll('.nav-link');
    const sections = document.querySelectorAll('.section');

    if (hamburger && navMenu) {
      hamburger.addEventListener('click', () => {
        hamburger.classList.toggle('active');
        navMenu.classList.toggle('active');
      });
    }

    navLinks.forEach(link => {
      link.addEventListener('click', () => {
        hamburger.classList.remove('active');
        navMenu.classList.remove('active');
      });
    });

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

    const observer = new IntersectionObserver(
      (entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.style.opacity = '1';
            entry.target.style.transform = 'translateY(0)';
          }
        });
      },
      { threshold: 0.1, rootMargin: '0px 0px -50px 0px' }
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
