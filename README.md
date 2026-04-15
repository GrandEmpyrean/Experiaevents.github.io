
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />

<title>Experia Events Portfolio</title>

<!-- GOOGLE FONT -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;700&display=swap" rel="stylesheet">

<style>
:root {
  --primary: #0d6efd;
  --accent: #2ec4b6;
  --text: #333;
  --muted: #666;
  --bg: #f5f7fa;
  --white: #fff;
}

/* RESET */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* BASE */
body {
  font-family: 'Poppins', sans-serif;
  background: var(--bg);
  color: var(--text);
  line-height: 1.6;
  transition: background 0.3s ease, color 0.3s ease;
}

/* HEADER (UPDATED) */
header {
  position: relative;
  background: #e9ecef; /* contrast background like logo */
  text-align: center;
  padding: 100px 20px 70px;
}

/* LOGO */
.logo {
  font-size: 4rem;
  font-weight: 800;
  letter-spacing: -2px;
  color: #000;
  text-transform: lowercase;
}

/* SPECIAL X STYLE */
.logo .x {
  background: linear-gradient(135deg, #1aa6a6 50%, #7fc7c9 50%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: 900;
}

/* TAGLINE */
header p {
  margin-top: 10px;
  font-size: 1.4rem;
  font-weight: 600;
  color: #111;
  letter-spacing: 1px;
}

/* DARK MODE HEADER */
body.dark header {
  background: #000;
}

body.dark .logo {
  color: #fff;
}

body.dark header p {
  color: #ddd;
}

/* DARK MODE BUTTON */
#theme-toggle {
  position: absolute;
  top: 20px;
  right: 20px;
  border: none;
  background: #eee;
  padding: 8px 12px;
  border-radius: 8px;
  cursor: pointer;
  font-size: 1rem;
}

/* CONTAINER */
.container {
  max-width: 1100px;
  margin: auto;
  padding: 30px 20px;
}

/* SECTION TITLE */
.section-title {
  text-align: center;
  margin-bottom: 30px;
}

.section-title h2 {
  font-size: 1.6rem;
}

.section-title p {
  font-size: 0.95rem;
  color: var(--muted);
}

/* GRID */
.grid {
  display: grid;
  gap: 20px;
  grid-template-columns: 1fr;
}

@media (min-width: 600px) {
  .grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 900px) {
  .grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

/* CARD */
.card {
  background: var(--white);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 6px 16px rgba(0,0,0,0.08);

  opacity: 0;
  transform: translateY(30px);
  transition: all 0.6s ease;
}

.card.show {
  opacity: 1;
  transform: translateY(0);
}

/* Hover only on desktop */
@media (hover: hover) {
  .card:hover {
    transform: translateY(-6px);
    box-shadow: 0 12px 24px rgba(0,0,0,0.15);
  }
}

/* IMAGE */
.card img {
  width: 100%;
  height: 180px;
  object-fit: cover;
}

/* CONTENT */
.card-content {
  padding: 16px;
}

.card h3 {
  font-size: 1.15rem;
  margin-bottom: 8px;
}

.card p {
  font-size: 0.92rem;
  color: var(--muted);
  margin-bottom: 14px;
}

/* BUTTON */
.btn {
  display: block;
  text-align: center;
  padding: 12px;
  background: var(--primary);
  color: white;
  text-decoration: none;
  border-radius: 8px;
  font-weight: 600;
  transition: background 0.2s ease;
}

.btn:active {
  background: #0b5ed7;
}

/* DARK MODE */
body.dark {
  background: #121212;
  color: #eaeaea;
}

body.dark .card {
  background: #1e1e1e;
}

body.dark .btn {
  background: var(--accent);
}

body.dark .btn:active {
  background: #24a89c;
}

body.dark #theme-toggle {
  background: #333;
  color: #fff;
}

/* MOBILE TWEAK */
@media (max-width: 480px) {
  .logo {
    font-size: 2.5rem;
  }

  header p {
    font-size: 1rem;
  }

  header {
    padding: 60px 15px;
  }
}
</style>
</head>

<body>

<header>
  <h1 class="logo">
    e<span class="x">x</span>peria
  </h1>
  <p>events that influence</p>

  <button id="theme-toggle">🌙</button>
</header>

<div class="container">

  <div class="section-title">
    <h2>Featured Events</h2>
    <p>A showcase of major international exhibitions in Singapore</p>
  </div>

  <div class="grid">

    <div class="card">
      <img src="https://i.imgur.com/5j8fztW.jpeg" alt="Singapore Airshow">
      <div class="card-content">
        <h3>Singapore Airshow</h3>
        <p>
          One of Asia’s largest aerospace exhibitions featuring global aviation innovation.
        </p>
        <a href="https://www.singaporeairshow.com/trade" target="_blank" class="btn">Visit Website</a>
      </div>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/Giialab.jpeg" alt="BAAFEx">
      <div class="card-content">
        <h3>BAAFEx</h3>
        <p>
          A premier business aviation event connecting industry leaders across Asia-Pacific.
        </p>
        <a href="https://www.baafex.com/" target="_blank" class="btn">Visit Website</a>
      </div>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/llTr8JE.jpeg" alt="IMDEX Asia">
      <div class="card-content">
        <h3>IMDEX Asia</h3>
        <p>
          A leading maritime defense exhibition showcasing naval technology and innovation.
        </p>
        <a href="https://www.imdexasia.com/" target="_blank" class="btn">Visit Website</a>
      </div>
    </div>
    
    <div class="card">
      <img src="https://i.imgur.com/rUO9gSm.jpeg" alt="Space Summit">
      <div class="card-content">
        <h3>Space Summit</h3>
        <p>
          A Space Summit is a high-level forum where industry leaders, policymakers, and experts convene to discuss developments, strategies, and collaboration in the space sector.
        </p>
        <a href="https://www.singaporespacesummit.com/" target="_blank" class="btn">Visit Website</a>
      </div>
    </div>

  </div>
</div>

<!-- SCRIPTS -->
<script>
const toggle = document.getElementById("theme-toggle");

toggle.addEventListener("click", () => {
  document.body.classList.toggle("dark");
  toggle.textContent =
    document.body.classList.contains("dark") ? "☀️" : "🌙";
});

const cards = document.querySelectorAll(".card");

const observer = new IntersectionObserver(
  (entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add("show");
      }
    });
  },
  { threshold: 0.2 }
);

cards.forEach(card => observer.observe(card));
</script>

</body>
</html>
