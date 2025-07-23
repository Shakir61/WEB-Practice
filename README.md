<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Shakir Ullah | Frontend Developer</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>

  <header>
    <h1>Shakir Ullah</h1>
    <p>Frontend Web Developer & Email Marketer</p>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h2>About Me</h2>
    <p>I’m a passionate Frontend Web Developer and Email Marketer with a strong eye for design and performance. I build user-friendly, responsive websites and create engaging email campaigns that drive results. Let’s build something great together!</p>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
      <li>Email Marketing</li>
    </ul>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <p>Coming Soon! 🚀</p>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:shakirullah5467@gmail.com">shakirullah5467@gmail.com</a></p>
    <p>LinkedIn: <a href="https://www.linkedin.com/in/shakir-ullah-08362b34" target="_blank">Visit my LinkedIn</a></p>
  </section>

  <footer>
    <p>© 2025 Shakir Ullah. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  background-color: #f9f9f9;
  color: #333;
  padding: 20px;
}

header {
  text-align: center;
  background-color: #333;
  color: white;
  padding: 40px 20px;
}

nav {
  display: flex;
  justify-content: center;
  background-color: #444;
  padding: 10px 0;
}

nav a {
  color: white;
  margin: 0 15px;
  text-decoration: none;
  font-weight: bold;
}

nav a:hover {
  text-decoration: underline;
}

section {
  padding: 40px 20px;
  max-width: 800px;
  margin: auto;
}

ul {
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
  justify-content: center;
  padding: 20px 0;
}

li {
  background-color: #eee;
  padding: 10px 20px;
  border-radius: 5px;
  font-weight: bold;
}

footer {
  text-align: center;
  padding: 20px;
  background-color: #333;
  color: white;
  margin-top: 30px;
}

/* Responsive */
@media (max-width: 600px) {
  nav {
    flex-direction: column;
  }
  ul {
    flex-direction: column;
    align-items: center;
  }
}

// Scroll to section smoothly
document.querySelectorAll('nav a').forEach(link => {
  link.addEventListener('click', function(e) {
    e.preventDefault();
    const section = document.querySelector(this.getAttribute('href'));
    section.scrollIntoView({ behavior: 'smooth' });
  });
});
