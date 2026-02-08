---
layout: page
permalink: /bosonic-learning-theory-winter26/
parent: Teaching
title: Quantum Learning Theory for Bosonic Systems (Winter 2026)
description:
nav: false
nav_order: 
# toc:
#   sidebar: left
---
<html>
    <head>
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Bitter:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">
        <style>
            body {
                font-family: "Bitter", serif;
                font-optical-sizing: auto;
                font-weight: 350;
                font-size: 1rem;
            }
            strong, b {
            font-weight: 600;
            }
            h1 { font-weight: 450; }
            h2 { font-weight: 450; }
            h3 { font-weight: 450; }
            h4, h5, h6 { font-weight: 450; }
        </style>
    </head>
</html>

#### Course Details
This winter school provides a focused introduction to quantum learning theory for bosonic and continuous-variable (CV) systems. Quantum learning theory seeks to understand how efficiently information can be extracted from quantum systems, yet most rigorous guarantees have traditionally been developed in finite-dimensional settings. In contrast, many experimental platforms, particularly those in quantum optics, operate in infinite-dimensional Hilbert spaces where theoretical learning guarantees have remained comparatively underdeveloped.

Recent progress has begun to close this gap by introducing new techniques for learning bosonic states, unitaries, and Hamiltonians under physically realistic constraints. The program will present these developments, explain the conceptual tools that drive them, and highlight emerging open directions at the interface of CV quantum information and quantum learning theory. In addition to bosonic systems, the school will also discuss several related results for fermionic systems.

**Prerequisites:** Participants are expected to have basic familiarity with quantum information theory and mathematical methods used in theoretical computer science. Knowledge of quantum states, channels, and measurements, as well as introductory concepts from learning theory such as sample complexity and concentration inequalities, will be helpful but not strictly required. Prior exposure to continuous-variable quantum information, including Gaussian states and operations, is advantageous but optional. Motivated students with strong mathematical interest are fully encouraged to participate.

