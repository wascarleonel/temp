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
        background-color: white;
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
        <button class="button" onclick="https://www.google.com">Section 1</button>
        <button class="button" onclick="showSection(2)">Section 2</button>
        <button class="button" onclick="showSection(3)">Section 3</button>
        <button class="button" onclick="showSection(4)">Section 4</button>
      </div>
    </header>
    <section id="section1" class="active" height = "1920">
      <h2>Section 1</h2>
      <p>This is the first section of my webpage.</p>
    </section>
    <section id="section2">
      <h2>Section 2</h2>
      <p>This is the second section of my webpage.</p>
// ============== TRANSCRIPTION ================

<div>
<div style="display: flex; margin-left: 20px; margin-right: 0px; justify-content; width: 990;">
    <p style = "font-size: 16px;">Interviewer: Ok, basically the idea we have is how to choose personalities from different areas so that they can tell us a little about how it was in 2012, what their main achievements were and also so that we can give a positive message to the country for the arrival of 2013, there is a lot of pessimism for all the things that are coming, but we really believe so, that 2013 is going to be a good year and we want people to know it from you, that is, you, for example, the artistic part, we have here  a businessman, we have the prosecutor, that is, each one from his area gives an optimistic message.</p>
      
      </div>
<p style="margin-left: 20px;">So the first thing is what 2012 meant to you, both personally and generally, how would you define 2012?</p>
    </div>

<div style="height: 4px; width: 28px; background-color: #011F3B;"></div>
<p style = "margin-left: 20px; width: 990; font-size: 16px;">Interviewed: You know about those signs that say ¨construction area¨, for me 2012 was a work process, of creating and creating, I finished my first album, I did my first television segment, on a personal level I also think that Being the second year that I had been in .......... I found myself, I found my people, I found what I like to do and I fell more in love with the country so much so that my desire is to stay and keep working here.</p>
   
<div style="height: 4px; width: 28px; background-color: #011F3B;"></div>
<p style = "margin-left: 20px; width: 990; font-size: 16px;">Interviewer: Ok, that album that you finished, what is the name?</p>
    
<div style="height: 4px; width: 28px; background-color: #011F3B;"></div>
<p style = "margin-left: 20px; width: 990; font-size: 16px;">Interviewed: It's called ¨Me encontre conmigo¨, it's a production that was made with -------- as producer and I also recorded a couple of other things and so we're starting the promotion process in 2013, but also a couple more projects</p>

// ---------------------------------------------

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
