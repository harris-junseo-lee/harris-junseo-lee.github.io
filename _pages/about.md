---
layout: about
title: About
permalink: /
subtitle:

profile:
  align: right
  image: board.jpg
  image_circular: true
  more_info: |
    <div style="
      margin-top: -7px;
      margin-bottom: 6px;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 4px;
    ">
      <img src="/assets/img/HQI.png"
           style="height: 52px; width: auto; object-fit: contain;">
      <img src="/assets/img/GSAS.png"
           style="height: 43px; width: auto; object-fit: contain;">
    </div>

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
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
            font-weight: 550;
            }
            h1 { font-weight: 350; }
            h2 { font-weight: 350; }
            h3 { font-weight: 350; }
            h4, h5, h6 { font-weight: 350; }
        </style>
    </head>
</html>



<b>Update:</b> 
I will be joining 
<a href="https://www.harvard.edu/" style="font-weight:400; text-decoration:none;">Harvard University</a> 
in Fall 2026 as a PhD student in Quantum Science and Engineering, 
where I am fortunate to be co-advised by 
<a href="https://anuraganshu.seas.harvard.edu/" style="font-weight:400; text-decoration:none;">Anurag Anshu</a>, 
<a href="https://sitanchen.com/" style="font-weight:400; text-decoration:none;">Sitan Chen</a>, and 
<a href="https://www.physics.harvard.edu/people/facpages/cotler" style="font-weight:400; text-decoration:none;">Jordan Cotler</a>. 
I will also be affiliated with the 
<a href="https://quantum.harvard.edu/" style="font-weight:400; text-decoration:none;">Harvard Quantum Initiative</a> 
and the 
<a href="https://toc.seas.harvard.edu/" style="font-weight:400; text-decoration:none;">Theory of Computation Group</a>.

I am currently a Research Fellow at the 
<a href="https://ict.snu.ac.kr/" style="font-weight:400; text-decoration:none;">
Institute of Computer Technology, Seoul National University (SNU)</a>, 
supported by 
<a href="https://www.nrf.re.kr/eng/index" style="font-weight:400; text-decoration:none;">NRF</a>, 
<a href="https://www.iitp.kr/eng/index.do" style="font-weight:400; text-decoration:none;">IITP</a>, 
and 
<a href="https://www.etri.re.kr/eng/main/main.etri" style="font-weight:400; text-decoration:none;">ETRI</a>.

My research focuses on the mathematical and theoretical computer science aspects of quantum systems, particularly quantum learning theory and quantum complexity theory, as well as their connections to quantum many-body physics.

Previously, I completed my mandatory military service in South Korea as a Technical Research Personnel, during which I was a Research Affiliate at the 
<a href="https://rim.math.snu.ac.kr/" style="font-weight:400; text-decoration:none;">
Research Institute of Mathematics, SNU</a>. 
I received my B.S. in Electrical and Electronic Engineering from 
<a href="https://www.yonsei.ac.kr/en_sc/index.do" style="font-weight:400; text-decoration:none;">
Yonsei University</a>, where I was supported by the 
<a href="https://www.hyundai-cmkfoundation.org/en/main" style="font-weight:400; text-decoration:none;">
Hyundai Motor CMK Science and Technology Scholarship</a>.

📄 <a href="/assets/pdf/CV.pdf"><b>Curriculum Vitae</b></a> (Last updated: April 19, 2026)<br>
🔗 <a href="http://www.linkedin.com/in/harris-quantum" style="font-weight:400; text-decoration:none;">LinkedIn</a>, 
<a href="https://scholar.google.co.kr/citations?user=mal5ZI8AAAAJ&hl=ko" style="font-weight:400; text-decoration:none;">Google Scholar</a>, 
<a href="https://x.com/harris_junseo" style="font-weight:400; text-decoration:none;">X (formerly Twitter)</a><br>
📨 <span style="font-family: monospace;">junseolee [at] fas.harvard.edu</span><br>
<!-- 📨 <span style="font-family: monospace;">junseolee [at] snu.ac.kr </span>(SNU-related)<br> -->
<!-- 💼 <span style="font-family: monospace;">SNU Bldg #138 Institute of Computer Technology, Room 203</span> -->


<h5
  onclick="togglePapers()"
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
  <span>Selected Papers</span>
  <span id="papers-icon" style="font-size: 1.2em; transition: transform 0.2s ease;">+</span>
</h5>

<div
  id="papers-content"
  style="
    max-height: 0;
    overflow: hidden;
    opacity: 0;
    transition: max-height 0.45s ease, opacity 0.3s ease;
  "
