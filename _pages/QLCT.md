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
- Lectures will primarily be delivered online through Zoom. Details for accessing the sessions will be provided later. The final lecture may optionally be held in person, subject to circumstances, and may include a Q&A session.
- Submission of the problem set is not mandatory. However, solutions will not be provided, and they will not be discussed during class. Students who submit their solutions will receive individual feedback.
<!-- - Recordings of lectures will not be available. -->

#### **Announcements**
- (Jul 25) The materials for the Week 3 (Special Lecture), including the recorded video, have been updated. The video will remain freely accessible until further notice.
- (Jul 17) Problem Set 2 has been posted.
- (Jul 14) Problem Set 1 has been posted.
- (Jul 7) All students who wish to enroll in this course are required to complete the following survey before the first lecture: [Survey Link](https://forms.gle/3qEH93qKtV1oZw6E6)

#### **Lectures**

<!-- All lectures are scheduled for <span style="color:#2e86c1;">Saturdays at 3 PM</span>, except <span style="color:#c0392b;">Lecture 2</span>, which will be held on Sunday. -->

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
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Jul 12 (Sat)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Overview of quantum learning theory</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;"><a href="/assets/pdf/QLCT/QLCT_Lec1.pdf">Lec 1</a>, <a href="/assets/pdf/QLCT/QLCT_Pset1.pdf">Pset 1</a> </span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/2897518.2897585">[HHJWY'16] Sample-optimal tomography of quantum states</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/2897518.2897544">[OW'16] Efficient quantum tomography</a></li>
          <li><a href="https://doi.org/10.1145/3106700.3106710">[AdW'17] A Survey of Quantum Learning Theory</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/3188745.3188802">[Aar'18] Shadow tomography of quantum states</a></li>
          <li><a href="https://www.nature.com/articles/s41567-020-0932-7">[HKP'20] Predicting many properties of a quantum system from very few measurements</a></li>
          <li><a href="https://dl.acm.org/doi/10.1145/3406325.3451109">[BO'21] Improved Quantum data analysis</a></li>
          <li><a href="https://www.computer.org/csdl/proceedings-article/focs/2022/205500a574/1BtftZspUxa">[CCHL’21] Exponential Separations Between Learning With and Without Quantum Memory</a></li>
          <li><a href="https://www.computer.org/csdl/proceedings-article/focs/2023/189400a391/1T96YaMKga4">[CHLLS’22] When Does Adaptivity Help for Quantum State Learning?</a></li>
          <li><a href="https://www.computer.org/csdl/proceedings-article/focs/2022/551900b205/1JtvVrKAv9S">[CHLL’22] Tight Bounds for Quantum State Certification with Incoherent Measurements</a></li>
          <li> Some parts of these lecture notes were inspired by Jerry Li’s presentation slides, which can be found <a href="https://youtu.be/GzyyC56p-as?si=GVEWJZkdrBJLXasy">here</a>. </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Jul 20 (Sun)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Haar measures and unitary designs</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;"><a href="/assets/pdf/QLCT/QLCT_Lec2.pdf">Lec 2</a>, <a href="/assets/pdf/QLCT/QLCT_Pset2.pdf">Pset 2</a> </span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://quantum-journal.org/papers/q-2024-05-08-1340/#">[Mel'23] Introduction to Haar Measure Tools in Quantum Information</a></li>
          <li><a href="https://arxiv.org/pdf/2507.06216">[CSBH'25] Unitary designs in nearly optimal depth</a></li>
          <li><a href="https://www.science.org/doi/10.1126/science.adv8590">[SHH'25] Random unitaries in extremely low depth</a></li>
          <li><a href="https://dl.acm.org/doi/pdf/10.1145/3717823.3718254">[MH'25] How to Construct Random Unitaries</a></li>
          <li><a href="https://pennylane.ai/qml/demos/tutorial_unitary_designs">PennyLane Demos: Unitary designs</a></li>
        </ul>
      </td>
    </tr>
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Jul 25 (Fri)</span></td>
      <!-- <td style="border: 1px solid #ccc;"><span style="color:#000000;">Quantum state certification (Special Guest Lectuer by Chirag Wadhwa)</span></td> -->
      <td style="border: 1px solid #ccc; padding: 8px;">
        <span style="color:#000000;">
          Quantum state certification<br>
          <small>* Special Guest Lecture by 
            <a href="https://chirag-w.github.io/">
              Chirag Wadhwa
            </a>
          </small>
        </span>
      </td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;"><a href="/assets/pdf/QLCT/QLCT_Lec3.pdf">Lec 3</a>, <a href="https://drive.google.com/file/d/1gEwIOjYtUgDb3sgVmdE_-scmigWDss7r/view?usp=sharing">Video</a> </span></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://link.springer.com/chapter/10.1007/978-3-540-70918-3_51">[CHW'07] Weak Fourier-Schur sampling, the hidden subgroup problem, and the quantum collision problem</a></li>
          <li><a href="https://dl.acm.org/doi/10.1145/2746539.2746582">[OW'15] Quantum Spectrum Testing</a></li>
          <li><a href="https://dl.acm.org/doi/10.1145/3313276.3316344">[BOW'19] Quantum state certification</a></li>
          <li><a href="https://proceedings.mlr.press/v178/chen22b.html">[CLO'22] Toward Instance-Optimal State Certification With Incoherent Measurements</a></li>
          <li><a href="https://www.computer.org/csdl/proceedings-article/focs/2022/551900b205/1JtvVrKAv9S">[CLHL'22] Tight Bounds for Quantum State Certification with Incoherent Measurements</a></li>
          <li><a href="https://arxiv.org/abs/2507.06010">[OW'25] Instance-Optimal Quantum State Certification with Entangled Measurements</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 02 (Sat)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Quantum property testing</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;"></span><a href="/assets/pdf/QLCT/QLCT_Lec4.pdf">Lec 4</a></td>
      <td style="border: 1px solid #ccc;">
        <ul>
          <li><a href="https://arxiv.org/pdf/quant-ph/0005055">[BHMT'00] Quantum Amplitude Amplification and Estimation</a></li>
          <li><a href="https://arxiv.org/pdf/1310.2035">[MW'18] A Survey of Quantum Property Testing</a></li>
          <li><a href="https://arxiv.org/pdf/1902.00814">[GL'19] Distributional property testing in a quantum world</a></li>
          <li><a href="https://arxiv.org/pdf/1806.01838">[GSLW'18] Quantum singular value transformation and beyond: exponential improvements for quantum matrix arithmetics</a></li>
          <li><a href="https://www.nature.com/articles/s41534-021-00379-1">[GGZW'21] Iterative quantum amplitude estimation</a></li>
          <li><a href="https://arxiv.org/pdf/2301.06783">[WZ'23] Fast Quantum Algorithms for Trace Distance Estimation</a></li>
        </ul>
      </td>
    </tr>
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 09 (Sat)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Classical shadows</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;"></span></td>
      <td style="border: 1px solid #ccc;">
        <!-- <ul>
          <li><a href="https://link.springer.com/article/10.1007/s11128-023-04253-1">Shin et al.: Estimating quantum mutual information through a quantum neural network</a></li>
          <li><a href="https://journals.aps.org/pra/abstract/10.1103/PhysRevA.110.062418">Shin et al.: Disentangling quantum neural networks for unified estimation of quantum entropies and distance measures</a></li>
          <li><a href="https://journals.aps.org/pra/abstract/10.1103/PhysRevA.109.032431">Goldfeld et al.: Quantum Neural Estimation of Entropies</a></li>
        </ul> -->
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 16 (Sat)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Complexity of learning quantum states</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;"></span></td>
      <td style="border: 1px solid #ccc;">
        <!-- <ul>
          <li><a href="https://www.nature.com/articles/s42254-023-00662-4">Anshu & Arunachalam: A survey on the complexity of learning quantum states
</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/3188745.3188802">Aaronson: Shadow tomography of quantum states</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/2897518.2897585">Haah et al.: Sample-optimal tomography of quantum states</a></li>
          <li><a href="https://dl.acm.org/doi/abs/10.1145/2897518.2897544">O'Donnell & Wright: Efficient quantum tomography</a></li>
        </ul> -->
      </td>
    </tr>
    <!-- <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 16</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Quantum complexity and homology problems</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;"></span></td>
      <td style="border: 1px solid #ccc;"> -->
        <!-- <ul>
          <li><a href="https://www.nature.com/articles/ncomms10138">Lloyd et al.: Quantum algorithms for topological and geometric analysis of data
</a></li>
          <li><a href="https://www.nature.com/articles/s41467-024-54118-z">Crichigno & Kohler: Clique Homology is QMA1-hard</a></li>
          <li><a href="https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.4.040349">Schmidhuber & Lloyd: Complexity-Theoretic Limitations on Quantum Algorithms for Topological Data Analysis</a></li>
          <li><a href="https://arxiv.org/abs/2506.01432">Lee & Nghiem: New aspects of quantum topological data analysis: Betti number estimation, and testing and tracking of homology and cohomology classes</a></li>
          <li><a href="https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.5.010319">Berry at el.: Analyzing Prospects for Quantum Advantage in Topological Data Analysis</a></li>
          <li><a href="https://quantum-journal.org/papers/q-2022-11-10-855/">Gyurik et al.: Towards quantum advantage via topological data analysis</a></li>
        </ul> -->
      <!-- </td>
    </tr> -->
    <tr style="background-color: #f9f9f9; color:black;">
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 23 (Sat)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Learning quantum circuits and unitaries</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;"></span></td>
      <td style="border: 1px solid #ccc;">
        <!-- <ul>
          <li><a href="https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.5.040306">Zhao et al.: Learning Quantum States and Unitaries of Bounded Gate Complexity</a></li>
          <li><a href="https://dl.acm.org/doi/10.1145/3618260.3649722">Huang et al.: Learning Shallow Quantum Circuits</a></li>
        </ul> -->
      </td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Aug 30 (Sat)</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;">Open problems and discussion session</span></td>
      <td style="border: 1px solid #ccc;"><span style="color:#000000;"></span></td>
      <td style="border: 1px solid #ccc;">
        <!-- <ul>
          <li><a href="https://jerryzli.github.io/focs24-workshop.html">FOCS 2024 Workshop: Recent Advances in Quantum Learning</a></li>
        </ul> -->
      </td>
    </tr>
  </tbody>
</table>
