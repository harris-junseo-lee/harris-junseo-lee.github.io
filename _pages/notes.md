---
layout: page
permalink: /notes/
title: Notes
description: I occasionally write on a range of topics, and I hope you enjoy reading!
nav: false
nav_order: 4
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

<h5
  onclick="togglePhdPost()"
  style="
    margin-top: 1.8em;
    margin-bottom: 0.6em;
    color: #1f4e79;
    border-bottom: 2px solid #d9e6f2;
    padding-bottom: 0.25em;
    cursor: pointer;
    user-select: none;
    display: flex;
    align-items: center;
    justify-content: space-between;
  "
>
  <span>My PhD Application Journey</span>
  <span id="phd-post-icon" style="font-size: 1.2em;">+</span>
</h5>

<div
  id="phd-post-content"
  style="
    max-height: 0;
    overflow: hidden;
    opacity: 0;
    transition: max-height 0.45s ease, opacity 0.3s ease;
  "
>
  <div style="padding-top: 0.4em;">
    <p>
      I applied to PhD programs for the Fall 2026 admission cycle. The experience of applying to PhD programs seems to vary widely across individuals and fields. In my case, I applied within theoretical quantum computing, broadly across programs in theoretical computer science, theoretical physics, and quantum science and engineering. While the program titles differed, the research directions I aimed to pursue were largely the same.
    </p>

    <p>
      I applied without holding a master’s degree, which is somewhat less common among Korean students, many of whom pursue a master’s before applying abroad. Instead, after completing my undergraduate studies, I fulfilled my mandatory military service in South Korea as a Technical Research Personnel before applying to PhD programs.
    </p>

    <p>
      Recently, I have received a number of inquiries from students seeking advice on the PhD application process, and I have been doing my best to provide helpful responses. For those who may be interested in my experience, I will also be sharing some thoughts at a study abroad information session at Yonsei University on May 16.
    </p>

    <p>
      I am very grateful to have been admitted to the PhD programs in Quantum Science and Engineering at Harvard and in Physics at MIT. After careful consideration, I have decided to join Harvard and therefore declined the offer from MIT. Following this decision, I withdrew my applications to Oxford and UC Berkeley—where I had already completed interviews—prior to receiving final decisions.
    </p>

    <p>
      I am also deeply grateful for the many people who supported me throughout the application process. I received invaluable advice and encouragement along the way, and I would like to sincerely thank Jaeyeon, Chanwoo, Gunhee, Sascha, Antonio, Francesco, Vishnu, Seyoon, Luke, Dominik, and Quynh. I hope to pay this kindness forward and offer the same support to others in the future.
    </p>

    <p>
      I look forward to continuing to connect with the quantum information community in the Boston/Cambridge area, and I feel very fortunate to be able to pursue quantum computing in such an exceptional environment.
    </p>
  </div>
</div>

<script>
  function togglePhdPost() {
    const content = document.getElementById("phd-post-content");
    const icon = document.getElementById("phd-post-icon");

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
</script>