#### Instructor
- **Main Organizer:** [Junseo Lee](https://harris-junseo-lee.github.io/) (Seoul National University, `harris.junseo(at)gmail.com`)
- **Invited Lecturers** (in alphabetical order):
  - [Marco Fanizza](https://quriosity.telecom-paris.fr/author/marco-fanizza/) (Inria, Télécom Paris - LTCI, Institut Polytechnique de Paris)
  - Filippo Girardi (Scuola Normale Superiore)
  - [Vishnu Iyer](https://vishnuiyer.org/) (University of Texas at Austin)
  - [Antonio Anna Mele](https://antonioannamele.com/) (Freie Universität Berlin)
  - [Francesco Anna Mele](https://sites.google.com/sns.it/francescoannamele/about-me) (Scuola Normale Superiore)

#### Course Policies
- All lectures will be conducted in English.
- All lectures are scheduled for 5:00 PM (KST) and may be adjusted depending on speaker availability.


#### Announcements
- TBA.

<!-- #### Acknowledgement
- We thank [Chirag Wadhwa](https://chirag-w.github.io/) for delivering an excellent special lecture on quantum state certification in Lecture 3.
- We thank [Antonio Anna Mele](https://antonioannamele.com/) for his work on Haar measure theory, which helped us structure the material for Lecture 5. -->

#### Lectures

<!-- All lectures are scheduled for <span style="color:#2e86c1;">Saturdays at 3 PM</span>, except <span style="color:#c0392b;">Lecture 2</span>, which will be held on Sunday. -->

<table style="border-collapse: collapse; width: 100%; border: 1px solid #ccc;">
  <thead style="background-color: #2e86c1; color: white;">
    <tr>
      <th style="padding: 10px; border: 1px solid #ccc;"> </th>
      <th style="padding: 10px; border: 1px solid #ccc;">Topic</th>
      <th style="padding: 10px; border: 1px solid #ccc;">Lecturer</th>
      <th style="padding: 10px; border: 1px solid #ccc;">Readings</th>
    </tr>
  </thead>
  <tbody>
    <!-- <tr style="background-color: #f9f9f9;">
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 1 (12/29)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Course Overview</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Junseo Lee</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://harris-junseo-lee.github.io/quantum-learning-theory-references/" target="_blank" rel="noopener">Quantum Learning Theory Zoo</a></li>
        </ul>
      </td>
    </tr> -->
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 1 (1/16)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Course Overview</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Junseo Lee</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://harris-junseo-lee.github.io/quantum-learning-theory-references/" target="_blank" rel="noopener">Quantum Learning Theory Zoo</a></li>
          <li><a href="https://harris-junseo-lee.github.io/qlct/" target="_blank" rel="noopener">Quantum Learning and Complexity Theory (Summer 2025)</a></li>
          <li><a href="https://www.nature.com/articles/s42254-023-00662-4" target="_blank" rel="noopener">A survey on the complexity of learning quantum states</a></li>
          <li><a href="https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.77.513" target="_blank" rel="noopener">Quantum information with continuous variables</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 2 (1/19)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Tomography of Energy-Constrained and Bosonic Gaussian States</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Francesco Anna Mele <br> [<a href="/assets/pdf/BLT/Lecture2_Francesco.pdf"><b>Notes</b></a>, <a href="https://youtu.be/J8_KzazbYcw?si=kzmByzS09Yl2S-eC"><b>Video</b></a>] </span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://www.nature.com/articles/s41567-025-03086-2" target="_blank" rel="noopener">Learning quantum states of continuous-variable systems</a></li>
          <li><a href="https://quantum-journal.org/papers/q-2025-06-12-1769/" target="_blank" rel="noopener">Optimal estimates of trace distance between bosonic Gaussian states and applications to learning</a></li>
          <li><a href="https://arxiv.org/abs/2508.14979" target="_blank" rel="noopener">Energy-independent tomography of Gaussian states</a></li>
        </ul>
      </td>
    </tr>
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 3 (1/21)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Learning t-Doped Fermionic and Bosonic Gaussian States</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Antonio Anna Mele <br> [<a href="https://youtu.be/tjAtRf_cpvM?si=AMCp2z9Fk8RGlexJ"><b>Video</b></a>] </span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.6.010319" target="_blank" rel="noopener">Efficient Learning of Quantum States Prepared With Few Fermionic Non-Gaussian Gates</a></li>
          <li><a href="https://www.nature.com/articles/s41567-025-03086-2" target="_blank" rel="noopener">Learning quantum states of continuous-variable systems</a></li>
        </ul>
      </td>
    </tr>
    <tr>
    <td colspan="4" style="border: 1px solid #ccc; text-align: center;">
      <span style="color:#000000;">QIP 2026 (1/24–1/30) · No Class</span>
    </td>
    </tr>
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 4 (2/2)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Gaussianity Testing of Bosonic Quantum States</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Filippo Girardi <br> [<a href="/assets/pdf/BLT/Lecture4_Filippo.pdf"><b>Notes</b></a>, <a href="https://youtu.be/i1Qrj-UPCMI?si=j2O0x-MiwcoJ9dqM"><b>Video</b></a>] </span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://arxiv.org/abs/2510.07305v1" target="_blank" rel="noopener">Is it Gaussian? Testing bosonic quantum states</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 5 (2/5)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Hamiltonian Learning for Bosonic Gaussian States</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Marco Fanizza <br> [<a href="/assets/pdf/BLT/Lecture5_Marco.pdf"><b>Notes</b></a>, <a href="https://youtu.be/H2BAFZhQ3_I?si=kuBjlpUV22MLK0xJ"><b>Video</b></a>] </span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://arxiv.org/abs/2411.03163" target="_blank" rel="noopener">Efficient Hamiltonian, structure and trace distance learning of Gaussian states</a></li>
        </ul>
      </td>
    </tr>
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 6 (2/9)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Learning t-Doped Fermionic Unitaries</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Vishnu Iyer</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.3.020328" target="_blank" rel="noopener">Fermion Sampling: A Robust Quantum Computational Advantage Scheme Using Fermionic Linear Optics and Magic Input States</a></li>
          <li><a href="https://arxiv.org/abs/2504.11318v2" target="_blank" rel="noopener">Mildly-Interacting Fermionic Unitaries are Efficiently Learnable</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 7 (2/12)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Learning Bosonic Gaussian Unitaries</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Junseo Lee</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://arxiv.org/abs/2510.05531v1" target="_blank" rel="noopener">Efficient learning of bosonic Gaussian unitaries</a></li>
        </ul>
      </td>
    </tr>
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 8 (2/16)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBD</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBD</span></td>
      <td style="border: 1px solid #ccc;"> TBD
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc; text-align: center;"><span style="color:#000000;">Lecture 9 (2/19)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBD</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBD</span></td>
      <td style="border: 1px solid #ccc;"> TBD
      </td>
    </tr>
  </tbody>
</table>
