# Experiaevents.github.io
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Experia Events Portfolio</title>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: Arial, Helvetica, sans-serif;
    background: #f4f6f8;
    color: #333;
  }

  /* HERO HEADER */
  header {
  position: relative;
  height: 60vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;

  background: #000;
  color: #fff;
  overflow: hidden;

  }

  header::before {
    content: "";
    position: absolute;
    inset: 0;
    background: rgba(0, 0, 0, 0.45);
  }

  header h1 {
    font-size: 3rem;
    z-index: 1;
    animation: fadeIn 1s ease-in-out;
  }

  header p {
    margin-top: 10px;
    font-size: 1.2rem;
    z-index: 1;
    opacity: 0.9;
  }

  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }

  /* CONTAINER */
  .container {
    max-width: 1100px;
    margin: auto;
    padding: 40px 20px;
  }

  /* GRID */
  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 25px;
  }

  /* CARD */
  .card {
    background: #fff;
    border-radius: 14px;
    overflow: hidden;
    box-shadow: 0 6px 18px rgba(0,0,0,0.08);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .card:hover {
    transform: translateY(-8px);
    box-shadow: 0 12px 28px rgba(0,0,0,0.15);
  }

  .card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }

  .card-content {
    padding: 18px;
  }

  .card h3 {
    margin-bottom: 10px;
    font-size: 1.2rem;
  }

  .card p {
    font-size: 0.95rem;
    line-height: 1.5;
    margin-bottom: 15px;
    color: #555;
  }

  /* BUTTON */
  .btn {
    display: inline-block;
    padding: 10px 14px;
    background: #007BFF;
    color: #fff;
    text-decoration: none;
    border-radius: 8px;
    font-weight: bold;
    transition: background 0.3s ease, transform 0.2s ease;
  }

  .btn:hover {
    background: #0056b3;
    transform: scale(1.05);
  }

  /* SECTION TITLE (optional improvement) */
  .section-title {
    text-align: center;
    margin-bottom: 30px;
  }

  .section-title h2 {
    font-size: 1.8rem;
    margin-bottom: 5px;
  }

  .section-title p {
    color: #666;
    font-size: 0.95rem;
  }

  /* RESPONSIVE */
  @media (max-width: 600px) {
    header h1 {
      font-size: 2.2rem;
    }
  }
</style>
</head>

<body>

<header>
  <h1>Experia Events</h1>
  <p>Events that Influence.</p>
</header>

<div class="container">

  <div class="section-title">
    <h2>Featured Events</h2>
    <p>A showcase of major international exhibitions in Singapore</p>
  </div>

  <div class="grid">

    <!-- CARD 1 -->
    <div class="card">
      <img src="https://i.imgur.com/5j8fztW.jpeg" alt="Singapore Airshow">
      <div class="card-content">
        <h3>Singapore Airshow</h3>
        <p>
          One of Asia’s largest aerospace and defense exhibitions, featuring aircraft displays, industry leaders, and global aviation innovation.
        </p>
        <a href="https://www.singaporeairshow.com/trade" target="_blank" class="btn">Visit Website</a>
      </div>
    </div>

    <!-- CARD 2 -->
    <div class="card">
      <img src="https://i.imgur.com/Giialab.jpeg" alt="BAAFEx">
      <div class="card-content">
        <h3>BAAFEx</h3>
        <p>
          A premier business aviation event in Asia-Pacific connecting aviation leaders, operators, and innovators in Singapore.
        </p>
        <a href="https://www.baafex.com/" target="_blank" class="btn">Visit Website</a>
      </div>
    </div>

    <!-- CARD 3 -->
    <div class="card">
      <img src="https://i.imgur.com/llTr8JE.jpeg" alt="IMDEX Asia">
      <div class="card-content">
        <h3>IMDEX Asia</h3>
        <p>
          A leading maritime defense exhibition showcasing naval technology, security systems, and global maritime innovation.
        </p>
        <a href="https://www.imdexasia.com/" target="_blank" class="btn">Visit Website</a>
      </div>
    </div>

  </div>
</div>

</body>
</html>
