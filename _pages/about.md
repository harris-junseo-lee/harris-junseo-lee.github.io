---
layout: about
title: About
permalink: /
subtitle: |
    <style>
    .subtitle-logos {
      margin-top: -7px;
      margin-bottom: 6px;
      display: flex;
      flex-direction: row;
      align-items: center;
      gap: 10px;
    }

    /* 모바일 대응 */
    @media (max-width: 600px) {
      .subtitle-logos {
        flex-direction: column;
        align-items: flex-start; /* 왼쪽 정렬 */
        gap: 6px;
      }

      .subtitle-logos img {
        height: 40px; /* 살짝 줄이면 더 자연스러움 */
      }
    }
    </style>

    <div class="subtitle-logos">
      <img src="/assets/img/HQI.png"
          style="height: 52px; width: auto; object-fit: contain;">
      <img src="/assets/img/GSAS.png"
          style="height: 42px; width: auto; object-fit: contain;">
      <img src="/assets/img/IAIFI.png"
          style="height: 43px; width: auto; object-fit: contain;">
    </div>

# profile:
#   align: right
#   image: board.jpg
#   image_circular: true
#   more_info: |
#     <div style="
#       margin-top: -7px;
#       margin-bottom: 6px;
#       display: flex;
#       flex-direction: column;
#       align-items: center;
#       gap: 4px;
#     ">
#       <img src="/assets/img/HQI.png"
#            style="height: 52px; width: auto; object-fit: contain;">
#       <img src="/assets/img/GSAS.png"
#            style="height: 43px; width: auto; object-fit: contain;">
#     </div>

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


<img src="/assets/img/jun.jpg" style="width:110px; border-radius:8px; float:left; margin-right:15px; margin-bottom:10px;">


I am an incoming PhD student in Quantum Science and Engineering at 
<b style="color: #A41034;">Harvard University</b>, where I am fortunate to be advised by Professors
<a href="https://anuraganshu.seas.harvard.edu/" style="text-decoration:none; font-weight:300;">Anurag Anshu</a>,
<a href="https://sitanchen.com/" style="text-decoration:none; font-weight:300;">Sitan Chen</a>, and
<a href="https://www.physics.harvard.edu/people/facpages/cotler" style="text-decoration:none; font-weight:300;">Jordan Cotler</a>.

At Harvard, I am affiliated with the
<a href="https://quantum.harvard.edu/" style="text-decoration:none; font-weight:300;">Harvard Quantum Initiative</a>,
the <a href="https://toc.seas.harvard.edu/" style="text-decoration:none; font-weight:300;">Theory of Computation Group</a>,
and the <a href="https://www.physics.harvard.edu/" style="text-decoration:none; font-weight:300;">Department of Physics</a>.
I am also a Junior Investigator at the
<a href="https://iaifi.org/" style="text-decoration:none; font-weight:300;">NSF AI Institute for Artificial Intelligence and Fundamental Interactions (IAIFI)</a>,
based at <a href="https://www.mit.edu/" style="text-decoration:none; font-weight:300;">MIT</a>.

My research lies at the interface of theoretical computer science and mathematical physics, with the goal of understanding the quantum world through computation and information. I am broadly interested in quantum complexity theory, including the quantum PCP conjecture, area laws, and connections to black holes and quantum field theory. I also study algorithms for learning quantum systems and extracting information from them, as well as problems in quantum many-body physics involving qubits, bosons, fermions, and anyons.

Previously, I conducted research at Seoul National University through the
<a href="https://ict.snu.ac.kr/" style="text-decoration:none; font-weight:300;">Institute of Computer Technology</a>
and the
<a href="https://rim.math.snu.ac.kr/" style="text-decoration:none; font-weight:300;">Research Institute of Mathematics</a>.
I completed my undergraduate studies in electrical and electronic engineering at
<a href="https://www.yonsei.ac.kr/en_sc/index.do" style="text-decoration:none; font-weight:300;">Yonsei University</a>,
fully supported by the
<a href="https://www.hyundai-cmkfoundation.org/en/main" style="text-decoration:none; font-weight:300;">Hyundai Motor CMK Science and Technology Scholarship</a>.