>
  <div style="padding-top: 0.4em;">
    A full publication list is available <a href="/publications/"><b>here</b></a>.

    <ul style="padding-left: 1.2em; margin-top: 0.8em;">
      <li style="margin-bottom: 1em;">
        <b>Certifying and learning local quantum Hamiltonians</b><br>
        <span style="letter-spacing:-0.002em;">
          with Andreas Bluhm, Matthias C. Caro, Francisco Escudero Gutiérrez, Aadil Oufkir, Cambyse Rouzé, Myeongjin Shin
        </span><br>
        <i>Contributed talk at TQC</i> (2026).<br>
        <a href="https://arxiv.org/abs/2603.29809"><b>[PDF]</b></a>,
        <a href="https://tqc-conference.org/2026/"><b>[TQC 2026]</b></a>
      </li>

      <li style="margin-bottom: 1em;">
        <b>Efficient learning of bosonic Gaussian unitaries</b><br>
        with Marco Fanizza, Vishnu Iyer, Antonio Anna Mele, Francesco Anna Mele<br>
        <i>Contributed talk at QIP</i> (2026).<br>
        <a href="https://arxiv.org/pdf/2510.05531v1"><b>[PDF]</b></a>,
        <a href="/assets/pdf/CV_unitary_tomography.pdf" target="_blank"><b>[Slides]</b></a>,
        <a href="https://qip2026.lu.lv/programme/accepted-papers/"><b>[QIP 2026]</b></a>
      </li>

      <li style="margin-bottom: 0.5em;">
        <b>Resource-efficient algorithm for estimating the trace of quantum state powers</b><br>
        with Myeongjin Shin, Seungwoo Lee, Kabgyun Jeong<br>
        <i>Quantum</i> (2025).<br>
        <a href="https://arxiv.org/pdf/2408.00314"><b>[PDF]</b></a>,
        <a href="https://quantum-journal.org/papers/q-2025-08-27-1832/"><b>[Journal]</b></a>,
        <a href="/assets/pdf/rank_qst.pdf" target="_blank"><b>[Slide]</b></a>,
        <a href="/assets/pdf/rank_poster.pdf" target="_blank"><b>[Poster]</b></a>,
        <a href="https://ptreview.sublinear.info/2025/09/news-for-august-2025/"><b>[Property Testing Review]</b></a>
      </li>
    </ul>
  </div>
</div>

