# Ex01 Portfolio
## Date: 31/8/2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <link rel="stylesheet" href="ex1.css">
</head>
<body>
  <!-- Header -->
  <header>
    <nav class="navbar">
      <div class="logo">My Portfolio</div>
      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a href="resume.pdf" target="_blank">Resume</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <div class="hero-content">
      <img src="photo.jpg" alt="My Photo" class="hero-photo">
      <h1>Hi, I'm <span class="highlight">Muthulakshmi D</span></h1>
      <p>Pre-final year Computer Science student</p>
      <div class="hero-actions">
        <a href="#projects" class="btn btn-primary">View Projects</a>
        <a href="resume.pdf" class="btn btn-secondary">View Resume</a>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="about">
    <h2>About Me</h2>
    <p>
      Hello! I’m Muthulakshmi, a passionate and curious Computer Engineering student with a strong interest in programming, web development, and problem-solving. I love turning ideas into real-world solutions using technologies like C, Python, Java, SQL, and modern frontend frameworks (HTML, CSS, JavaScript).
I am also fascinated by UI/UX design, and I enjoy creating interfaces that are not only functional but also intuitive and visually appealing. I thrive on challenges and continuously seek opportunities to learn, innovate, and contribute to meaningful projects.
When I’m not coding, I’m exploring emerging tech trends, experimenting with small projects, and improving my design and development skills. I aim to build solutions that make a real impact while constantly growing as a developer and problem solver.
    </p>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="projects">
    <h2>My Projects</h2>
    <div class="project-list">
      <div class="project-card">
        <h3>Project One</h3>
        <p>Personal Portfolio Website</p>
      </div>
      <div class="project-card">
        <h3>Project Two</h3>
        <p>Image Gallery</p>
      </div>
      <div class="project-card">
        <h3>Project Three</h3>
        <p>E-commerce Website</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact">
    <h2>Contact Me</h2>
    <p>Email: <a href="mailto:mmuthulakshmi063@gmail.com">mmuthulakshmi063@gmail.com</a></p>
    <p>LinkedIn: <a href="#">linkedin.com/in/muthulakshmid</a></p>
    <p>GitHub: <a href="#">github.com/MuthulakshmiD</a></p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 Muthulakshmi D | Register No: 212223040122</p>
  </footer>
</body>
</html>
```
```/* ---------------- Reset ---------------- */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}

body {
  line-height: 1.6;
  background: #f9f9f9;
  color: #333;
}

/* ---------------- Navbar ---------------- */
header {
  background: #333;
  color: #fff;
  padding: 10px 20px;
}
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.nav-links {
  list-style: none;
  display: flex;
}
.nav-links li {
  margin-left: 20px;
}
.nav-links a {
  color: #fff;
  text-decoration: none;
  transition: 0.3s;
}
.nav-links a:hover {
  color: #ff9800;
}

/* ---------------- Hero ---------------- */
.hero {
  background: #222;
  color: #fff;
  height: 70vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-direction: column;
  padding: 20px;
}
.hero-photo {
  width: 160px;
  height: 160px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 20px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.3);
}
.hero h1 {
  font-size: 2.5rem;
}
.hero .highlight {
  color: #ff9800;
}
.hero-actions {
  margin-top: 20px;
}

/* ---------------- Buttons (Outlined) ---------------- */
.btn {
  background: transparent;       
  border: 2px solid #ff9800;    
  color: #ff9800;                
  padding: 10px 20px;
  border-radius: 5px;
  text-decoration: none;
  margin: 5px;
  display: inline-block;
  transition: 0.3s;
  font-weight: 500;
}
.btn:hover {
  background: #ff9800;           
  color: #fff;                   
}

/* ---------------- Sections ---------------- */
section {
  padding: 50px 20px;
  text-align: center;
}
.projects {
  background: #eee;
}
.project-list {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}
.project-card {
  background: #fff;
  padding: 20px;
  border-radius: 10px;
  width: 250px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  transition: 0.3s;
}
.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 12px rgba(0,0,0,0.2);
}

/* ---------------- Footer ---------------- */
footer {
  background: #333;
  color: #fff;
  text-align: center;
  padding: 15px 0;
}

/* ---------------- Responsive ---------------- */
@media (max-width: 768px) {
  .nav-links {
    flex-direction: column;
    gap: 10px;
  }
  .hero h1 {
    font-size: 2rem;
  }
  .project-list {
    flex-direction: column;
    align-items: center;
  }
}
```
## OUTPUT
<img width="1919" height="925" alt="image" src="https://github.com/user-attachments/assets/a827b5c3-3797-44b9-a839-df77ac63acd7" />
<img width="1919" height="979" alt="image" src="https://github.com/user-attachments/assets/47c97be8-8a02-459a-9661-3fdb3d58ec59" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
