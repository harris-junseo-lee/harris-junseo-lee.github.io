---
layout: page
permalink: /qlct/
title: Quantum Learning and Complexity Theory
description: 2025 Summer QISCA (Quantum Information Student Community Association) Summer School Program
nav: false
nav_order: 0
# toc:
#   sidebar: left
---

#### **Course Details**
This course is an introductory-level overview of quantum learning theory and quantum complexity theory. It covers fundamental tools for analyzing the sample complexity of basic quantum learning tasks, including techniques involving the Haar measure. The course also explores core algorithms for learning quantum states, unitaries, processes, and circuits. In addition, it introduces important quantum complexity classes and provides the theoretical computer science background needed to understand foundational papers in quantum computation. The course will also touch on recent research trends in the field. The exact topics covered may be adjusted based on the interests of the participants.

**Prerequisites:** This course assumes that participants are already familiar with linear algebra, probability theory, and the basics of quantum information theory. Students are expected to be comfortable with the density matrix formalism, POVMs, Pauli matrices, the Bloch sphere representation, basic quantum channels (such as depolarizing and dephasing channels), and the properties of unitary and Hermitian matrices, including their spectral decompositions. Familiarity with tensor product notation, partial trace, and entanglement measures such as the von Neumann entropy and mutual information is also assumed. These topics will not be reviewed during the course, so students without this background may find it difficult to follow the material.

#### **Instructor**
- [Junseo Lee](https://harris-junseo-lee.github.io/) (SNU-Team QST, `harris.junseo(at)gmail.com`)
- [Myeongjin Shin](https://scholar.google.com/citations?user=9mRACrMAAAAJ&hl=en) (KAIST and SNU-Team QST, `hanwoolmj(at)kaist.ac.kr`)

#### **Course Policies**
- Recordings of lectures will not be available.
- Lectures will primarily be delivered online through Zoom. Details for accessing the sessions will be provided later. The final lecture may optionally be held in person, subject to circumstances, and may include a Q&A session.

#### **Announcements**
- TBA.

#### **Lectures**

All lectures are scheduled for <span style="color:#2e86c1;">Saturdays at 3 PM</span>, except <span style="color:#c0392b;">Lecture 2</span>, which will be held on Sunday.

<table style="border-collapse: collapse; width: 100%; border: 1px solid #ccc;">
  <thead style="background-color: #2e86c1; color: white;">
    <tr>
      <th style="padding: 10px; border: 1px solid #ccc;">Date</th>
      <th style="padding: 10px; border: 1px solid #ccc;">Title</th>
      <th style="padding: 10px; border: 1px solid #ccc;">Lecture Notes</th>
      <th style="padding: 10px; border: 1px solid #ccc;">Helpful References</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color: #f9f9f9;">
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Jul 12</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Overview of quantum learning theory</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBA</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://doi.org/10.1145/3106700.3106710">Arunachalam & de Wolf: Guest Column: A Survey of Quantum Learning Theory</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Jul 20</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Haar measures and classical shadows (1)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBA</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://quantum-journal.org/papers/q-2024-05-08-1340/#">Mele: Introduction to Haar Measure Tools in Quantum Information</a></li>
          <li><a href="https://pennylane.ai/qml/demos/tutorial_haar_measure">PennyLane Demos: Understanding the Haar measure</a></li>
        </ul>
      </td>
    </tr>
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Jul 26</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Haar measures and classical shadows (2)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBA</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://quantum-journal.org/papers/q-2024-05-08-1340/#">Mele: Introduction to Haar Measure Tools in Quantum Information</a></li>
          <li><a href="https://www.nature.com/articles/s41567-020-0932-7">Huang et al.: Predicting many properties of a quantum system from very few measurements</a></li>
          <li><a href="https://pennylane.ai/qml/demos/tutorial_classical_shadows">PennyLane Demos: Classical shadows</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 02</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Quantum property neural estimation</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBA</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://link.springer.com/article/10.1007/s11128-023-04253-1">Shin et al.: Estimating quantum mutual information through a quantum neural network</a></li>
          <li><a href="https://journals.aps.org/pra/abstract/10.1103/PhysRevA.110.062418">Shin et al.: Disentangling quantum neural networks for unified estimation of quantum entropies and distance measures</a></li>
          <li><a href="https://journals.aps.org/pra/abstract/10.1103/PhysRevA.109.032431">Goldfeld et al.: Quantum Neural Estimation of Entropies</a></li>
        </ul>
      </td>
    </tr>
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 09</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Complexity of learning quantum states (1)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBA</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://www.nature.com/articles/s42254-023-00662-4">Anshu & Arunachalam: A survey on the complexity of learning quantum states
</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/3188745.3188802">Aaronson: Shadow tomography of quantum states</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/2897518.2897585">Haah et al.: Sample-optimal tomography of quantum states</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/2897518.2897544">O'Donnell & Wright: Efficient quantum tomography</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 16</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Complexity of learning quantum states (2)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBA</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://www.nature.com/articles/s42254-023-00662-4">Anshu & Arunachalam: A survey on the complexity of learning quantum states
</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/3188745.3188802">Aaronson: Shadow tomography of quantum states</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/2897518.2897585">Haah et al.: Sample-optimal tomography of quantum states</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/2897518.2897544">O'Donnell & Wright: Efficient quantum tomography</a></li>
        </ul>
      </td>
    </tr>
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 23</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Learning quantum circuits and unitaries</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBA</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.5.040306">Zhao et al.: Learning Quantum States and Unitaries of Bounded Gate Complexity</a></li>
          <li><a href="https://dl.acm.org/doi/10.1145/3618260.3649722">Huang et al.: Learning Shallow Quantum Circuits</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 30</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Open problems and discussion session</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">TBA</span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://jerryzli.github.io/focs24-workshop.html">FOCS 2024 Workshop: Recent Advances in Quantum Learning</a></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
