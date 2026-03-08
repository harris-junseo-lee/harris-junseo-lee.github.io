---
layout: page
permalink: /bosonic-learning-theory-winter26/
parent: Teaching
title: Quantum Learning Theory for Bosonic and Fermionic Systems (Winter 2026)
description: 2026 QISCA (Quantum Information Student Community Association) Winter School Program
nav: false
nav_order: 
# toc:
#   sidebar: left
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


#### Course Details
This winter school provides a focused introduction to quantum learning theory for bosonic and continuous-variable (CV) systems. Quantum learning theory seeks to understand how efficiently information can be extracted from quantum systems, yet most rigorous guarantees have traditionally been developed in finite-dimensional settings. In contrast, many experimental platforms, particularly those in quantum optics, operate in infinite-dimensional Hilbert spaces where theoretical learning guarantees have remained comparatively underdeveloped.

Recent progress has begun to close this gap by introducing new techniques for learning bosonic states, unitaries, and Hamiltonians under physically realistic constraints. The program will present these developments, explain the conceptual tools that drive them, and highlight emerging open directions at the interface of CV quantum information and quantum learning theory. In addition to bosonic systems, the school will also discuss several related results for fermionic systems.

**Prerequisites:** Participants are expected to have basic familiarity with quantum information theory and mathematical methods used in theoretical computer science. Knowledge of quantum states, channels, and measurements, as well as introductory concepts from learning theory such as sample complexity and concentration inequalities, will be helpful but not strictly required. Prior exposure to continuous-variable quantum information, including Gaussian states and operations, is advantageous but optional. Motivated students with strong mathematical interest are fully encouraged to participate.