📄 <a href="/assets/pdf/CV.pdf"><b>Curriculum Vitae</b></a> (Last updated: May 23, 2026)<br>
🔗 <a href="http://www.linkedin.com/in/harris-quantum" style="text-decoration:none;">LinkedIn</a> | 
<a href="https://scholar.google.co.kr/citations?user=mal5ZI8AAAAJ&hl=ko" style="text-decoration:none;">Google Scholar</a> | <a href="https://arxiv.org/a/lee_j_24.html" style="text-decoration:none;">arXiv</a> | <a href="https://x.com/harris_junseo" style="text-decoration:none;">X (formerly Twitter)</a><br>
📨 <span style="font-family: monospace;">junseolee at fas.harvard.edu</span><br>



<h5
  onclick="toggleNews()"
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
  <span>News</span>
  <span id="news-icon" style="font-size: 1.2em;">+</span>
</h5>

<div
  id="news-content"
  style="
    max-height: 0;
    overflow: hidden;
    opacity: 0;
    transition: max-height 0.45s ease, opacity 0.3s ease;
  "
>
  <div style="padding-top: 0.4em;">

    <ul style="margin-top: 0.1em;">

      <li>
        <b>May 2026:</b> I joined the <a href="https://iaifi.org/" style="text-decoration:none;">NSF AI Institute for Artificial Intelligence and Fundamental Interactions (IAIFI)</a> as a Junior Investigator.
      </li>
      
      <li>
        <b>Apr. 2026:</b> I gave an <a href="https://www.linkedin.com/posts/harris-quantum_quantumcomputing-ugcPost-7451973783667785728-mJEH?utm_source=share&utm_medium=member_desktop&rcm=ACoAACWtYG8Byci-8uftMxr4hHdXV7ORmM8_trA" style="text-decoration:none;">invited career talk</a> for students at Shinil High School.
      </li>

      <li>
        <b>Apr. 2026:</b> Our paper on <a href="https://arxiv.org/abs/2603.29809" style="text-decoration:none;">Hamiltonian certification</a> was selected as a contributed talk at TQC 2026.
      </li>

      <li>
        <b>Apr. 2026:</b> I joined the Institute of Computer Technology at Seoul National University as a Research Associate, where I will be working until August 2026 before joining Harvard.
      </li>

      <li>
        <b>Mar. 2026:</b> I visited Harvard for the QSE Open House and continued my visit with support from Anurag Anshu.
      </li>

      <li>
        <b>Mar. 2026:</b> I completed my mandatory military service!
      </li>

      <li>
        <b>Feb. 2026:</b> I was delighted to be admitted to the doctoral programs in Quantum Science and Engineering at Harvard, Physics at MIT, and Computer Science at Oxford. I have accepted the offer from Harvard and am excited for the journey ahead!
      </li>

    </ul>

  </div>
</div>

