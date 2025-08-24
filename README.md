## EX01 - PORTFOLIO
## Date:

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
 # HTML
 ```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MY PORTFOLIO</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
  <div class="container nav">
    <div class="brand">
      <h1>MY PORTFOLIO</h1>
    </div>
    <nav>
      <a href="#about">ABOUT</a>
      <a href="#skills">SKILLS</a>
      <a href="#projects">PROJECTS</a>
      <a href="#contact">CONTACT</a>
    </nav>
  </div>
</header>

<section class="hero" id="home">
  <div class="container hero-content">
    <div>
      <h2>KARTHICK KISHORE T</h2>
      <p>A passionate web developer building modern websites and apps.</p>
      <a href="#projects" class="btn">View My Work</a>
      <a href="#contact" class="btn outline">Contact Me</a>
    </div>
    <div class="avatar-wrap">
      <div class="avatar">
        <img src="kk2.jpg" alt="KARTHICK KISHORE T">
      </div>
      <div class="status">Available for Work</div>
    </div>
  </div>
</section>

<section id="about" class="section">
  <div class="container">
    <h2>ABOUT</h2>
    <p>I create responsive, user-friendly websites. I love problem-solving and learning new technologies.</p>
  </div>
</section>

<section id="skills" class="section">
  <div class="container">
    <h2>SKILLS</h2>
    <label>HTML & CSS</label><div class="bar"><span style="width:90%"></span></div>
    <label>JavaScript</label><div class="bar"><span style="width:75%"></span></div>
    <label>Python</label><div class="bar"><span style="width:60%"></span></div>
    <label>React</label><div class="bar"><span style="width:45%"></span></div>
  </div>
</section>

<section id="projects" class="section">
  <div class="container">
    <h2>PROJECTS</h2>
    <div class="grid">
      <div class="card"><img src="istockphoto-1439256518-612x612.jpg" alt="Project 1"><div class="card-pad">
        <h3>Smart Portfolio Dashboard</h3>
        <P>A responsive web dashboard that visualizes data with charts and metrics, allowing users to monitor performance in real-time.</P>
    </div></div>
      <div class="card"><img src="images (1).jpg" alt="Project 2"><div class="card-pad">
        <h3>TaskMaster App</h3>
        <p>A productivity-focused app to manage tasks, set deadlines, and track progress efficiently with an intuitive interface.</p>
    </div></div>
      <div class="card"><img src="psychedelic-swirl-groovy-pattern-psychedelic-retro-wave-wallpaper-liquid-groovy-background-design-illustration-vector.jpg" alt="Project 3"><div class="card-pad">
        <h3>Travel Explorer Website</h3>
        <p>An interactive platform for planning trips, exploring destinations, and creating personalized itineraries with maps and recommendations.</p>
    </div></div>
    </div>
  </div>
</section>

<section id="contact" class="section">
  <div class="container">
    <h2>CONTACT</h2>
    <form>
      <label>Name<input type="text" placeholder="Your Name"></label>
      <label>Email<input type="email" placeholder="Your Email"></label>
      <label>Message<textarea rows="5" placeholder="Your Message"></textarea></label>
      <button type="submit" class="btn">Send Message</button>
    </form>
  </div>
</section>

<footer>
  <div class="container footer">
    <p>&copy; 2025 KARTHICK KISHORE T. All Rights Reserved.</p>
  </div>
</footer>

</body>
</html>
```
# CSS
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Arial", sans-serif;
  line-height: 1.6;
  background: #121212;
  color: #eee;
}

.container {
  width: 90%;
  max-width: 1100px;
  margin: auto;
}

.section {
  padding: 80px 0;
}

p {
  margin-bottom: 15px;
  color: #ccc;
}

a {
  text-decoration: none;
  color: inherit;
}

.btn {
  display: inline-block;
  padding: 12px 25px;
  border-radius: 30px;
  background: #00bfff;
  color: #121212;
  font-weight: bold;
  transition: 0.3s;
  cursor: pointer;
}

.btn:hover {
  background: #009acd;
}

.btn.outline {
  background: transparent;
  border: 2px solid #00bfff;
  color: #00bfff;
}

.btn.outline:hover {
  background: #00bfff;
  color: #121212;
}

header {
  background: #1a1a1a;
  padding: 15px 0;
  position: sticky;
  top: 0;
  z-index: 10;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.5);
}

header .nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header nav a {
  margin: 0 15px;
  color: #eee;
  font-weight: bold;
}

header nav a:hover {
  color: #00bfff;
}

.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  min-height: 100vh;
  position: relative;
  background: url("istockphoto-1439256518-612x612.jpg") center/cover no-repeat;
  padding: 50px 0;
}

.hero::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.hero-content {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 100%;
  z-index: 1;
}

.hero p {
  margin: 20px 0;
  max-width: 500px;
  color: #ddd;
}

.avatar-wrap {
  text-align: center;
}

.avatar {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  overflow: hidden;
  margin: auto;
  border: 5px solid #00bfff;
  box-shadow: 0 0 20px #00bfff;
}

.avatar img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.status {
  margin-top: 10px;
  padding: 5px 15px;
  display: inline-block;
  background: #00bfff;
  color: #06050c;
  border-radius: 20px;
  font-weight: bold;
}

#about {
  text-align: center;
}

#skills {
  background: #00bfff;
  text-align: center;
}


.skills label {
  font-weight: bold;
  display: block;
  margin-top: 15px;
}

.skills .bar {
  border-radius: 20px;
  overflow: hidden;
  height: 12px;
  margin: 5px 0 10px;
}

.skills .bar span {
  display: block;
  height: 100%;
  transition: width 0.5s;
}

.projects .grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 25px;
}

.card {
  
  border-radius: 15px;
  overflow: hidden;
  box-shadow: 0 5px 20px rgba(0, 191, 255, 0.2);
  transition: all 0.3s;
}

.card:hover {
  transform: translateY(-10px);
  box-shadow: 0 10px 30px rgba(8, 211, 242, 0.953);
}

.card img {
  width: 100%;
  height: 180px;
  object-fit: cover;
}

.card-pad {
  padding: 20px;
}

form {
  max-width: 500px;
  margin: auto;
  display: flex;
  flex-direction: column;
}

form label {
  margin-bottom: 15px;
  font-weight: bold;
  color: #eee;
}

form input,
form textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #090202;
  border-radius: 10px;
  background: #0aade4;
  color: #0f0202;
  margin-top: 5px;
}

form input:focus,
form textarea:focus {
  outline: none;
  border-color: #000405;
}

form button {
  margin-top: 15px;
  padding: 12px;
  font-size: 1rem;
}

footer {
  background: #ee2626;
  color: #120404;
  text-align: center;
  background: url("images.jpg") center/cover no-repeat;
  padding: 25px 0;
  border-top: 1px solid #f10d0d;
}
```


## OUTPUT
<img width="1918" height="1078" alt="Screenshot 2025-08-17 144028" src="https://github.com/user-attachments/assets/f3a762c9-0462-43bd-95b0-aa0a8de422c6" />
<img width="1918" height="1078" alt="Screenshot 2025-08-17 144201" src="https://github.com/user-attachments/assets/933819a0-af87-437d-aa98-6f284e5094cc" />
<img width="1918" height="1078" alt="Screenshot 2025-08-17 144256" src="https://github.com/user-attachments/assets/28d64de4-bba3-4421-b7ae-fe1086b143b1" />
<img width="1918" height="1078" alt="Screenshot 2025-08-17 144359" src="https://github.com/user-attachments/assets/d516dbe7-8841-4bab-bf36-23ee161b8ec0" />



## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
