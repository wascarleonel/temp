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
      #header {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px;
        background-color: #fff;
      }
      #header h1 {
        font-size: 24px;
        margin: 0;
      }
      #profile-pic {
        width: 200px;
        height: 200px;
        border-radius: 50%;
        margin-right: 10px;
      }
      #name {
        font-size: 18px;
        font-weight: bold;
        margin: 0;
      }
      #profession {
        font-size: 14px;
        margin: 0;
      }
    </style>
  </head>
  <body>
    <header id="header">
      <div>
        <img src="https://img.freepik.com/free-photo/portrait-young-smiling-man_171337-11976.jpg" alt="Profile Picture" id="profile-pic">
        <div>
          <h1 id="name">Wascar Leonel</h1>
          <p id="profession">Copywriter | Editor | Educator</p>
        </div>
      </div>
      <div>
        <button class="button" onclick="showSection(1)">Section 1</button>
        <button class="button" onclick="showSection(2)">Section 2</button>
        <button class="button" onclick="showSection(3)">Section 3</button>
        <button class="button" onclick="showSection(4)">Section 4</button>
      </div>
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
        // scroll to selected section
        sectionToShow.scrollIntoView({behavior: 'smooth'});
      }
    </script>
  </body>
</html>
