# portfolio 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Mansi Shinde - Digital Portfolio</title>
  <link rel="stylesheet" href="HELLO.CSS"/>
  <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
</head>
<body>
  <header>
    <h1>Mansi Shinde</h1>
    <p>First-Year Computer Engineering Student | Passionate Coder</p>
  </header>

  <nav>
    <a href="#home" onclick="showSection('home')">Home</a>
    <a href="#about" onclick="showSection('about')">About</a>
    <a href="#certifications" onclick="showSection('certifications')">Certifications</a>
    <a href="#strengths" onclick="showSection('strengths')">Strengths</a>
    <a href="#goals" onclick="showSection('goals')">Goals</a>
    <a href="#projects" onclick="showSection('projects')">Projects</a>
    <a href="#contact" onclick="showSection('contact')">Contact</a>
  </nav>

  <main>
    <section id="home" class="active">
      <h2>Welcome to My Portfolio</h2>
      <p>Explore my work, skills, and passion for building innovative tech solutions. I'm excited to share my journey with you!</p>
    </section>

    <section id="about">
      <h2>About Me</h2>
      <p>Hi, I'm <strong>Mansi Shinde</strong>, a first-year Computer Engineering student at MITAOE. I'm passionate about <strong>coding</strong> and love exploring the world of software and hardware. I aim to work in a <strong>software-based company</strong> and make a meaningful impact through technology. I'm a great team player and eager to learn and grow.</p>
      <h3>Skills</h3>
      <ul>
        <li>Python</li>
        <li>C</li>
        <li>HTML (Basic)</li>
        <li>Betaflight (Basic - Drone Club)</li>
        <li>Teamwork & Collaboration</li>
      </ul>
    </section>

    <section id="certifications">
      <h2>Certifications</h2>
      <ul>
        <li>NASSCOM Future Skills Prime - Python Basics</li>
        <li>CISCO Introduction to Cybersecurity</li>
        <li>Design Thinking Workshop</li>
        <li>Drone Basics - Internal Club Certification</li>
      </ul>
    </section>

    <section id="strengths">
      <h2>Strengths</h2>
      <ul>
        <li>Quick Learner</li>
        <li>Team Player</li>
        <li>Curious & Creative Thinker</li>
        <li>Problem Solving Attitude</li>
        <li>Organized and Responsible</li>
      </ul>
    </section>

    <section id="goals">
      <h2>Goals</h2>
      <ul>
        <li>Get internship experience in web or software development by 2nd year</li>
        <li>Master DSA and contribute to open-source projects</li>
        <li>Build a strong resume with impactful projects</li>
        <li>Secure placement in a top tech company post-graduation</li>
        <li>Continuously upskill with certifications and workshops</li>
      </ul>
    </section>

    <section id="projects">
      <h2>Projects</h2>
      <div class="project">
        <h3>Smart Soil Moisture Control System</h3>
        <p>Design Thinking project: A group-based system that automates plant watering using soil moisture sensors to prevent over- or under-watering.</p>
      </div>
      <div class="project">
        <h3>Hackathon: Smart Attendance Tracker</h3>
        <p>Built for a hackathon: Smart Attendance & Engagement Tracker using QR code, face recognition, Firebase integration, and a responsive webpage.</p>
      </div>
      <div class="project">
        <h3>Data Warehouse Model</h3>
        <p>Designed a dimensional model for a pathology lab including dimensions, facts, schema diagrams, and SQL queries.</p>
      </div>
      <div class="project">
        <h3>Portfolio Website</h3>
        <p>This responsive website you're currently browsing, built with HTML and CSS!</p>
      </div>
    </section>

    <section id="contact">
      <h2>Contact Me</h2>
      <form>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <label for="message">Message:</label>
        <textarea id="message" name="message" rows="4" required></textarea>

        <button type="submit">Send</button>
      </form>

      <p><strong>Email:</strong> mansikviit@gmail.com</p>
      <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/mansi-shinde-a16190324" target="_blank">linkedin.com/in/mansi-shinde-a16190324</a></p>
      <p><strong>Phone:</strong> 9930334436</p>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Mansi Shinde</p>
  </footer>

  <script>
    function showSection(id) {
      document.querySelectorAll('section').forEach(sec => sec.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>
</body>
</html>


/* General styles */
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background-color: #f2f2f2;
  color: #333;
  line-height: 1.6;
  transition: background-color 0.3s, color 0.3s;
}

header {
  background-color: #3f51b5;
  color: white;
  text-align: center;
  padding: 2rem 1rem;
  transition: background-color 0.3s ease;
}

header h1 {
  margin: 0;
  font-size: 2.5rem;
}

nav {
  display: flex;
  justify-content: center;
  background-color: #283593;
  flex-wrap: wrap;
  transition: background-color 0.3s ease;
}

nav a {
  color: white;
  padding: 1rem;
  text-decoration: none;
  transition: background-color 0.3s ease;
}

nav a:hover {
  background-color: #1a237e;
}

main {
  max-width: 1000px;
  margin: auto;
  padding: 2rem;
}

/* Section control */
section {
  display: none;
  animation: fadeIn 1s ease-in-out;
}

section.active {
  display: block;
}

/* Project section styling */
.project {
  background-color: white;
  border-left: 5px solid #3f51b5;
  margin: 1rem 0;
  padding: 1rem;
  border-radius: 5px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  transition: box-shadow 0.3s ease;
}

.project:hover {
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
}

/* Contact form styling */
form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

input, textarea, button {
  padding: 0.75rem;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  background-color: #3f51b5;
  color: white;
  border: none;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #1a237e;
}

/* Footer */
footer {
  text-align: center;
  padding: 1rem;
  background-color: #3f51b5;
  color: white;
  margin-top: 2rem;
}

/* Dark Mode styles */
body.dark-mode {
  background-color: #121212;
  color: #f5f5f5;
}

header.dark-mode {
  background-color: #1e1e1e;
}

nav.dark-mode {
  background-color: #212121;
}

.project.dark-mode {
  background-color: #2c2c2c;
  border-left: 5px solid #3f51b5;
}

footer.dark-mode {
  background-color: #1e1e1e;
}

/* Dark Mode Button */
.dark-mode-toggle {
  position: fixed;
  top: 20px;
  right: 20px;
  background-color: #3f51b5;
  color: white;
  border: none;
  padding: 10px 15px;
  font-size: 1rem;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.dark-mode-toggle:hover {
  background-color: #1a237e;
}

/* Responsive layout */
@media (max-width: 768px) {
  nav {
    flex-direction: column;
  }

  header h1 {
    font-size: 2rem;
  }

  main {
    padding: 1rem;
  }
}

/* Fade In Animation */
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
