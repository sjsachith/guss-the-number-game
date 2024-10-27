<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Endemic Plants and Animals of India</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      color: #1b5e20;
      margin: 0;
      padding: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }

    .container {
      max-width: 700px;
      width: 90%;
      margin: auto;
      padding: 20px;
      border-radius: 8px;
      color: white;
      box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
      position: relative;
      display: none;
    }

    .container.active {
      display: block;
    }

    h1, h2 {
      text-align: center;
    }

    .points {
      list-style: none;
      padding: 0;
      margin: 10px 0;
    }

    .points li {
      margin-bottom: 10px;
    }

    .btn-container {
      text-align: center;
    }

    .btn {
      background-color: #4caf50;
      color: white;
      padding: 10px 20px;
      text-decoration: none;
      border-radius: 5px;
      margin: 5px;
      cursor: pointer;
      display: inline-block;
    }

    .btn:hover {
      background-color: #388e3c;
    }

    /* Background Colors for Each Slide */
    #slide1 { background-color: #388e3c; }
    #slide2 { background-color: #00796b; }
    #slide3 { background-color: #558b2f; }
    #slide4 { background-color: #5d4037; }
    #slide5 { background-color: #2e7d32; }
  </style>
</head>
<body>

<div id="slide1" class="container active">
  <h1>Endemic Plants and Animals of India</h1>
  <p>Explore the unique world of endemic plants and animals that are found exclusively in India’s ecosystems.</p>
  <div class="btn-container">
    <button class="btn" onclick="nextSlide(2)">Next</button>
  </div>
</div>

<div id="slide2" class="container">
  <h2>What Are Endemic Species?</h2>
  <ul class="points">
    <li>Endemic species are plants or animals found only in a particular geographical region.</li>
    <li>They develop special adaptations to survive in specific climates and ecosystems.</li>
    <li>In India, many unique species are endemic due to diverse habitats like the Western Ghats, Himalayas, and more.</li>
    <li>Examples include the Indian Gaur, the Purple Frog, and numerous rare plant species.</li>
  </ul>
  <div class="btn-container">
    <button class="btn" onclick="prevSlide(1)">Back</button>
    <button class="btn" onclick="nextSlide(3)">Next</button>
  </div>
</div>

<div id="slide3" class="container">
  <h2>Example of an Endemic Plant: Neelakurinji</h2>
  <ul class="points">
    <li>The Neelakurinji (<em>Strobilanthes kunthiana</em>) blooms only once every 12 years in the Western Ghats.</li>
    <li>This unique flowering plant is known for covering hillsides with a carpet of blue-purple flowers when it blooms.</li>
    <li>Its rare bloom attracts numerous tourists and supports local biodiversity.</li>
    <li>Neelakurinji is a symbol of India’s rich plant diversity and is protected in places like the Eravikulam National Park.</li>
  </ul>
  <div class="btn-container">
    <button class="btn" onclick="prevSlide(2)">Back</button>
    <button class="btn" onclick="nextSlide(4)">Next</button>
  </div>
</div>

<div id="slide4" class="container">
  <h2>Example of an Endemic Animal: Nilgiri Tahr</h2>
  <ul class="points">
    <li>The Nilgiri Tahr (<em>Nilgiritragus hylocrius</em>) is a mountain goat native to the Nilgiri Hills and Western Ghats.</li>
    <li>This endangered species has adapted to steep, rocky terrain, making it agile and resilient.</li>
    <li>It plays a significant role in the ecosystem, helping to maintain the balance of local flora through grazing.</li>
    <li>Conservation efforts are ongoing in sanctuaries to protect the Nilgiri Tahr from habitat loss and poaching.</li>
  </ul>
  <div class="btn-container">
    <button class="btn" onclick="prevSlide(3)">Back</button>
    <button class="btn" onclick="nextSlide(5)">Next</button>
  </div>
</div>

<div id="slide5" class="container">
  <h2>Why Protect Endemic Species?</h2>
  <ul class="points">
    <li>Endemic species are essential for ecological balance and biodiversity in India’s varied ecosystems.</li>
    <li>Their extinction would disrupt food chains and impact the survival of other species.</li>
    <li>Protecting endemic species also safeguards natural heritage, ensuring these unique organisms remain for future generations.</li>
    <li>Conservation involves habitat preservation, protection against poaching, and educating communities on sustainable practices.</li>
  </ul>
  <div class="btn-container">
    <button class="btn" onclick="prevSlide(4)">Back</button>
    <button class="btn" onclick="nextSlide(1)">Start Over</button>
  </div>
</div>

<script>
  function nextSlide(slideNumber) {
    document.querySelectorAll('.container').forEach(slide => slide.classList.remove('active'));
    document.getElementById('slide' + slideNumber).classList.add('active');
  }

  function prevSlide(slideNumber) {
    document.querySelectorAll('.container').forEach(slide => slide.classList.remove('active'));
    document.getElementById('slide' + slideNumber).classList.add('active');
  }
</script>

</body>
</html>
