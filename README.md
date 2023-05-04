<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>My Webpage</title>
    <style>
      body {
        background-color: #011F3B;
      }
      section {
        height: 500px;
        width: 100%;
        display: none;
      }
      section.active {
        display: block;
      }
      .button {
        padding: 10px;
        background-color: white;
        color: #011F3B;
        font-size: 18px;
        font-weight: bold;
        border: none;
        cursor: pointer;
      }
    </style>
  </head>
  <body>
    <header>
      <button class="button" onclick="showSection(1)">Section 1</button>
      <button class="button" onclick="showSection(2)">Section 2</button>
      <button class="button" onclick="showSection(3)">Section 3</button>
      <button class="button" onclick="showSection(4)">Section 4</button>
    </header>
    <section id="section1" class="active">
      <h2>Section 1</h2>
      <p>This is the first section of my webpage.</p>
    </section>
    <section id="section2">
      <h2>Section 2</h2>
      <p>This is the second section of my webpage.</p>
    </section>
    <section id="section3">
      <h2>Section 3</h2>
      <p>This is the third section of my webpage.</p>
    </section>
    <section id="section4">
      <h2>Section 4</h2>
      <p>This is the fourth section of my webpage.</p>
    </section>
    <script>
      function showSection(sectionNum) {
        // hide all sections
        const sections = document.querySelectorAll('section');
        sections.forEach(section => section.classList.remove('active'));
        // show selected section
        const sectionToShow = document.getElementById('section' + sectionNum);
        sectionToShow.classList.add('active');
      }
    </script>
  </body>
</html>
