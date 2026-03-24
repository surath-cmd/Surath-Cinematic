<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Surath Mohideen | Portfolio</title>

  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600;800&display=swap" rel="stylesheet">

  <style>
    body { margin:0; font-family:'Montserrat',sans-serif; background:#000; color:#fff; overflow-x:hidden; }

    /* HERO SHOWREEL */
    .hero {
      position: relative;
      height: 100vh;
      overflow: hidden;
    }

    .hero video {
      position: absolute;
      width: 100%;
      height: 100%;
      object-fit: cover;
      filter: brightness(0.4);
    }

    .hero-content {
      position: relative;
      z-index: 2;
      text-align: center;
      top: 50%;
      transform: translateY(-50%);
    }

    .hero h1 {
      font-size: 56px;
      color: #e50914;
      font-weight: 800;
      letter-spacing: 3px;
    }

    .hero p { color:#ccc; }

    .play-btn {
      margin-top:20px;
      display:inline-block;
      padding:12px 24px;
      border:2px solid #e50914;
      color:#fff;
      cursor:pointer;
      transition:0.3s;
    }

    .play-btn:hover { background:#e50914; }

    .container { max-width:1000px; margin:auto; padding:40px 20px; }

    h2 { color:#e50914; border-left:4px solid #e50914; padding-left:10px; }

    .card {
      background:#141414;
      padding:25px;
      margin:20px 0;
      border-radius:10px;
      opacity:0;
      transform: translateY(40px);
      transition:0.6s ease;
    }

    .card.show { opacity:1; transform: translateY(0); }

    .tag { display:inline-block; background:#1f1f1f; padding:8px 12px; margin:6px; border-radius:6px; }

    footer { text-align:center; padding:30px; border-top:1px solid #222; color:#777; }

  </style>
</head>
<body>

<!-- HERO SHOWREEL -->
<section class="hero">
  <video autoplay muted loop>
    <source src="your-showreel.mp4" type="video/mp4">
  </video>
  <div class="hero-content">
    <h1>SURATH MOHIDEEN</h1>
    <p>Senior Video Editor | Motion Graphics Artist | AI Creator</p>
    <div class="play-btn">View Showreel</div>
  </div>
</section>

<div class="container">

  <section>
    <h2>Profile</h2>
    <div class="card">
      Creative Senior Video Editor and Motion Graphics Artist with experience in broadcast, digital media, and marketing. Currently working with influencers and brands to create high-performance content.
    </div>
  </section>

  <section>
    <h2>Experience</h2>

    <div class="card">
      <strong>Adityaram Group</strong><br>
      Senior Editor – Marketing
    </div>

    <div class="card">
      <strong>Retroluxe</strong><br>
      Chief Editor
    </div>

    <div class="card">
      <strong>BB TV & Bloom Buff</strong><br>
      Senior Editor
    </div>

  </section>

  <section>
    <h2>Skills</h2>
    <div class="card">
      <span class="tag">Premiere Pro</span>
      <span class="tag">After Effects</span>
      <span class="tag">DaVinci Resolve</span>
      <span class="tag">AI Tools</span>
    </div>
  </section>

</div>

<footer>
  © 2026 Surath Mohideen
</footer>

<script>
  const cards = document.querySelectorAll('.card');
  window.addEventListener('scroll', () => {
    cards.forEach(card => {
      const top = card.getBoundingClientRect().top;
      if(top < window.innerHeight - 100) {
        card.classList.add('show');
      }
    });
  });
</script>

</body>
</html>