<script>
  function toggleNews() {
    const content = document.getElementById("news-content");
    const icon = document.getElementById("news-icon");

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

    <ul style="margin-top: 0.8em;">
      <li style="margin-bottom: 1em;">
        <b>Certifying and learning local quantum Hamiltonians</b><br>
        (<i>with</i> Andreas Bluhm, Matthias C. Caro, Francisco Escudero Gutiérrez, Aadil Oufkir, Cambyse Rouzé, Myeongjin Shin)<br>
        <a href="https://tqc-conference.org/2026/"><b>Contributed Talk at the 21st Conference on Theory of Quantum Computation, Communication and Cryptography (TQC 2026)</b></a><br>
      </li>

      <li style="margin-bottom: 1em;">
        <b>Efficient learning of bosonic Gaussian unitaries</b><br>
        (<i>with</i> Marco Fanizza, Vishnu Iyer, Antonio Anna Mele, Francesco Anna Mele)<br>
        <a href="https://qip2026.lu.lv/programme/accepted-papers/"><b>Contributed Talk at the 29th Annual Conference on Quantum Information Processing (QIP 2026)</b></a><br>
      </li>

      <li style="margin-bottom: 0.5em;">
        <b>Resource-efficient algorithm for estimating the trace of quantum state powers</b><br>
        (<i>with</i> Myeongjin Shin, Seungwoo Lee, Kabgyun Jeong)<br>
        <a href="https://quantum-journal.org/papers/q-2025-08-27-1832/"><b>Quantum 9, 1832 (2025)</b></a><br>
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
      I mentored undergraduate students in research, which I found both deeply rewarding and intellectually enriching. I had the privilege of working with outstanding students and learned a great deal from our collaborations. The students I have worked with are listed below:
    </p>

    <h6 style="margin-bottom: 0.4em;"><b>Current Mentees:</b></h6>
    <ul style="margin-top: 0.4em;">

      <li>
        <a href="https://www.linkedin.com/in/hugo-mackay-628926247/" style="text-decoration:none;"><b>Hugo Mackay</b></a> (Harvard College, 2026–)
        <ul>
          <li>
            <a href="https://uraf.harvard.edu/herchel-smith-summer-program" style="text-decoration:none;">
              Herchel Smith Undergraduate Science Research Program
            </a>
            (2026, in collaboration with Prof.
            <a href="https://anuraganshu.seas.harvard.edu/" style="text-decoration:none;">Anurag Anshu</a>)
          </li>
        </ul>
      </li>

      <!-- <li>
        <a href="https://arulandu.com/" style="text-decoration:none;"><b>Alvan Arulandu</b></a> (Harvard College, 2026–)
        <ul>
          <li>
            <a href="https://quantum.harvard.edu/harvard-quantum-initiative-undergraduate-research-fellowship" style="text-decoration:none;">
              Harvard Quantum Initiative Summer Undergraduate Research Fellowship
            </a> and
            <a href="https://uraf.harvard.edu/hcrp" style="text-decoration:none;">
              Harvard College Research Program
            </a>
            (2026)
          </li>
        </ul>
      </li> -->

      <li>
        <a href="https://arulrhikm.github.io/" style="text-decoration:none;"><b>Arul Rhik Mazumder</b></a>
        (Carnegie Mellon University, 2026–)
      </li>

      <li>
        <a href="https://harris-junseo-lee.github.io/" style="text-decoration:none;"><b>Jaemin Park</b></a>
        (SNU, 2026–)
      </li>

      <li>
        <a href="https://scholar.google.com/citations?user=OTXe1oAAAAAJ&hl=ko" style="text-decoration:none;"><b>Donghwa Ji</b></a>
        (SNU, 2025–, in collaboration with Dr. <a href="https://www.preskill.caltech.edu/" style="text-decoration:none;">Kabgyun Jeong</a>)
      </li>

      <li>
        <a href="https://scholar.google.com/citations?user=ok3lJjEAAAAJ&hl=ko" style="text-decoration:none;"><b>Mingyu Lee</b></a>
        (SNU, 2024–)
        <ul>
          <li>
            Internship at the University of Oxford
            (2026, in collaboration with Dr. 
            <a href="https://www.cs.ox.ac.uk/people/sathyawageeswar.subramanian/" style="text-decoration:none;">Sathyawageeswar Subramanian</a>)
          </li>
        </ul>
      </li>

      <li>
        <a href="https://myeongjinshin.github.io/" style="text-decoration:none;"><b>Myeongjin Shin</b></a>
        (KAIST, 2023–)
        <ul>
          <li>
            <a href="https://sfp.caltech.edu/undergraduate-research/programs/surf" style="text-decoration:none;">
              SURF at Caltech
            </a>
            (2026, in collaboration with Profs.
            <a href="https://sites.math.duke.edu/~yt222/" style="text-decoration:none;">Yu Tong</a> and <a href="https://www.preskill.caltech.edu/" style="text-decoration:none;">John Preskill</a>)
          </li>
        </ul>
      </li>

    </ul>

    <h6 style="margin-top: 1.2em; margin-bottom: 0.4em;"><b>Former Mentees:</b></h6>
    <ul style="margin-top: 0.4em;">

      <li>
        <a href="https://k-styles.github.io/" style="text-decoration:none;"><b>Kartik Anand</b></a>
        (IIT Goa, 2025; now a master's student at Hamburg University of Technology)
      </li>

    </ul>

  </div>
  <p>
    I am happy to discuss potential research opportunities with undergraduate students, including summer projects. In some cases, projects may also develop into collaborations involving other researchers. Please feel free to reach out by email if you are interested!
  </p>
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
  <span>Teaching</span>
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
  <style>
    .teaching-section-title {
      margin-top: 0.7em;
      margin-bottom: 0.15em;
      font-weight: 500;
    }
  </style>

  <div class="teaching-section-title">QISCA Special Lecture Series:</div>
  <ul style="margin-top: 0.1em;">
    <li>
      Organizer &amp; Lecturer,
      <a href="/bosonic-learning-theory-winter26/" target="_blank"><i>Quantum Learning Theory for Bosonic and Fermionic Systems</i></a>,
      Winter 2026
    </li>
    <li>
      Invited Lecturer,
      <a href="/quantum-complexity-reading-group-fall25/" target="_blank"><i>Quantum Complexity Theory Reading Group</i></a>,
      Fall 2025
    </li>
    <li>
      Invited Lecturer,
      <a href="/qlct/" target="_blank"><i>Quantum Learning and Complexity Theory</i></a>,
      Summer 2025
    </li>
  </ul>

<div class="teaching-section-title">University-Industry Research Internship:</div>
<ul style="margin-top: 0.1em;">
  <li>
    Instructor,
    <i>AAA559: College of Informatics Internship (II) (Graduate Course)</i>,
    Korea University,
    Fall 2025
  </li>
  <li>
    Instructor,
    <i>AAA558: College of Informatics Internship (I) (Graduate Course)</i>,
    Korea University,
    Fall 2025
  </li>
  <li>
    Instructor,
    <i>SW4343: Software Field Placement (I)</i>,
    Korea Aerospace University,
    Fall 2024
  </li>
</ul>

<div class="teaching-section-title">Yonsei University:</div>
<ul style="margin-top: 0.1em;">
  <li>
    Teaching Assistant,
    <i>YCS1009: Change the World through Programming</i>,
    Fall 2022
  </li>
  <li>
    Teaching Assistant,
    <i>YCS1002: Software Programming</i>,
    Fall 2022
  </li>
  <li>
    Teaching Assistant,
    <i>EEE1108: Engineering Information Processing</i>,
    Fall 2021
  </li>
  <li>
    Course Tutor,
    <i>MAT2016: Engineering Mathematics (III)</i>,
    Spring 2022
    (Best Tutor Award)
  </li>
  <li>
    Course Tutor,
    <i>MAT1012: Engineering Mathematics (II)</i>,
    Fall 2021
    (Best Tutor Award)
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



<!-- <h5
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
      I enjoy playing table tennis and the piano, and I also like a wide variety of puzzle games. I was born in Asan, South Korea, and spent most of my life in Seoul.
    </p>

    <p>
        I am also particularly interested in the <a href="https://www.genealogy.math.ndsu.nodak.edu/" style="text-decoration:none;">Mathematics Genealogy Project</a>. By tracing the academic lineages of my advisors, I came across several fascinating connections. In particular, it was striking to encounter figures such as 
        <a href="https://en.wikipedia.org/wiki/Leonhard_Euler" style="text-decoration:none;">Leonhard Euler</a> (from Anurag Anshu), 
        <a href="https://en.wikipedia.org/wiki/Carl_Gustav_Jacob_Jacobi" style="text-decoration:none;">Carl Gustav Jacob Jacobi</a> (from Sitan Chen), and 
        <a href="https://en.wikipedia.org/wiki/Paul_Dirac" style="text-decoration:none;">Paul Dirac</a> (from Jordan Cotler) 
        along these lineages!
    </p>

    <p style="margin-top: 0.8em;">
      <a
        href="javascript:void(0);"
        onclick="toggleLineageList(event)"
        style="font-weight:400; text-decoration:none;"
      >
        <span id="lineage-toggle-text"> [See full list] </span>
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
      text.textContent = "[Hide full list]";
    } else {
      list.style.display = "none";
      text.textContent = "[See full list]";
    }

    setTimeout(() => {
      if (miscContent.style.maxHeight !== "0px") {
        miscContent.style.maxHeight = miscContent.scrollHeight + "px";
      }
    }, 10);
  }
</script> -->
