<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>8SIDEE Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Fredoka One', cursive;
      background: linear-gradient(to bottom, white 0%, #0d1b2a 100%);
      color: black;
      overflow-x: hidden;
    }

    header {
      padding: 50px 20px;
      text-align: center;
      color: black;
    }

    section {
      padding: 40px 20px;
      max-width: 1100px;
      margin: auto;
      opacity: 0;
      transform: translateY(50px);
      transition: all 1s ease-in-out;
    }

    section.visible {
      opacity: 1;
      transform: translateY(0);
    }

    h2 {
      font-size: 2rem;
      margin-bottom: 20px;
      color: black;
    }

    p, li {
      font-size: 1.1rem;
      color: black;
      line-height: 1.6;
    }

    ul {
      padding-left: 20px;
    }

    ul li {
      margin: 10px 0;
    }

    a {
      color: #4b8bd5;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: rgba(0, 0, 0, 0.05);
      color: rgb(105, 4, 236);
      font-size: 0.9rem;
      margin-top: 40px;
    }
  </style>
</head>
<body>

<header>
  <h1>8SIDEE's Roblox Game Development Portfolio</h1>
</header>

<section id="about">
  <h2>About Me</h2>
  <p>Hi, I'm <strong>8SIDEE</strong>, a passionate Roblox game developer with over 6 years of experience in the game development industry. Throughout my journey, I've honed my skills in creating high-quality, engaging, and immersive games that captivate players and encourage long-term involvement. My expertise spans across multiple aspects of game creation, including game design, scripting, user interface design, and asset creation.</p>
  
  <p>In addition to developing games, I have contributed to the Roblox platform in various ways, including as a tester, collaborator, and active community member. I've played a pivotal role in projects that have accumulated a total of over <strong>590 million visits</strong>, which speaks to the effectiveness of my work in delivering engaging experiences. My focus is not just on creating smooth gameplay but also on fostering positive player communities and designing experiences that keep players coming back.</p>

  <p>I specialize in building immersive worlds that transport players into new adventures, integrating interactive gameplay mechanics, and ensuring that my creations are both fun and rewarding. Beyond just game mechanics, I strive to optimize every detail of my games, from performance to visual aesthetics, ensuring that they run smoothly on all devices.</p>

  <p>Through my years of experience, I’ve developed a keen eye for what works and what doesn’t, always refining my projects to create the most polished and enjoyable experiences possible. Whether I'm working solo or collaborating with other developers, I am always eager to push the boundaries of what’s possible within Roblox.</p>
</section>

<section id="services">
  <h2>Services</h2>
  <ul>
    <li>Game Development</li>
    <li>UI/UX Design</li>
    <li>SFX & Audio</li>
    <li>Game Testing & Feedback</li>
  </ul>
</section>

<section id="games">
  <h2>Featured Games</h2>
  <p><a href="https://www.roblox.com/games/10924916839/Bee-Factory-Tycoon">Bee Factory Tycoon</a> – Build and expand your honey empire!</p>
  <p><a href="https://www.roblox.com/games/119136010018221/Plants-Evolution-WORLD5">Plants Evolution WORLD5</a> – Evolve unique plants in this creative simulator.</p>
  <p>And many more...</p>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>Message me on Discord: <strong>8sidee</strong></p>
</section>

<footer>
  <p>All Rights Reserved! &copy; 2025 8SIDEE</p>
</footer>

<script>
  function revealOnScroll() {
    const sections = document.querySelectorAll("section");
    for (let i = 0; i < sections.length; i++) {
      const windowHeight = window.innerHeight;
      const elementTop = sections[i].getBoundingClientRect().top;
      const revealPoint = 150;

      if (elementTop < windowHeight - revealPoint) {
        sections[i].classList.add("visible");
      }
    }
  }

  window.addEventListener("scroll", revealOnScroll);
  window.addEventListener("load", revealOnScroll);
</script>

</body>
</html>