#### Instructor
- **Main Organizer:** [Junseo Lee](https://harris-junseo-lee.github.io/) (Seoul National University, Harvard University)
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
- All lectures from our course have now been released as a public **[YouTube playlist](https://youtube.com/playlist?list=PLD-yYWNmQxZxDqJo25kkS-NWIh9jWT0NT&si=D5yztAx674aklQ8b)**.
- Please note that Lecture 6, scheduled for February 9, will take place at 2:00 PM (KST).

<!-- #### Acknowledgement
- We thank [Chirag Wadhwa](https://chirag-w.github.io/) for delivering an excellent special lecture on quantum state certification in Lecture 3.
- We thank [Antonio Anna Mele](https://antonioannamele.com/) for his work on Haar measure theory, which helped us structure the material for Lecture 5. -->

#### Lectures

<!-- All lectures are scheduled for <span style="color:#2e86c1;">Saturdays at 3 PM</span>, except <span style="color:#c0392b;">Lecture 2</span>, which will be held on Sunday. -->

<table style="border-collapse: collapse; width: 100%; font-size: 15px; border: 1px solid #ddd;">
  <thead style="background: #1f4e79; color: white;">
    <tr>
      <th style="padding: 12px; border: 1px solid #ddd; width: 170px;">Lecture</th>
      <th style="padding: 12px; border: 1px solid #ddd;">Topic</th>
      <th style="padding: 12px; border: 1px solid #ddd; width: 200px;">Lecturer</th>
      <th style="padding: 12px; border: 1px solid #ddd;">Readings</th>
    </tr>
  </thead>

  <tbody>

    <tr style="background:#f8fbff;">
      <td style="border: 1px solid #ddd; text-align:center; padding:10px;">Lecture 1 (Jan 16)</td>
      <td style="border: 1px solid #ddd; padding:10px;">Course Overview</td>
      <td style="border: 1px solid #ddd; padding:10px;">Junseo Lee</td>
      <td style="border: 1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://harris-junseo-lee.github.io/quantum-learning-theory-references/" target="_blank">Quantum Learning Theory Zoo</a></li>
          <li><a href="https://harris-junseo-lee.github.io/qlct/" target="_blank">Quantum Learning and Complexity Theory (Summer 2025)</a></li>
          <li><a href="https://www.nature.com/articles/s42254-023-00662-4" target="_blank">A survey on the complexity of learning quantum states</a></li>
          <li><a href="https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.77.513" target="_blank">Quantum information with continuous variables</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td style="border: 1px solid #ddd; text-align:center; padding:10px;">Lecture 2 (Jan 19)</td>
      <td style="border: 1px solid #ddd; padding:10px;">Tomography of Energy-Constrained and Bosonic Gaussian States</td>
      <td style="border: 1px solid #ddd; padding:10px;">
        Francesco Anna Mele <br>
        [<a href="/assets/pdf/BLT/Lecture2_Francesco.pdf"><b>Notes</b></a>,
        <a href="https://youtu.be/J8_KzazbYcw"><b>Video</b></a>]
      </td>
      <td style="border: 1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://www.nature.com/articles/s41567-025-03086-2" target="_blank">Learning quantum states of continuous-variable systems</a></li>
          <li><a href="https://quantum-journal.org/papers/q-2025-06-12-1769/" target="_blank">Optimal estimates of trace distance between bosonic Gaussian states and applications to learning</a></li>
          <li><a href="https://arxiv.org/abs/2508.14979" target="_blank">Energy-independent tomography of Gaussian states</a></li>
        </ul>
      </td>
    </tr>

    <tr style="background:#f8fbff;">
      <td style="border: 1px solid #ddd; text-align:center; padding:10px;">Lecture 3 (Jan 21)</td>
      <td style="border: 1px solid #ddd; padding:10px;">Learning t-Doped Fermionic and Bosonic Gaussian States</td>
      <td style="border: 1px solid #ddd; padding:10px;">
        Antonio Anna Mele <br>
        [<a href="/assets/pdf/BLT/Lecture3_Antonio.pdf"><b>Notes</b></a>,
        <a href="https://youtu.be/tjAtRf_cpvM"><b>Video</b></a>]
      </td>
      <td style="border: 1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.6.010319" target="_blank">Efficient Learning of Quantum States Prepared With Few Fermionic Non-Gaussian Gates</a></li>
          <li><a href="https://www.nature.com/articles/s41567-025-03086-2" target="_blank">Learning quantum states of continuous-variable systems</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td colspan="4" style="border:1px solid #ddd; text-align:center; padding:12px; background:#eef4fb; font-weight:500;">
        QIP 2026 (Jan 24 – Jan 30) · No Class
      </td>
    </tr>

    <tr style="background:#f8fbff;">
      <td style="border: 1px solid #ddd; text-align:center; padding:10px;">Lecture 4 (Feb 2)</td>
      <td style="border: 1px solid #ddd; padding:10px;">Gaussianity Testing of Bosonic Quantum States</td>
      <td style="border: 1px solid #ddd; padding:10px;">
        Filippo Girardi <br>
        [<a href="/assets/pdf/BLT/Lecture4_Filippo.pdf"><b>Notes</b></a>,
        <a href="https://youtu.be/i1Qrj-UPCMI"><b>Video</b></a>]
      </td>
      <td style="border: 1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2510.07305v1" target="_blank">Is it Gaussian? Testing bosonic quantum states</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td style="border: 1px solid #ddd; text-align:center; padding:10px;">Lecture 5 (Feb 5)</td>
      <td style="border: 1px solid #ddd; padding:10px;">Hamiltonian Learning for Bosonic Gaussian States</td>
      <td style="border: 1px solid #ddd; padding:10px;">
        Marco Fanizza <br>
        [<a href="/assets/pdf/BLT/Lecture5_Marco.pdf"><b>Notes</b></a>,
        <a href="https://youtu.be/H2BAFZhQ3_I"><b>Video</b></a>]
      </td>
      <td style="border: 1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2411.03163" target="_blank">Efficient Hamiltonian, structure and trace distance learning of Gaussian states</a></li>
        </ul>
      </td>
    </tr>

    <tr style="background:#f8fbff;">
      <td style="border: 1px solid #ddd; text-align:center; padding:10px;">Lecture 6 (Feb 9)</td>
      <td style="border: 1px solid #ddd; padding:10px;">Learning t-Doped Fermionic Unitaries</td>
      <td style="border: 1px solid #ddd; padding:10px;">
        Vishnu Iyer <br>
        [<a href="https://youtu.be/pEx7CgVYSBw"><b>Video</b></a>]
      </td>
      <td style="border: 1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.3.020328" target="_blank">Fermion Sampling</a></li>
          <li><a href="https://arxiv.org/abs/2504.11318v2" target="_blank">Mildly-Interacting Fermionic Unitaries are Efficiently Learnable</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td style="border: 1px solid #ddd; text-align:center; padding:10px;">Lecture 7 (Feb 12)</td>
      <td style="border: 1px solid #ddd; padding:10px;">Learning Bosonic Gaussian Unitaries</td>
      <td style="border: 1px solid #ddd; padding:10px;">
        Junseo Lee <br>
        [<a href="/assets/pdf/BLT/Lecture7_Junseo.pdf"><b>Notes</b></a>]
      </td>
      <td style="border: 1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2510.05531v1" target="_blank">Efficient learning of bosonic Gaussian unitaries</a></li>
        </ul>
      </td>
    </tr>

  </tbody>
</table>
