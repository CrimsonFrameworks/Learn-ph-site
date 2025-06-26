<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>learn.ph.edu - Learn Anytime, Anywhere</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #fdfdfd;
    }

    header {
      background-color: #b80000;
      color: white;
      padding: 40px 20px;
      text-align: center;
    }

    nav {
      background-color: #990000;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }

    nav a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
    }

    nav a:hover {
      background-color: #800000;
    }

    .search-container {
      margin: 20px auto;
      text-align: center;
    }

    input[type="text"] {
      width: 80%;
      max-width: 400px;
      padding: 10px;
      border: 2px solid #b80000;
      border-radius: 5px;
    }

    section {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
    }

    h2 {
      color: #b80000;
    }

    .material {
      background-color: #fff4f4;
      border-left: 5px solid #b80000;
      padding: 15px 20px;
      margin: 20px 0;
      box-shadow: 0 0 5px rgba(0,0,0,0.1);
    }

    iframe {
      width: 100%;
      max-width: 700px;
      height: 400px;
      border: none;
      margin-top: 15px;
    }

    footer {
      background-color: #222;
      color: white;
      text-align: center;
      padding: 20px 0;
    }
  </style>
  <script>
    function searchContent() {
      const input = document.getElementById("searchInput").value.toLowerCase();
      const materials = document.querySelectorAll(".material");
      materials.forEach(material => {
        const text = material.innerText.toLowerCase();
        material.style.display = text.includes(input) ? "block" : "none";
      });
    }
  </script>
</head>
<body>
  <header>
    <h1>learn.ph.edu</h1>
    <p>Learn Anytime, Anywhere – Free & Accessible Education for Filipinos</p>
  </header>

  <nav>
    <a href="#filipino">Filipino</a>
    <a href="#history">History</a>
    <a href="#math">Math</a>
    <a href="#science">Science</a>
    <a href="#english">English</a>
    <a href="#contact">Contact</a>
  </nav>

  <div class="search-container">
    <input type="text" id="searchInput" onkeyup="searchContent()" placeholder="Search learning materials..." />
  </div>

  <section id="filipino">
    <h2>📚 Filipino</h2>
    <div class="material">
      <h3>Wika at Panitikan</h3>
      <p>Panitikan ng Pilipinas at kasaysayan ng ating wika.</p>
      <iframe src="https://drive.google.com/file/d/1ydL2Jk3Ev4RAjjJvPzYoqLKDN_cKtkfE/preview" allow="autoplay"></iframe>
    </div>
    <div class="material">
      <h3>Pagtukoy ng Pangngalan</h3>
      <p>Pagkilala sa uri at gamit ng pangngalan.</p>
      <iframe src="https://www.youtube.com/embed/Eo2ZsV9U_Y0" allowfullscreen></iframe>
    </div>
  </section>

  <section id="history">
    <h2>📖 Philippine History</h2>
    <div class="material">
      <h3>Panahon ng Kastila</h3>
      <p>Panahon ng mga Espanyol sa Pilipinas.</p>
      <iframe src="https://www.youtube.com/embed/SaUgcmvNP0Q" allowfullscreen></iframe>
    </div>
    <div class="material">
      <h3>Kasaysayan ng Katipunan (PDF)</h3>
      <p>Mga kaganapan bago at habang rebolusyon.</p>
      <iframe src="https://drive.google.com/file/d/1kcnTxWbCqIMQp6rNs0J-ixUt6VZ0Qiea/preview" allow="autoplay"></iframe>
    </div>
  </section>

  <section id="math">
    <h2>🧮 Mathematics</h2>
    <div class="material">
      <h3>Basic Arithmetic PDF</h3>
      <p>Intro to addition, subtraction, multiplication, and division.</p>
      <iframe src="https://drive.google.com/file/d/1EdXbbXpN6Bd4v_OzZ4EMznToRmV6YO_z/preview" allow="autoplay"></iframe>
    </div>
  </section>

  <section id="science">
    <h2>🔬 Science</h2>
    <div class="material">
      <h3>Earth & Life Science</h3>
      <p>Pag-aaral ng kalikasan, mundo, halaman, at hayop.</p>
      <iframe src="https://www.youtube.com/embed/bErljS08F0I" allowfullscreen></iframe>
    </div>
  </section>

  <section id="english">
    <h2>📘 English</h2>
    <div class="material">
      <h3>Parts of Speech</h3>
      <p>Nouns, verbs, adjectives, and how they work together.</p>
      <iframe src="https://www.youtube.com/embed/NJqqL7Zl47Q" allowfullscreen></iframe>
    </div>
  </section>

  <section id="contact">
    <h2>📞 Contact</h2>
    <p>For inquiries or feedback, contact us at: <strong>09679011513</strong></p>
  </section>

  <footer>
    <p>&copy; 2025 learn.ph.edu – All rights reserved.</p>
  </footer>
</body>
</html>
