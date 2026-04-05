---
layout: page
permalink: /quantum-complexity-reading-group-fall25/
parent: Teaching
title: Quantum Complexity Theory Reading Group (Fall 2025)
description: 2025 QISCA (Quantum Information Student Community Association) Study Group Program
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
This reading group is dedicated to exploring both foundational and recent research in quantum complexity theory. Over the course of 11 weeks, we will study key papers and results covering topics such as quantum computational complexity, Hamiltonian complexity, and quantum circuit complexity. The sessions will combine short theoretical lectures with student-led presentations and discussions of selected papers.

**Prerequisites:** Participants are expected to have a solid background in theoretical computer science and quantum information. Familiarity with computational complexity theory (e.g., P, NP, BQP, QMA) and basic quantum computing concepts (quantum states, unitaries, and measurements) will be assumed. Prior exposure to quantum algorithms or quantum complexity theory is helpful but not strictly required; motivated students with strong mathematical preparation are welcome.

#### Instructor
- [Junseo Lee](https://harris-junseo-lee.github.io/) (Seoul National University)

#### Course Policies
- The reading group will be conducted primarily via Zoom. In-person sessions may be organized when necessary.
- All participants are required to attend every session, regardless of whether it is their presentation day. To ensure active discussion, cameras must remain on during class.
- Each student is expected to give at least one paper review presentation during the course.
- Presentation slides must be submitted to the instructor no later than the day before the presentation. Students who are not presenting are expected to read the paper in advance and prepare questions.


#### Announcements
- (Sep 25) The paper list has been released. Students will select their presentation topics on a first-come, first-served basis.

<!-- #### Acknowledgement
- We thank [Chirag Wadhwa](https://chirag-w.github.io/) for delivering an excellent special lecture on quantum state certification in Lecture 3.
- We thank [Antonio Anna Mele](https://antonioannamele.com/) for his work on Haar measure theory, which helped us structure the material for Lecture 5. -->

#### Lectures

<!-- All lectures are scheduled for <span style="color:#2e86c1;">Saturdays at 3 PM</span>, except <span style="color:#c0392b;">Lecture 2</span>, which will be held on Sunday. -->

<table style="border-collapse: collapse; width: 100%; font-size: 15px; border: 1px solid #ddd; color:#000;">
  <thead style="background:#1f4e79; color:white;">
    <tr>
      <th style="padding:12px; border:1px solid #ddd; width:120px;">Week</th>
      <th style="padding:12px; border:1px solid #ddd;">Topic</th>
      <th style="padding:12px; border:1px solid #ddd; width:200px;">Speaker</th>
      <th style="padding:12px; border:1px solid #ddd;">Readings</th>
    </tr>
  </thead>

  <tbody>

    <tr style="background:#f8fbff;">
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">1</td>
      <td style="border:1px solid #ddd; padding:10px;">Foundational Concepts</td>
      <td style="border:1px solid #ddd; padding:10px;">Junseo Lee</td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/0804.3401">[Wat'08] Quantum Computational Complexity</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">2</td>
      <td style="border:1px solid #ddd; padding:10px;">Complexity Theory for NISQ Devices</td>
      <td style="border:1px solid #ddd; padding:10px;">
        Sung-Bin Lee <br> <a href="/assets/pdf/QC_reading/2_NISQComplexity.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2210.07234">[CCHL'22] The Complexity of NISQ</a></li>
        </ul>
      </td>
    </tr>

    <tr style="background:#f8fbff;">
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">3</td>
      <td style="border:1px solid #ddd; padding:10px;">Complexity Theory, Unitary Designs, and Randomness</td>
      <td style="border:1px solid #ddd; padding:10px;">
        Seonggeun Park <br> <a href="/assets/pdf/QC_reading/3_ComplexityGrowth.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/1912.04297">[BCHKP'19] Models of quantum complexity growth</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">4</td>
      <td style="border:1px solid #ddd; padding:10px;">Understanding BQP</td>
      <td style="border:1px solid #ddd; padding:10px;">
        Jaehun Han <br> <a href="/assets/pdf/QC_reading/4_BQP.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2111.10409">[AIK'24] The Acrobatics of BQP</a></li>
          <li><a href="https://arxiv.org/abs/2508.02514">[GS'25] Forrelation is Extremally Hard</a></li>
        </ul>
      </td>
    </tr>

    <tr style="background:#f8fbff;">
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">5</td>
      <td style="border:1px solid #ddd; padding:10px;">Quantum State Property Testing and Complexity</td>
      <td style="border:1px solid #ddd; padding:10px;">
        JungMo Lee <br> <a href="/assets/pdf/QC_reading/5_trace_of_power.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2410.13559">[LW'25] On estimating the trace of quantum state powers</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">6</td>
      <td style="border:1px solid #ddd; padding:10px;">Quantum Interactive Proof Systems (I)</td>
      <td style="border:1px solid #ddd; padding:10px;">
        Hyuntaek Shin <br> <a href="/assets/pdf/QC_reading/6_NEEXP_MIPstar.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/1904.05870">[NW'19] NEEXP ⊆ MIP*</a></li>
        </ul>
      </td>
    </tr>

    <tr style="background:#f8fbff;">
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">7</td>
      <td style="border:1px solid #ddd; padding:10px;">Quantum Interactive Proof Systems (II)</td>
      <td style="border:1px solid #ddd; padding:10px;">
        Hyungmin Lim <br> <a href="/assets/pdf/QC_reading/7_MIPstar=RE.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2001.04383">[JNVWY'22] MIP* = RE</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">8</td>
      <td style="border:1px solid #ddd; padding:10px;">NLTS Hamiltonians</td>
      <td style="border:1px solid #ddd; padding:10px;">
        Eunsoo Eun <br> <a href="/assets/pdf/QC_reading/8_NLTS.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2206.13228">[ABN'22] NLTS Hamiltonians from good quantum codes</a></li>
          <li><a href="https://arxiv.org/abs/2311.09503">[GK'23] NLTS Hamiltonians and Strongly-Explicit SoS Lower Bounds from Low-Rate Quantum LDPC Codes</a></li>
        </ul>
      </td>
    </tr>

    <tr style="background:#f8fbff;">
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">9</td>
      <td style="border:1px solid #ddd; padding:10px;">Quantum PCPs</td>
      <td style="border:1px solid #ddd; padding:10px;">
        Gyuhyun Kim <br> <a href="/assets/pdf/QC_reading/9_QPCP.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2403.04841">[BHW'25] Quantum PCPs</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">10</td>
      <td style="border:1px solid #ddd; padding:10px;">Hamiltonian Complexity and Fault Tolerance</td>
      <td style="border:1px solid #ddd; padding:10px;">
        Jeongbin Jo <br> <a href="/assets/pdf/QC_reading/10_Circ2Ham.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2309.16475">[ABN'24] Circuit-to-Hamiltonian from tensor networks and fault tolerance</a></li>
        </ul>
      </td>
    </tr>

    <tr style="background:#f8fbff;">
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">11</td>
      <td style="border:1px solid #ddd; padding:10px;">Quantum Complexity and Cryptography</td>
      <td style="border:1px solid #ddd; padding:10px;">
        InHee Yun <br>  <a href="/assets/pdf/QC_reading/11_OneQuery.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/abs/2310.08870">[LMW'23] A one-query lower bound for unitary synthesis and breaking quantum cryptography</a></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td style="border:1px solid #ddd; text-align:center; padding:10px;">12</td>
      <td style="border:1px solid #ddd; padding:10px;">Computational Power of QAC0</td>
      <td style="border:1px solid #ddd; padding:10px;">
        Wonjun Baek <br> <a href="/assets/pdf/QC_reading/12_QAC0.pdf">[Slides]</a>
      </td>
      <td style="border:1px solid #ddd; padding:10px;">
        <ul style="margin:0; padding-left:18px;">
          <li><a href="https://arxiv.org/pdf/2410.06499">[ADOY'25] On the Computational Power of QAC0 with Barely Superlinear Ancillae</a></li>
        </ul>
      </td>
    </tr>

  </tbody>
</table>