<script>
  function togglePapers() {
    const content = document.getElementById("papers-content");
    const icon = document.getElementById("papers-icon");

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


<h5
  onclick="toggleTeaching()"
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
  <span>Selected Teaching</span>
  <span id="teaching-icon" style="font-size: 1.2em; transition: transform 0.2s ease;">+</span>
</h5>

<div
  id="teaching-content"
  style="
    max-height: 0;
    overflow: hidden;
    opacity: 0;
    transition: max-height 0.45s ease, opacity 0.3s ease;
  "
>
  <div style="padding-top: 0.4em;">
    A full list of teaching materials is available
    <a href="/teaching/"><b>here</b></a>.

    <ul style="margin-top: 0.8em;">
      <li>
        <a href="/bosonic-learning-theory-winter26/" target="_blank">
          Quantum Learning Theory for Bosonic and Fermionic Systems (Winter 2026)
        </a>
      </li>
      <li>
        <a href="/quantum-complexity-reading-group-fall25/" target="_blank">
          Quantum Complexity Theory Reading Group (Fall 2025)
        </a>
      </li>
      <li>
        <a href="/qlct/" target="_blank">
          Quantum Learning and Complexity Theory (Summer 2025)
        </a>
      </li>
    </ul>
  </div>
</div>

<script>
  function toggleTeaching() {
    const content = document.getElementById("teaching-content");
    const icon = document.getElementById("teaching-icon");

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



<h5
  onclick="toggleMentoring()"
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
  <span>Mentoring</span>
  <span id="mentoring-icon" style="font-size: 1.2em;">+</span>
</h5>

<div
  id="mentoring-content"
  style="
    max-height: 0;
    overflow: hidden;
    opacity: 0;
    transition: max-height 0.45s ease, opacity 0.3s ease;
  "
>
  <div style="padding-top: 0.4em;">

    <p>
      During my time as a Research Fellow and Research Affiliate at Seoul National University, I mentored undergraduate students in research. It was a great privilege and a deeply rewarding experience to work with such talented students, and I learned a great deal from our collaborations as well.
    </p>

    <ul style="margin-top: 0.8em;">

      <li>
        <a href="https://myeongjinshin.github.io/" style="font-weight:400; text-decoration:none;">
          Myeongjin Shin
        </a>
        (Spring 2023–present, co-supervised with 
        <a href="https://sites.google.com/site/kabgyunspage/" style="font-weight:400; text-decoration:none;">
          Kabgyun Jeong</a>)
      </li>

      <li>
        <a href="https://scholar.google.com/citations?user=ok3lJjEAAAAJ&hl=ko" style="font-weight:400; text-decoration:none;">
          Mingyu Lee
        </a>
        (Spring 2024–present, co-supervised with 
        <a href="https://www.cs.ox.ac.uk/people/sathyawageeswar.subramanian/" style="font-weight:400; text-decoration:none;">
          Sathya Subramanian</a>)
      </li>

      <li>
        <a href="https://scholar.google.com/citations?user=OTXe1oAAAAAJ&hl=ko" style="font-weight:400; text-decoration:none;">
          Donghwa Ji
        </a>
        (Spring 2025–present, co-supervised with 
        <a href="https://sites.google.com/site/kabgyunspage/" style="font-weight:400; text-decoration:none;">
          Kabgyun Jeong</a>)
      </li>

      <li>
        <a href="https://www.linkedin.com/in/kartik-anand-6abb94192/" style="font-weight:400; text-decoration:none;">
          Kartik Anand
        </a>
        (Summer 2025)
      </li>

    </ul>

  </div>
  I would be happy to mentor research projects if there is a suitable fit. Feel free to reach out by email if you are interested!
</div>

<script>
  function toggleMentoring() {
    const content = document.getElementById("mentoring-content");
    const icon = document.getElementById("mentoring-icon");

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



<h5
  onclick="toggleMisc()"
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
  <span>Miscellaneous</span>
  <span id="misc-icon" style="font-size: 1.2em;">+</span>
</h5>

<div
  id="misc-content"
  style="
    max-height: 0;
    overflow: hidden;
    opacity: 0;
    transition: max-height 0.45s ease, opacity 0.3s ease;
  "
>
  <div style="padding-top: 0.4em;">
    <p>
      I enjoy playing table tennis and piano, and I also like a wide variety of puzzle games.
    </p>

    <p>
        I am also particularly interested in the <a href="https://www.genealogy.math.ndsu.nodak.edu/" style="font-weight:400; text-decoration:none;"><b>Mathematics Genealogy Project</b></a>. By tracing the academic lineages of my advisors, I came across several fascinating connections. In particular, it was striking to encounter figures such as 
        <a href="https://en.wikipedia.org/wiki/Leonhard_Euler" style="font-weight:400; text-decoration:none;"><b>Leonhard Euler</b></a> (from Anurag Anshu), 
        <a href="https://en.wikipedia.org/wiki/Carl_Gustav_Jacob_Jacobi" style="font-weight:400; text-decoration:none;"><b>Carl Gustav Jacob Jacobi</b></a> (from Sitan Chen), and 
        <a href="https://en.wikipedia.org/wiki/Paul_Dirac" style="font-weight:400; text-decoration:none;"><b>Paul Dirac</b></a> (from Jordan Cotler) 
        along these lineages!
    </p>

    <p style="margin-top: 0.8em;">
      <a
        href="javascript:void(0);"
        onclick="toggleLineageList(event)"
        style="font-weight:400; text-decoration:none;"
      >
        <span id="lineage-toggle-text">See full list</span>
      </a>
    </p>

    <div
      id="lineage-list"
      style="
        display: none;
        margin-top: 0.8em;
        line-height: 1.7;
      "
    >
      <p>
        Anurag Anshu → Rahul Jain → Jaikumar Radhakrishnan → Endre Szemerédi → Israel Gelfand → Andrey Kolmogorov → Nikolai Luzin → Dmitri Egorov → Nikolai Bugaev → Joseph Liouville → Siméon Poisson → Joseph-Louis Lagrange → Leonhard Euler → Johann Bernoulli → (...)
      </p>

      <p>
        Sitan Chen → Ankur Moitra → Thomson Leighton → Gary Miller → Manuel Blum → Marvin Minsky → Albert W. Tucker → Solomon Lefschetz → William Edward Story → Carl Neumann → Friedrich Julius Richelot → Carl Gustav Jacob Jacobi → Enno Dirksen → Johann Tobias Mayer → (...)
      </p>

      <p>
        Jordan Cotler → Patrick Hayden → Artur Ekert → David Deutsch → Dennis Sciama → Paul Dirac → Ralph Fowler → Archibald Vivian Hill → Sir Walter Fletcher → John Newport Langley → Michael Foster → Thomas Henry Huxley → Thomas W. Jones → William MacKenzie → (...)
      </p>
    </div>
  </div>
</div>

<script>
  function toggleMisc() {
    const content = document.getElementById("misc-content");
    const icon = document.getElementById("misc-icon");

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

  function toggleLineageList(event) {
    event.stopPropagation();

    const list = document.getElementById("lineage-list");
    const text = document.getElementById("lineage-toggle-text");
    const miscContent = document.getElementById("misc-content");

    if (list.style.display === "none" || list.style.display === "") {
      list.style.display = "block";
      text.textContent = "Hide full list";
    } else {
      list.style.display = "none";
      text.textContent = "See full list";
    }

    setTimeout(() => {
      if (miscContent.style.maxHeight !== "0px") {
        miscContent.style.maxHeight = miscContent.scrollHeight + "px";
      }
    }, 10);
  }
</script>