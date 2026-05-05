---
layout: page
permalink: /teaching/
title: Teaching
description:
nav: false
nav_order: 3
dropdown: false
children:
  - title: Teaching List
    permalink: /teaching/
  - title: Quantum Learning Theory for Bosonic and Fermionic Systems (Winter 2026)
    permalink: /bosonic-learning-theory-winter26/
  - title: Quantum Complexity Theory Reading Group (Fall 2025)
    permalink: /quantum-complexity-reading-group-fall25/
  - title: Quantum Learning and Complexity Theory (Summer 2025)
    permalink: /qlct/

---
<html>
    <head>
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Roboto+Serif:ital,opsz,wght@0,8..144,100..900;1,8..144,100..900&display=swap" rel="stylesheet">
        <style>
            body {
                font-family: "Roboto Serif", serif;
                font-optical-sizing: auto;
                font-weight: 200;
                font-size: 0.96rem;
            }
            strong, b {
            font-weight: 500;
            }
            h1 { font-weight: 350; }
            h2 { font-weight: 350; }
            h3 { font-weight: 350; }
            h4, h5, h6 { font-weight: 350; }
        </style>
    </head>
</html>


<div style="font-size:15px; line-height:1.65;">

<!-- Instructor -->
<h5 onclick="toggleInstructor()" style="margin-top:1.8em; margin-bottom:0.6em; color:#1f4e79; border-bottom:2px solid #d9e6f2; padding-bottom:0.25em; cursor:pointer; display:flex; justify-content:space-between;">
  <span>Instructor</span>
  <span id="instructor-icon">+</span>
</h5>

<div id="instructor-content" style="max-height:0; overflow:hidden; opacity:0; transition:max-height 0.45s ease, opacity 0.3s ease;">
<ul style="padding-left:1.4em; margin-top:0.6em;">

<li style="margin-bottom:1em;">
<b>Quantum Learning Theory for Bosonic and Fermionic Systems</b> (Undergraduate, Graduate)<br>
Winter 2026, QISCA<br>
<a href="/bosonic-learning-theory-winter26" target="_blank"><b>[Course Website]</b></a>
</li>

<li style="margin-bottom:1em;">
<b>Reading Group: Quantum Complexity Theory</b> (Undergraduate, Graduate)<br>
Fall 2025, QISCA<br>
<a href="/quantum-complexity-reading-group-fall25" target="_blank"><b>[Course Website]</b></a>
</li>

<li style="margin-bottom:1em;">
<b>AAA559: College of Informatics Internship 2</b> (Graduate)<br>
Fall 2025, Korea University
</li>

<li style="margin-bottom:1em;">
<b>AAA558: College of Informatics Internship 1</b> (Graduate)<br>
Fall 2025, Korea University
</li>

<li style="margin-bottom:1em;">
<b>Quantum Learning and Complexity Theory</b> (Undergraduate, Graduate)<br>
Summer 2025, QISCA<br>
<a href="/qlct" target="_blank"><b>[Course Website]</b></a>
</li>

<li style="margin-bottom:0.6em;">
<b>SW4343: Software Field Placement 1</b> (Undergraduate)<br>
Fall 2024, Korea Aerospace University and Korea Quantum Industry Center
</li>

</ul>
</div>

<hr style="border:none; border-top:1px solid #FFFFFF; margin:1em 0;">

<!-- TA -->
<h5 onclick="toggleTA()" style="margin-top:0; margin-bottom:0.6em; color:#1f4e79; border-bottom:2px solid #d9e6f2; padding-bottom:0.25em; cursor:pointer; display:flex; justify-content:space-between;">
  <span>Teaching Assistant</span>
  <span id="ta-icon">+</span>
</h5>

<div id="ta-content" style="max-height:0; overflow:hidden; opacity:0; transition:max-height 0.45s ease, opacity 0.3s ease;">
<ul style="padding-left:1.4em; margin-top:0.6em;">

<li style="margin-bottom:1em;">
<b>YCS1009: Change the World through Programming</b> (Undergraduate)<br>
Fall 2022, Yonsei University
</li>

<li style="margin-bottom:1em;">
<b>YCS1002: Software Programming</b> (Undergraduate)<br>
Fall 2022, Yonsei University
</li>

<li style="margin-bottom:0.6em;">
<b>EEE1108: Engineering Information Processing</b> (Undergraduate)<br>
Fall 2021, Yonsei University
</li>

</ul>
</div>

<hr style="border:none; border-top:1px solid #FFFFFF; margin:1em 0;">

<!-- Tutor -->
<h5 onclick="toggleTutor()" style="margin-top:0; margin-bottom:0.6em; color:#1f4e79; border-bottom:2px solid #d9e6f2; padding-bottom:0.25em; cursor:pointer; display:flex; justify-content:space-between;">
  <span>Course Tutor</span>
  <span id="tutor-icon">+</span>
</h5>

<div id="tutor-content" style="max-height:0; overflow:hidden; opacity:0; transition:max-height 0.45s ease, opacity 0.3s ease;">
<ul style="padding-left:1.4em; margin-top:0.6em;">

<li style="margin-bottom:1em;">
<b>MAT2016: Engineering Mathematics 3 (Differential Equations and Linear Algebra)</b> (Undergraduate)<br>
Spring 2022, Yonsei University<br>
<span style="color:navy;"><b>Best Tutor Award</b></span>
</li>

<li style="margin-bottom:0.6em;">
<b>MAT1012: Engineering Mathematics 2 (Multivariable and Vector Calculus)</b> (Undergraduate)<br>
Fall 2021, Yonsei University<br>
<span style="color:navy;"><b>Best Tutor Award</b></span>
</li>

</ul>
</div>

</div>

<script>
function toggleSection(contentId, iconId) {
  const content = document.getElementById(contentId);
  const icon = document.getElementById(iconId);

  if (content.style.maxHeight && content.style.maxHeight !== "0px") {
    content.style.maxHeight = "0";
    content.style.opacity = "0";
    icon.textContent = "+";
  } else {
    content.style.maxHeight = content.scrollHeight + "px";
    content.style.opacity = "1";
    icon.textContent = "−";
  }
}

function toggleInstructor() {
  toggleSection("instructor-content", "instructor-icon");
}

function toggleTA() {
  toggleSection("ta-content", "ta-icon");
}

function toggleTutor() {
  toggleSection("tutor-content", "tutor-icon");
}
</script>