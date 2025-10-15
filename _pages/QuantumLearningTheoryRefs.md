---
permalink: /quantum-learning-theory-references/
title: QLT Zoo
nav: true
nav_order: 7
---

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Quantum Learning Theory Zoo</title>
  <style>
    body { background: #ffffff; color: #111; font-family: system-ui, -apple-system, Segoe UI, Roboto, Inter, Arial, "Noto Sans", sans-serif; margin: 0; padding: 0; }
    a { color: #0056b3; text-decoration: none; }
    a:hover { text-decoration: underline; }
    .container { max-width: 1050px; margin: 0 auto; padding: 24px; }
    header { display:flex; align-items:center; justify-content:space-between; gap: 16px; margin-bottom: 16px; }
    .title { font-size: clamp(22px, 3vw, 32px); font-weight: 700; }
    .desc { color: #444; max-width: 880px; margin-top: 4px; }
    .panel { background: #f7f7f7; border: 1px solid #ddd; border-radius: 14px; padding: 16px; }
    .controls { display: grid; grid-template-columns: 2fr 1fr; gap: 10px; align-items: center; }
    .search { display:flex; align-items:center; gap:8px; background: #fff; border:1px solid #ccc; border-radius: 8px; padding: 8px 12px; }
    .search input{ width:100%; background:transparent; color:#111; border:none; outline:none; font-size:14px; }

    .filterbar { display:flex; flex-wrap:wrap; gap:8px; margin-top: 12px; }
    .chip { display:inline-flex; align-items:center; gap:8px; background: #fff; border:1px solid #ccc; color:#333; border-radius:999px; padding:6px 10px; font-size:12px; cursor:pointer; user-select:none; }
    .chip.on { background:#1a73e8; color:#fff; border-color:#1a73e8; }

    .row { display:flex; align-items:center; gap:10px; flex-wrap: wrap; margin-top: 10px; }
    select { background: #fff; color: #111; border:1px solid #ccc; border-radius: 8px; padding: 8px 12px; font-size:14px; }

    .count { margin-left:auto; color:#666; font-size:13px; }

    .year-group { margin-top: 28px; }
    .year-header { position: sticky; top: 0; background: #fff; padding: 6px 0; font-weight: 700; border-bottom: 1px solid #ccc; margin-bottom: 8px; }
    .pub { display:grid; grid-template-columns: 1fr auto; gap: 10px; padding: 14px 16px; border-radius: 8px; border:1px solid #ddd; background: #fafafa; }
    .pub + .pub { margin-top: 10px; }
    .pub-title { font-weight: 600; font-size: 16px; }
    .pub-meta { color: #555; font-size: 13px; }
    .tagline { display:flex; flex-wrap:wrap; gap:6px; margin-top: 6px; }
    .tag { background:#e8f0ff; color:#0056b3; border:1px solid #ccdfff; font-size:11px; border-radius:999px; padding: 4px 8px; }
    .actions { display:flex; align-items:center; gap:10px; }
    .btn { display:inline-flex; align-items:center; gap:8px; background: #f0f0f0; border:1px solid #ccc; color: #111; border-radius: 6px; padding: 6px 10px; font-size:12px; text-decoration:none; }
    .btn:hover { background:#e5e5e5; }

    footer { color: #666; font-size: 12px; text-align:center; margin: 36px 0 12px; }

    @media (max-width: 860px){
      .controls { grid-template-columns: 1fr; }
      .pub { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
    <div>
        <div class="title">Quantum Learning Theory Zoo</div>
        <div class="desc">
        A curated list of research papers and key references in quantum learning theory. 
        Use keyword chips (multi-select) and the year filter to narrow results.<br><br>
        <span style="font-size:0.9em; color:#555;">
            Last updated: <b>October 15, 2025</b> · Maintained by <a href="https://harris-junseo-lee.github.io" target="_blank" rel="noopener">Junseo Lee</a>. (This list may not be fully exhaustive, but efforts are made to keep it as up to date as possible.) For feedback or corrections, contact <code>harris.junseo(at)gmail.com</code>.<br><br>
        </span>
        <!-- New: collapsible About section -->
          <span style="font-size:0.9em; color:#555;">
            <details class="about">
              <summary>About this page</summary>
              <div style="margin-top:6px; font-size:0.95em; color:#333;">
                <p style="margin:6px 0;">
                  This page focuses on <b>learning and testing algorithms for understanding quantum systems</b> and does <em>not</em> cover <q>(variational) quantum machine learning models</q> (e.g., QCNNs, QGANs).
                </p>
                <p style="margin:6px 0;">
                  In the keyword classification, <em>Hamiltonian learning</em> includes certain algorithms designed for quantum many-body systems.
                </p>
                <p style="margin:6px 0;">
                  Within each year, papers are <b>sorted alphabetically by title</b>.
                </p>
                <p style="margin:6px 0;">
                  When both arXiv and published (journal or conference) versions exist, the <b>most recent publication year</b> is shown,  
                  and all paper links point to the <b>arXiv version</b>.
                </p>
              </div>
            </details>
          </span>
        </div>
    </div>
    </header>
    <div class="panel">
      <div class="controls">
        <label class="search" title="Search by title, author, venue, or free keywords">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21 21l-4.35-4.35" stroke="currentColor" stroke-width="1.6" stroke-linecap="round"/><circle cx="10.5" cy="10.5" r="6.5" stroke="currentColor" stroke-width="1.6" fill="none"/></svg>
          <input id="q" placeholder="Search by author or title keywords (e.g., “Lee”, “Bosonic Unitaries”)…" />
          <div class="count" id="resultCount">0 results</div>
        </label>
        <div class="row">
          <label for="fYear" style="font-size:13px;color:#555">Year</label>
          <select id="fYear"></select>
        </div>
      </div>
      <div class="filterbar" id="keywordBar"></div>
    </div>
    <div id="list"></div>
    <footer>
      Maintained by <a href="https://harris-junseo-lee.github.io" target="_blank" rel="noopener">Junseo Lee</a>. 
      Built for quick literature navigation in quantum learning theory.
    </footer>
  </div>

<script>
const KEYWORDS = [
  { key: 'state learning', label: 'State Learning' },
  { key: 'process learning', label: 'Process Learning' },
  { key: 'agnostic learning', label: 'Agnostic Learning' },
  { key: 'hamiltonian learning', label: 'Hamiltonian Learning' },
  { key: 'PAC learning', label: 'PAC learning' },
  { key: 'function learning', label: 'Function Learning' },
  { key: 'property testing', label: 'Property Testing' },
  { key: 'certification', label: 'Certification' },
  { key: 'continuous-variable', label: 'Continuous-Variable' },
  { key: 'fermionic', label: 'Fermionic' },
  { key: 'pseudorandomness', label: 'Pseudorandomness' },
  { key: 'survey', label: 'Survey' },
];

const PAPERS = [
  {
    title: 'Efficient learning of bosonic Gaussian unitaries',
    authors: ['Marco Fanizza', 'Vishnu Iyer', 'Junseo Lee', 'Antonio A. Mele', 'Francesco A. Mele'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.05531',
    keywords: ['process learning', 'continuous-variable'],
  },
  {
    title: 'Sample-efficient learning of interacting quantum systems',
    authors: ['Anurag Anshu', 'Srinivasan Arunachalam', 'Tomotaka Kuwahara', 'Mehdi Soleimanifar'],
    year: 2021,
    venue: 'Nature Physics',
    link: 'https://arxiv.org/abs/2004.07266',
    keywords: ['hamiltonian learning'],
  },
  {
    title: 'The learnability of quantum states',
    authors: ['Scott Aaronson'],
    year: 2007,
    venue: 'Proceedings of the Royal Society A',
    link: 'https://arxiv.org/abs/quant-ph/0608142',
    keywords: ['state learning'],
  },
  {
    title: 'Shadow tomography of quantum states',
    authors: ['Scott Aaronson'],
    year: 2018,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/1711.01053',
    keywords: ['state learning'],
  },
  {
    title: 'Online learning of quantum states',
    authors: ['Scott Aaronson', 'Xinyi Chen', 'Elad Hazan', 'Satyen Kale', 'Ashwin Nayak'],
    year: 2018,
    venue: 'NeurIPS',
    link: 'https://arxiv.org/abs/1802.09046',
    keywords: ['state learning'],
  },
  {
    title: 'Optimal algorithms for learning quantum phase states',
    authors: ['Srinivasan Arunachalam', 'Sergey Bravyi', 'Arkopal Dutt', 'Theodore J. Yoder'],
    year: 2022,
    venue: 'TQC',
    link: 'https://arxiv.org/abs/2208.07851',
    keywords: ['state learning', 'hamiltonian learning'],
  },
  {
    title: 'Two new results about quantum exact learning',
    authors: ['Srinivasan Arunachalam', 'Sourav Chakraborty', 'Troy Lee', 'Manaswi Paraashar', 'Ronald de Wolf'],
    year: 2021,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/1810.00481',
    keywords: ['function learning'],
  },
  {
    title: 'Guest column: A survey of quantum learning theory',
    authors: ['Srinivasan Arunachalam', 'Ronald de Wolf'],
    year: 2017,
    venue: 'SIGACT News',
    link: 'https://arxiv.org/abs/1701.06806',
    keywords: ['survey'],
  },
  {
    title: 'Optimal quantum sample complexity of learning algorithms',
    authors: ['Srinivasan Arunachalam', 'Ronald de Wolf'],
    year: 2018,
    venue: 'JMLR',
    link: 'https://arxiv.org/pdf/1607.00932',
    keywords: ['PAC learning', 'function learning'],
  },
  {
    title: 'Quantum learning algorithms imply circuit lower bounds',
    authors: ['Srinivasan Arunachalam', 'Alex B. Grilo', 'Tom Gur', 'Igor C. Oliveira', 'Aarthi Sundaram'],
    year: 2022,
    venue: 'FOCS',
    link: 'https://arxiv.org/pdf/2012.01920',
    keywords: ['PAC learning', 'function learning'],
  },
  {
    title: 'Quantum statistical query learning',
    authors: ['Srinivasan Arunachalam', 'Alex B. Grilo', 'Henry Yuen'],
    year: 2020,
    venue: 'arXiv:2002.08240',
    link: 'https://arxiv.org/pdf/2002.08240',
    keywords: ['PAC learning', 'function learning'],
  },
  {
    title: 'Distributed quantum inner product estimation',
    authors: ['Anurag Anshu', 'Zeph Landau', 'Yunchao Liu'],
    year: 2022,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2111.03273',
    keywords: ['property testing', 'state learning'],
  },
  {
    title: 'Private learning implies quantum stability',
    authors: ['Srinivasan Arunachalam', 'Yihui Quek', 'John A. Smolin'],
    year: 2021,
    venue: 'NeurIPS 2021',
    link: 'https://arxiv.org/abs/2102.07171',
    keywords: ['state learning']
  },
  {
    title: 'Cryptography from pseudorandom quantum states',
    authors: ['Prabhanjan Ananth', 'Luowen Qian', 'Henry Yuen'],
    year: 2022,
    venue: 'CRYPTO',
    link: 'https://arxiv.org/abs/2112.10020',
    keywords: ['pseudorandomness']
  },
  {
    title: 'Gentle measurement of quantum states and differential privacy',
    authors: ['Scott Aaronson', 'Guy N. Rothblum'],
    year: 2019,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/1904.08747',
    keywords: ['state learning']
  },
  {
    title: 'Quantum algorithms for learning and testing juntas',
    authors: ['Alp Atici', 'Rocco A. Servedio'],
    year: 2007,
    venue: 'QIP',
    link: 'https://arxiv.org/abs/0707.3479',
    keywords: ['property testing', 'function learning']
  },
  {
    title: 'Learning a local Hamiltonian from local measurements',
    authors: ['Eyal Bairey', 'Itai Arad', 'Netanel H. Lindner'],
    year: 2019,
    venue: 'PRL',
    link: 'https://arxiv.org/abs/1807.04564',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Improved quantum data analysis',
    authors: ['Costin Bădescu', 'Ryan O’Donnell'],
    year: 2021,
    venue: 'TheoretiCS',
    link: 'https://arxiv.org/abs/2011.10908',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'Efficiently learning Ising models on arbitrary graphs',
    authors: ['Guy Bresler'],
    year: 2015,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/1411.6156',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Quantum learning boolean linear functions wrt product distributions',
    authors: ['Matthias C. Caro'],
    year: 2020,
    venue: 'QIP',
    link: 'https://arxiv.org/abs/1902.08753',
    keywords: ['function learning']
  },
  {
    title: 'Learning quantum processes and Hamiltonians via the Pauli transfer matrix',
    authors: ['Matthias C. Caro'],
    year: 2022,
    venue: 'ACM Transactions on Quantum Computing',
    link: 'https://arxiv.org/abs/2212.04471',
    keywords: ['process learning', 'hamiltonian learning']
  },
  {
    title: 'Exponential separations between learning with and without quantum memory',
    authors: ['Sitan Chen', 'Jordan Cotler', 'Hsin-Yuan Huang', 'Jerry Li'],
    year: 2021,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2111.05881',
    keywords: ['state learning', 'process learning', 'property testing']
  },
  {
    title: 'When Does Adaptivity Help for Quantum State Learning?',
    authors: ['Sitan Chen', 'Brice Huang', 'Jerry Li', 'Allen Liu', 'Mark Sellke'],
    year: 2022,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2206.05265',
    keywords: ['state learning']
  },
  {
    title: 'Adaptive online learning of quantum states',
    authors: ['Xinyi Chen', 'Elad Hazan', 'Tongyang Li', 'Zhou Lu', 'Xinzhao Wang', 'Rui Yang'],
    year: 2022,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2206.00220',
    keywords: ['state learning']
  },
  {
    title: 'Sample efficient algorithms for learning quantum channels in PAC model and the approximate state discrimination problem',
    authors: ['Kai-Min Chung', 'Han-Hsuan Lin'],
    year: 2021,
    venue: 'TQC',
    link: 'https://arxiv.org/abs/1810.10938',
    keywords: ['process learning', 'PAC learning']
  },
  {
    title: 'Efficient quantum state tomography',
    authors: ['Marcus Cramer', 'Martin B. Plenio', 'Steven T. Flammia', 'Rolando Somma', 'David Gross', 'Stephen D. Bartlett', 'Olivier Landon-Cardinal', 'Yi-Kai Liu', 'David Poulin'],
    year: 2010,
    venue: 'Nature Communications',
    link: 'https://arxiv.org/abs/1101.4366',
    keywords: ['state learning']
  },
  {
    title: 'Active learning of quantum system Hamiltonians yields query advantage',
    authors: ['Arkopal Dutt', 'Edwin Pednault', 'Chai Wah Wu', 'Sarah Sheldon', 'John Smolin', 'Lev Bishop', 'Isaac L. Chuang'],
    year: 2021,
    venue: 'PRR',
    link: 'https://arxiv.org/abs/2112.14553',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Fast and robust quantum state tomography from few basis measurements',
    authors: ['Fernando G. S. L. Brandão', 'Richard Kueng', 'Daniel Stilck França'],
    year: 2021,
    venue: 'TQC',
    link: 'https://arxiv.org/abs/2009.08216',
    keywords: ['state learning']
  },
  {
    title: 'Quantum tomography via compressed sensing: error bounds, sample complexity and efficient estimators',
    authors: ['Steven T. Flammia', 'David Gross', 'Yi-Kai Liu', 'Jens Eisert'],
    year: 2012,
    venue: 'NPJ',
    link: 'https://arxiv.org/abs/1205.2300',
    keywords: ['state learning']
  },
  {
    title: 'Quantum chi-squared tomography and mutual information testing',
    authors: ['Steve Flammia', 'Ryan O’Donnell'],
    year: 2023,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2305.18519',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'Learning quantum processes without input control',
    authors: ['Marco Fanizza', 'Yihui Quek', 'Matteo Rosati'],
    year: 2024,
    venue: 'PRX Quantum',
    link: 'https://arxiv.org/abs/2211.05005',
    keywords: ['process learning']
  },
  {
    title: 'Learning distributions over quantum measurement outcomes',
    authors: ['Weiyuan Gong', 'Scott Aaronson'],
    year: 2022,
    venue: 'ICML',
    link: 'https://arxiv.org/abs/2209.03007',
    keywords: ['state learning']
  },
  {
    title: 'Efficient learning of quantum states prepared with few non-Clifford gates',
    authors: ['Sabee Grewal', 'Vishnu Iyer', 'William Kretschmer', 'Daniel Liang'],
    year: 2023,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2305.13409',
    keywords: ['state learning']
  },
  {
    title: 'Improved stabilizer estimation via Bell difference sampling',
    authors: ['Sabee Grewal', 'Vishnu Iyer', 'William Kretschmer', 'Daniel Liang'],
    year: 2024,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2304.13915',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'On the hardness of PAC-learning stabilizer states with noise',
    authors: ['Aravind Gollakota', 'Daniel Liang'],
    year: 2022,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2102.05174',
    keywords: ['state learning', 'PAC learning']
  },
  {
    title: 'Learning quantum systems',
    authors: ['Valentin Gebhart', 'Raffaele Santagati', 'Antonio Andrea Gentile', 'Erik M. Gauger', 'David Craig', 'Natalia Ares', 'Leonardo Banchi', 'Florian Marquardt', 'Luca Pezzè', 'Cristian Bonato'],
    year: 2023,
    venue: 'Nature Reviews Physics, February 2023',
    link: 'https://arxiv.org/abs/2207.00298',
    keywords: ['state learning', 'process learning', 'survey']
  },
  {
    title: 'Learning to predict arbitrary quantum processes',
    authors: ['Hsin-Yuan Huang', 'Sitan Chen', 'John Preskill'],
    year: 2022,
    venue: 'PRX Quantum',
    link: 'https://arxiv.org/abs/2210.14894',
    keywords: ['process learning']
  },
  {
    title: 'Sample-optimal tomography of quantum states',
    authors: ['Jeongwan Haah', 'Aram W. Harrow', 'Zhengfeng Ji', 'Xiaodi Wu', 'Nengkun Yu'],
    year: 2016,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/1508.01797',
    keywords: ['state learning']
  },
  {
    title: 'Learnability of the output distributions of local quantum circuits',
    authors: ['Marcel Hinsche', 'Marios Ioannou', 'Alexander Nietner', 'Jonas Haferkamp', 'Yihui Quek', 'Dominik Hangleiter', 'Jean-Pierre Seifert', 'Jens Eisert', 'Ryan Sweke'],
    year: 2021,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2110.05517',
    keywords: ['process learning', 'function learning', 'PAC learning']
  },
  {
    title: 'A single T-gate makes distribution learning hard',
    authors: ['Marcel Hinsche', 'Marios Ioannou', 'Alexander Nietner', 'Jonas Haferkamp', 'Yihui Quek', 'Dominik Hangleiter', 'Jean-Pierre Seifert', 'Jens Eisert', 'Ryan Sweke'],
    year: 2022,
    venue: 'PRL',
    link: 'https://arxiv.org/abs/2207.03140',
    keywords: ['process learning', 'function learning']
  },
  {
    title: 'Query-optimal estimation of unitary channels in diamond distance',
    authors: ['Jeongwan Haah', 'Robin Kothari', 'Ryan O’Donnell', 'Ewin Tang'],
    year: 2023,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2302.14066',
    keywords: ['process learning']
  },
  {
    title: 'Predicting many properties of a quantum system from very few measurements',
    authors: ['Hsin-Yuan Huang', 'Richard Kueng', 'John Preskill'],
    year: 2020,
    venue: 'Nature Physics',
    link: 'https://arxiv.org/abs/2002.08953',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'Optimal learning of quantum Hamiltonians from high-temperature Gibbs states',
    authors: ['Jeongwan Haah', 'Robin Kothari', 'Ewin Tang'],
    year: 2022,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2108.04842',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Provably efficient machine learning for quantum many-body problems',
    authors: ['Hsin-Yuan Huang', 'Richard Kueng', 'Giacomo Torlai', 'Victor V. Albert', 'John Preskill'],
    year: 2022,
    venue: 'Science',
    link: 'https://arxiv.org/abs/2106.12627',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Sequential measurements, disturbance and property testing',
    authors: ['Aram W. Harrow', 'Cedric Yen-Yu Lin', 'Ashley Montanaro'],
    year: 2017,
    venue: 'SODA',
    link: 'https://arxiv.org/abs/1607.03236',
    keywords: ['property testing']
  },
  {
    title: 'Learning many-body Hamiltonians with Heisenberg-limited scaling',
    authors: ['Hsin-Yuan Huang', 'Yu Tong', 'Di Fang', 'Yuan Su'],
    year: 2023,
    venue: 'PRL',
    link: 'https://arxiv.org/abs/2210.03030',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Hamiltonian simulation with optimal sample complexity',
    authors: ['Shelby Kimmel', 'Cedric Yen-Yu Lin', 'Guang Hao Low', 'Maris Ozols', 'Theodore J. Yoder'],
    year: 2017,
    venue: 'npj Quantum Information',
    link: 'https://arxiv.org/abs/1608.00281',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Fast and efficient exact synthesis of single qubit unitaries generated by Clifford and T gates',
    authors: ['Vadym Kliuchnikov', 'Dmitri Maslov', 'Michele Mosca'],
    year: 2013,
    venue: 'QIC',
    link: 'https://arxiv.org/abs/1206.5236',
    keywords: ['process learning']
  },
  {
    title: 'Learning DNFs under product distributions via μ-biased quantum Fourier sampling',
    authors: ['Varun Kanade', 'Andrea Rocchetto', 'Simone Severini'],
    year: 2019,
    venue: 'QIC',
    link: 'https://arxiv.org/abs/1802.05690',
    keywords: ['function learning']
  },
  {
    title: 'Entanglement Hamiltonian tomography in quantum simulation',
    authors: ['Christian Kokail', 'Rick van Bijnen', 'Andreas Elben', 'Benoît Vermersch', 'Peter Zoller'],
    year: 2021,
    venue: 'Nature Physics',
    link: 'https://arxiv.org/abs/2009.09000',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Learning quantum circuits of some T gates',
    authors: ['Ching-Yi Lai', 'Hao-Chung Cheng'],
    year: 2022,
    venue: 'IEEE Transactions on Information Theory',
    link: 'https://arxiv.org/abs/2106.12524',
    keywords: ['process learning']
  },
  {
    title: 'Efficient direct tomography for matrix product states',
    authors: ['Olivier Landon-Cardinal', 'Yi-Kai Liu', 'David Poulin'],
    year: 2010,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/1002.4632',
    keywords: ['state learning']
  },
  {
    title: 'Improved machine learning algorithm for predicting ground state properties',
    authors: ['Laura Lewis', 'Hsin-Yuan Huang', 'Viet T. Tran', 'Sebastian Lehner', 'Richard Kueng', 'John Preskill'],
    year: 2023,
    venue: 'Nature Communications',
    link: 'https://arxiv.org/abs/2301.13169',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Clifford circuits can be properly PAC learned if and only if RP = NP',
    authors: ['Daniel Liang'],
    year: 2022,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2204.06638',
    keywords: ['process learning', 'PAC learning']
  },
  {
    title: 'Lower bounds for learning quantum states with single-copy measurements',
    authors: ['Angus Lowe', 'Ashwin Nayak'],
    year: 2025,
    venue: 'ACM Transactions on Computation Theory',
    link: 'https://arxiv.org/abs/2207.14438',
    keywords: ['state learning', 'lower bounds']
  },
  {
    title: 'Learning and testing algorithms for the Clifford group',
    authors: ['Richard A. Low'],
    year: 2009,
    venue: 'PRA',
    link: 'https://arxiv.org/abs/0907.2833',
    keywords: ['property testing']
  },
  {
    title: 'Memory-sample lower bounds for learning with classical-quantum hybrid memory',
    authors: ['Qipeng Liu', 'Ran Raz', 'Wei Zhan'],
    year: 2023,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2303.00209',
    keywords: ['function learning', 'property testing']
  },
  {
    title: 'A polynomial time algorithm for the ground state of one-dimensional gapped local Hamiltonians',
    authors: ['Zeph Landau', 'Umesh Vazirani', 'Thomas Vidick'],
    year: 2015,
    venue: 'Nature Physics',
    link: 'https://arxiv.org/abs/1307.5143',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Learning stabilizer states by Bell sampling',
    authors: ['Ashley Montanaro'],
    year: 2017,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/1707.04012',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'Quantum circuits and low-degree polynomials over F_2',
    authors: ['Ashley Montanaro'],
    year: 2017,
    venue: 'JPA',
    link: 'https://arxiv.org/abs/1607.08473',
    keywords: ['process learning']
  },
  {
    title: 'On the average-case complexity of learning output distributions of quantum circuits',
    authors: ['Alexander Nietner', 'Marios Ioannou', 'Ryan Sweke', 'Richard Kueng', 'Jens Eisert', 'Marcel Hinsche', 'Jonas Haferkamp'],
    year: 2025,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2305.05765',
    keywords: ['process learning', 'function learning']
  }, 
  {
    title: 'Efficient learning of ground & thermal states within phases of matter',
    authors: ['Emilio Onorati', 'Cambyse Rouzé', 'Daniel Stilck França', 'James D. Watson'],
    year: 2023,
    venue: 'Nature Communications',
    link: 'https://arxiv.org/abs/2301.12946',
    keywords: ['state learning', 'hamiltonian learning']
  },
  {
    title: 'Quantum spectrum testing',
    authors: ['Ryan O’Donnell', 'John Wright'],
    year: 2015,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/1501.05028',
    keywords: ['property testing']
  },
  {
    title: 'Efficient quantum tomography',
    authors: ['Ryan O’Donnell', 'John Wright'],
    year: 2016,
    venue: 'Proceedings of the 48th Annual ACM Symposium on Theory of Computing (STOC 2016), pp. 899–912',
    link: 'https://doi.org/10.1145/2897518.2897646',
    keywords: ['state learning', 'tomography']
  },
  {
    title: 'Efficient quantum tomography II',
    authors: ['Ryan O’Donnell', 'John Wright'],
    year: 2017,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/1508.01907',
    keywords: ['state learning']
  },
  {
    title: 'Determining a local Hamiltonian from a single eigenstate',
    authors: ['Xiao-Liang Qi', 'Daniel Ranard'],
    year: 2019,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/1712.01850',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Fast learning requires good memory: A time-space lower bound for parity learning',
    authors: ['Ran Raz'],
    year: 2019,
    venue: 'Journal of the ACM',
    link: 'https://arxiv.org/abs/1602.05161',
    keywords: ['function learning']
  },
  {
    title: 'Learning quantum many-body systems from a few copies',
    authors: ['Cambyse Rouzé', 'Daniel Stilck França'],
    year: 2024,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2107.03333',
    keywords: ['hamiltonian learning', 'state learning']
  },
  {
    title: 'Stabiliser states are efficiently PAC-learnable',
    authors: ['Andrea Rocchetto'],
    year: 2018,
    venue: 'QIC',
    link: 'https://arxiv.org/abs/1705.00345',
    keywords: ['state learning', 'PAC learning']
  },
  {
    title: 'Quantifying hole-motion-induced frustration in doped antiferromagnets by Hamiltonian reconstruction',
    authors: ['Henning Schlomer', 'Timon Hilker', 'Immanuel Bloch', 'Ulrich Schollwöck', 'Fabian Grusdt', 'Annabelle Bohrdt'],
    year: 2023,
    venue: 'Communications Materials ',
    link: 'https://arxiv.org/abs/2210.02440',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Interaction screening: Efficient and sample-optimal learning of Ising models',
    authors: ['Marc Vuffray', 'Sidhant Misra', 'Andrey Lokhov', 'Michael Chertkov'],
    year: 2016,
    venue: 'NeurIPS',
    link: 'https://arxiv.org/abs/1605.07252',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Hamiltonian learning and certification using quantum resources',
    authors: ['Nathan Wiebe', 'Christopher Granade', 'Christopher Ferrie', 'David G. Cory'],
    year: 2014,
    venue: 'PRL',
    link: 'https://arxiv.org/abs/1309.0876',
    keywords: ['hamiltonian learning', 'certification']
  },
  {
    title: 'An Improved Sample Complexity Lower Bound for (Fidelity) Quantum State Tomography',
    authors: ['Henry Yuen'],
    year: 2023,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2206.11185',
    keywords: ['state learning']
  },
  {
    title: 'A survey on the complexity of learning quantum states',
    authors: ['Anurag Anshu', 'Srinivasan Arunachalam'],
    year: 2024,
    venue: 'Nature Review Physics',
    link: 'https://arxiv.org/abs/2305.20069',
    keywords: ['state learning', 'hamiltonian learning', 'survey']
  },
  {
    title: 'On the Role of Entanglement and Statistics in Learning',
    authors: ['Srinivasan Arunachalam', 'Vojtech Havlicek', 'Louis Schatzki'],
    year: 2023,
    venue: 'NeurIPS',
    link: 'https://arxiv.org/abs/2306.03161',
    keywords: ['function learning']
  },
  {
    title: 'Neural network state estimation for full quantum state tomography',
    authors: ['Qian Xu', 'Shuqi Xu'],
    year: 2018,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/1811.06654',
    keywords: ['state learning']
  },
  {
    title: 'Information-Computation Gaps in Quantum Learning via Low-Degree Likelihood',
    authors: ['Sitan Chen', 'Weiyuan Gong', 'Jonas Haferkamp', 'Yihui Quek'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2505.22743',
    keywords: ['state learning', 'process learning']
  },
  {
    title: 'Predicting quantum channels over general product distributions',
    authors: ['Sitan Chen', 'Jaume de Dios Pont', 'Jun-Ting Hsieh', 'Hsin-Yuan Huang', 'Jane Lange', 'Jerry Li'],
    year: 2025,
    venue: 'COLT',
    link: 'https://arxiv.org/abs/2409.03684',
    keywords: ['process learning']
  },
  {
    title: 'Stabilizer bootstrapping: A recipe for efficient agnostic tomography and magic estimation',
    authors: ['Sitan Chen', 'Weiyuan Gong', 'Qi Ye', 'Zhihan Zhang'],
    year: 2025,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2408.06967',
    keywords: ['state learning', 'agnostic learning']
  },
  {
    title: 'Optimal high-precision shadow estimation',
    authors: ['Sitan Chen', 'Jerry Li', 'Allen Liu'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2407.13874',
    keywords: ['state learning']
  },
  {
    title: 'Efficient Pauli channel estimation with logarithmic quantum memory',
    authors: ['Sitan Chen', 'Weiyuan Gong'],
    year: 2025,
    venue: 'PRX Quantum',
    link: 'https://arxiv.org/abs/2309.14326',
    keywords: ['process learning']
  },
  {
    title: 'Optimal tradeoffs for estimating Pauli observables',
    authors: ['Sitan Chen', 'Weiyuan Gong', 'Qi Ye'],
    year: 2024,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2404.19105',
    keywords: ['process learning']
  },
  {
    title: 'An optimal tradeoff between entanglement and copy complexity for state tomography',
    authors: ['Sitan Chen', 'Jerry Li', 'Allen Liu'],
    year: 2024,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2402.16353',
    keywords: ['state learning']
  },
  {
    title: 'Tight Bounds for Quantum State Certification with Incoherent Measurements',
    authors: ['Sitan Chen', 'Jerry Li', 'Allen Liu'],
    year: 2022,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2204.07155',
    keywords: ['certification']
  },
  {
    title: 'Quantum advantage in learning from experiments',
    authors: ['Hsin-Yuan Huang', 'Michael Broughton', 'Jordan Cotler', 'Sitan Chen', 'Jerry Li', 'Masoud Mohseni', 'Hartmut Neven', 'Ryan Babbush', 'Richard Kueng', 'John Preskill', 'Jarrod R. McClean'],
    year: 2022,
    venue: 'Science',
    link: 'https://arxiv.org/abs/2112.00778',
    keywords: ['state learning', 'process learning']
  },
  {
    title: 'A Hierarchy for Replica Quantum Advantage',
    authors: ['Sitan Chen', 'Jordan Cotler', 'Hsin-Yuan Huang', 'Jerry Li'],
    year: 2021,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2111.05874',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'Instance-Optimal Quantum State Certification with Entangled Measurements',
    authors: ['Ryan O’Donnell', 'Chirag Wadhwa'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2507.06010',
    keywords: ['certification']
  },
  {
    title: 'Toward Instance-Optimal State Certification With Incoherent Measurements',
    authors: ['Sitan Chen', 'Jerry Li', 'Ryan O’Donnell'],
    year: 2022,
    venue: 'COLT',
    link: 'https://arxiv.org/abs/2102.13098',
    keywords: ['certification']
  },
  {
    title: 'Entanglement is Necessary for Optimal Quantum Property Testing',
    authors: ['Sebastien Bubeck', 'Sitan Chen', 'Jerry Li'],
    year: 2020,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2004.07869',
    keywords: ['property testing']
  },
  {
    title: 'Learning Quantum Processes with Quantum Statistical Queries',
    authors: ['Chirag Wadhwa', 'Mina Doosti'],
    year: 2025,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2310.02075',
    keywords: ['process learning']
  },
  {
    title: 'Agnostic Process Tomography',
    authors: ['Chirag Wadhwa', 'Laura Lewis', 'Elham Kashefi', 'Mina Doosti'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2410.11957',
    keywords: ['process learning', 'agnostic learning']
  },
  {
    title: 'Mildly-Interacting Fermionic Unitaries are Efficiently Learnable',
    authors: ['Vishnu Iyer'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2504.11318',
    keywords: ['process learning', 'fermionic']
  },
  {
    title: 'Agnostic Tomography of Stabilizer Product States',
    authors: ['Sabee Grewal', 'Vishnu Iyer', 'William Kretschmer', 'Daniel Liang'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2404.03813',
    keywords: ['state learning', 'agnostic learning']
  },
  {
    title: 'Beating full state tomography for unentangled spectrum estimation',
    authors: ['Angelos Pelecanos', 'Xinyu Tan', 'Ewin Tang', 'John Wright'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2504.02785',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'Quantum state certification',
    authors: ['Costin Bădescu', 'Ryan O’Donnell', 'John Wright'],
    year: 2019,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/1708.06002',
    keywords: ['certification']
  },
  {
    title: 'Quantum learning advantage on a scalable photonic platform',
    authors: ['Zheng-Hao Liu', 'Romain Brunel', 'Emil E. B. Østergaard', 'Oscar Cordero', 'Senrui Chen', 'Yat Wong', 'Jens A. H. Nielsen', 'Axel B. Bregnsbo', 'Sisi Zhou', 'Hsin-Yuan Huang', 'Changhun Oh', 'Liang Jiang', 'John Preskill', 'Jonas S. Neergaard-Nielsen', 'Ulrik L. Andersen'],
    year: 2025,
    venue: 'Science',
    link: 'https://arxiv.org/abs/2502.07770',
    keywords: ['process learning', 'continuous-variable']
  },
  {
    title: 'Certifying almost all quantum states with few single-qubit measurements',
    authors: ['Hsin-Yuan Huang', 'John Preskill', 'Mehdi Soleimanifar'],
    year: 2025,
    venue: 'Nature Physics',
    link: 'https://arxiv.org/abs/2404.07281',
    keywords: ['certification']
  },
  {
    title: 'Unitary designs in nearly optimal depth',
    authors: ['Laura Cui', 'Thomas Schuster', 'Fernando Brandao', 'Hsin-Yuan Huang'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2507.06216',
    keywords: ['pseudorandomness']
  },
  {
    title: 'Random unitaries in extremely low depth',
    authors: ['Thomas Schuster', 'Jonas Haferkamp', 'Hsin-Yuan Huang'],
    year: 2025,
    venue: 'Science',
    link: 'https://arxiv.org/abs/2407.07754',
    keywords: ['pseudorandomness']
  },
  {
    title: 'Learning shallow quantum circuits with many-qubit gates',
    authors: ['Francisca Vasconcelos', 'Hsin-Yuan Huang'],
    year: 2025,
    venue: 'COLT',
    link: 'https://arxiv.org/abs/2410.16693',
    keywords: ['process learning']
  },
  {
    title: 'Entanglement-enabled advantage for learning a bosonic random displacement channel',
    authors: ['Changhun Oh', 'Senrui Chen', 'Yat Wong', 'Sisi Zhou', 'Hsin-Yuan Huang', 'Jens A.H. Nielsen', 'Zheng-Hao Liu', 'Jonas S. Neergaard-Nielsen', 'Ulrik L. Andersen', 'Liang Jiang', 'John Preskill'],
    year: 2024,
    venue: 'PRL',
    link: 'https://arxiv.org/abs/2402.18809',
    keywords: ['process learning', 'continuous-variable']
  },
  {
    title: 'Tight bounds on Pauli channel learning without entanglement',
    authors: ['Senrui Chen', 'Changhun Oh', 'Sisi Zhou', 'Hsin-Yuan Huang', 'Liang Jiang'],
    year: 2024,
    venue: 'PRL',
    link: 'https://arxiv.org/abs/2309.13461',
    keywords: ['process learning']
  },
  {
    title: 'Learning shallow quantum circuits',
    authors: ['Hsin-Yuan Huang', 'Yunchao Liu', 'Michael Broughton', 'Isaac Kim', 'Anurag Anshu', 'Zeph Landau', 'Jarrod R. McClean'],
    year: 2024,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2401.10095',
    keywords: ['process learning']
  },
  {
    title: 'Learning quantum states and unitaries of bounded gate complexity',
    authors: ['Haimeng Zhao', 'Laura Lewis', 'Ishaan Kannan', 'Yihui Quek', 'Hsin-Yuan Huang', 'Matthias C. Caro'],
    year: 2024,
    venue: 'PRX Quantum',
    link: 'https://arxiv.org/abs/2310.19882',
    keywords: ['state learning', 'process learning']
  },
  {
    title: 'Exponential Separations between Quantum Learning with and without Purification',
    authors: ['Zhenhuan Liu', 'Weiyuan Gong', 'Zhenyu Du', 'Zhenyu Cai'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2410.17718',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'On the sample complexity of purity and inner product estimation',
    authors: ['Weiyuan Gong', 'Jonas Haferkamp', 'Qi Ye', 'Zhihan Zhang'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2410.12712',
    keywords: ['property testing']
  },
  {
    title: 'Ansatz-free Hamiltonian learning with Heisenberg-limited scaling',
    authors: ['Hong-Ye Hu', 'Muzhou Ma', 'Weiyuan Gong', 'Qi Ye', 'Yu Tong', 'Steven T. Flammia', 'Susanne F. Yelin'],
    year: 2025,
    venue: 'PRX Quantum',
    link: 'https://arxiv.org/abs/2502.11900',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Adaptivity can help exponentially for shadow tomography',
    authors: ['Sitan Chen', 'Weiyuan Gong', 'Zhihan Zhang'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2412.19022',
    keywords: ['state learning']
  },
  {
    title: 'An infinite hierarchy of multi-copy quantum learning tasks',
    authors: ['Jan Nöller', 'Viet T. Tran', 'Mariami Gachechiladze', 'Richard Kueng'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.08070',
    keywords: ['state learning']
  },
  {
    title: 'Continuous Variable Hamiltonian Learning at Heisenberg Limit via Displacement-Random Unitary Transformation',
    authors: ['Xi Huang', 'Lixing Zhang', 'Di Luo'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.08419',
    keywords: ['hamiltonian learning', 'continuous-variable']
  },
  {
    title: 'Agnostic Product Mixed State Tomography via Robust Statistics',
    authors: ['Alvan Arulandu', 'Ilias Diakonikolas', 'Daniel Kane', 'Jerry Li'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.08472',
    keywords: ['state learning', 'agnostic learning']
  },
  {
    title: 'Learning and certification of local time-dependent quantum dynamics and noise',
    authors: ['Daniel Stilck França', 'Tim Möbus', 'Cambyse Rouzé', 'Albert H. Werner'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.08500',
    keywords: ['process learning', 'hamiltonian learning', 'certification']
  },
  {
    title: 'Product testing with single-copy measurements',
    authors: ['Jacob Beckey', 'Luke Coffman', 'Ariel Shlosberg', 'Louis Schatzki', 'Felix Leditzky'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.07820',
    keywords: ['property testing']
  },
  {
    title: 'Optimal lower bounds for quantum state tomography',
    authors: ['Thilo Scharnhorst', 'Jack Spilecki', 'John Wright'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://www.arxiv.org/abs/2510.07699',
    keywords: ['state learning']
  },
  {
    title: 'Random unitaries from Hamiltonian dynamics',
    authors: ['Laura Cui', 'Thomas Schuster', 'Liang Mao', 'Hsin-Yuan Huang', 'Fernando Brandao'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://www.arxiv.org/abs/2510.08434',
    keywords: ['pseudorandomness', 'hamiltonian learning']
  },
  {
    title: 'Quantum Probe Tomography',
    authors: ['Sitan Chen', 'Jordan Cotler', 'Hsin-Yuan Huang'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.08499',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Random unitaries that conserve energy',
    authors: ['Liang Mao', 'Laura Cui', 'Thomas Schuster', 'Hsin-Yuan Huang'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.08448v1',
    keywords: ['pseudorandomness']
  },
  {
    title: 'Non-iid hypothesis testing: from classical to quantum',
    authors: ['Giacomo De Palma', 'Marco Fanizza', 'Connor Mowry', 'Ryan O’Donnell'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.06147',
    keywords: ['property testing']
  },
  {
    title: 'Is it Gaussian? Testing bosonic quantum states',
    authors: ['Filippo Girardi', 'Freek Witteveen', 'Francesco Anna Mele', 'Lennart Bittel', 'Salvatore F. E. Oliviero', 'David Gross', 'Michael Walter'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.07305',
    keywords: ['property testing', 'continuous-variable']
  },
  {
    title: 'Higher moment theory and learnability of bosonic states',
    authors: ['Joseph T. Iosue', 'Yu-Xin Wang', 'Ishaun Datta', 'Soumik Ghosh', 'Changhun Oh', 'Bill Fefferman', 'Alexey V. Gorshkov'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.01610',
    keywords: ['state learning', 'continuous-variable']
  },
  {
    title: 'Query-Optimal Estimation of Unitary Channels via Pauli Dimensionality',
    authors: ['Sabee Grewal', 'Daniel Liang'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.00168',
    keywords: ['process learning', 'property testing']
  },
  {
    title: 'Exponential Advantage from One More Replica in Estimating Nonlinear Properties of Quantum States',
    authors: ['Qi Ye', 'Zhenhuan Liu', 'Dong-Ling Deng'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2509.24000',
    keywords: ['property testing']
  },
  {
    title: 'Lower Bounds for Learning Hamiltonians from Time Evolution',
    authors: ['Ziyun Chen', 'Jerry Li'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2509.20665',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Efficiently learning depth-3 circuits via quantum agnostic boosting',
    authors: ['Srinivasan Arunachalam', 'Arkopal Dutt', 'Alexandru Gheorghiu', 'Michael de Oliveira'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://www.arxiv.org/abs/2509.14461',
    keywords: ['agnostic learning', 'process learning']
  },
  {
    title: 'Nearly optimal algorithms to learn sparse quantum Hamiltonians in physically motivated distances',
    authors: ['Amira Abbas', 'Nunzia Cerrato', 'Francisco Escudero Gutiérrez', 'Dmitry Grinko', 'Francesco Anna Mele', 'Pulkit Sinha'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2509.09813',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Certifying and learning quantum Ising Hamiltonians',
    authors: ['Andreas Bluhm', 'Matthias C. Caro', 'Francisco Escudero Gutiérrez', 'Aadil Oufkir', 'Cambyse Rouzé'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2509.10239',
    keywords: ['hamiltonian learning', 'certification']
  },
  {
    title: 'Improved Hamiltonian learning and sparsity testing through Bell sampling',
    authors: ['Savar D. Sinha', 'Yu Tong'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2509.07937',
    keywords: ['hamiltonian learning', 'property testing']
  },
  {
    title: 'Energy-independent tomography of Gaussian states',
    authors: ['Lennart Bittel', 'Francesco A. Mele', 'Jens Eisert', 'Antonio A. Mele'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2508.14979',
    keywords: ['state learning', 'continuous-variable']
  },
  {
    title: 'Adversarially robust quantum state learning and testing',
    authors: ['Maryam Aliakbarpour', 'Vladimir Braverman', 'Nai-Hui Chia', 'Yuhan Liu'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2508.13959',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'Random Unitaries in Constant (Quantum) Time',
    authors: ['Ben Foxman', 'Natalie Parham', 'Francisca Vasconcelos', 'Henry Yuen'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2508.11487',
    keywords: ['pseudorandomness']
  },
  {
    title: 'Certifying Quantum States with Uniform Measurements',
    authors: ['Liang Mao', 'Yifei Wang', 'Yingfei Gu', 'Chengshu Li'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://www.arxiv.org/abs/2508.09259',
    keywords: ['certification']
  },
  {
    title: 'Pauli Measurements Are Near-Optimal for Single-Qubit Tomography',
    authors: ['Jayadev Acharya', 'Abhilash Dharmavarapu', 'Yuhan Liu',' Nengkun Yu'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2507.22001',
    keywords: ['state learning']
  },
  {
    title: 'Noise-tolerant learnability of shallow quantum circuits from statistics and the cost of quantum pseudorandomness',
    authors: ['Chirag Wadhwa', 'Mina Doosti'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2405.12085',
    keywords: ['process learning']
  },
  {
    title: 'Online Learning of Pure States is as Hard as Mixed States',
    authors: ['Maxime Meyer', 'Soumik Adhikary', 'Naixu Guo', 'Patrick Rebentrost'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2502.00823',
    keywords: ['state learning']
  },
  {
    title: 'Pauli measurements are not optimal for single-copy tomography',
    authors: ['Jayadev Acharya', 'Abhilash Dharmavarapu', 'Yuhan Liu', 'Nengkun Yu'],
    year: 2025,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2502.18170',
    keywords: ['state learning']
  },
  {
    title: 'Improved Sample Upper and Lower Bounds for Trace Estimation of Quantum State Powers',
    authors: ['Kean Chen', 'Qisheng Wang'],
    year: 2025,
    venue: 'COLT',
    link: 'https://arxiv.org/abs/2505.09563',
    keywords: ['property testing']
  },
  {
    title: 'Learning quantum states of continuous variable systems',
    authors: ['Francesco Anna Mele', 'Antonio Anna Mele', 'Lennart Bittel', 'Jens Eisert', 'Vittorio Giovannetti', 'Ludovico Lami', 'Lorenzo Leone', 'Salvatore F.E. Oliviero'],
    year: 2025,
    venue: 'Nature Physics',
    link: 'https://arxiv.org/abs/2405.01431',
    keywords: ['state learning', 'continuous-variable']
  },
  {
    title: 'Quantum Hamiltonian Certification',
    authors: ['Minbo Gao', 'Zhengfeng Ji', 'Qisheng Wang', 'Wenjun Yu', 'Qi Zhao'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2505.13217',
    keywords: ['certification', 'hamiltonian learning']
  },
  {
    title: 'Hamiltonian Locality Testing via Trotterized Postselection',
    authors: ['John Kallaugher', 'Daniel Liang'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2505.06478',
    keywords: ['property testing', 'hamiltonian learning']
  },
  {
    title: 'Efficient Learning Implies Quantum Glassiness',
    authors: ['Eric R. Anschuetz'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2505.00087',
    keywords: ['property testing', 'hamiltonian learning']
  },
  {
    title: 'Efficiently learning fermionic unitaries with few non-Gaussian gates',
    authors: ['Sharoon Austin', 'Mauro E.S. Morales', 'Alexey Gorshkov'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2504.15356',
    keywords: ['process learning', 'fermionic']
  },
  {
    title: 'Learning to erase quantum states: thermodynamic implications of quantum learning theory',
    authors: ['Haimeng Zhao', 'Yuzhen Zhang', 'John Preskill'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2504.07341',
    keywords: ['state learning']
  },
  {
    title: 'Learning quantum Gibbs states locally and efficiently',
    authors: ['Chi-Fang Chen', 'Anurag Anshu', 'Quynh T. Nguyen'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2504.02706',
    keywords: ['state learning', 'hamiltonian learning']
  },
  {
    title: 'Quantum advantage for learning shallow neural networks with natural data distributions',
    authors: ['Laura Lewis', 'Dar Gilboa', 'Jarrod R. McClean'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2503.20879',
    keywords: ['process learning']
  },
  {
    title: 'A Dobrushin condition for quantum Markov chains: Rapid mixing and conditional mutual information at high temperature',
    authors: ['Ainesh Bakshi', 'Allen Liu', 'Ankur Moitra', 'Ewin Tang'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.08542',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Learning the closest product state',
    authors: ['Ainesh Bakshi', 'John Bostanci', 'William Kretschmer', 'Zeph Landau', 'Jerry Li', 'Allen Liu', 'Ryan O’Donnell', 'Ewin Tang'],
    year: 2025,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2411.04283',
    keywords: ['state learning', 'agnostic learning']
  },
  {
    title: 'Structure learning of Hamiltonians from real-time evolution',
    authors: ['Ainesh Bakshi', 'Allen Liu', 'Ankur Moitra', 'Ewin Tang'],
    year: 2024,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2405.00082',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'High-Temperature Gibbs States are Unentangled and Efficiently Preparable',
    authors: ['Ainesh Bakshi', 'Allen Liu', 'Ankur Moitra', 'Ewin Tang'],
    year: 2024,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2403.16850',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Learning quantum Hamiltonians at any temperature in polynomial time',
    authors: ['Ainesh Bakshi', 'Allen Liu', 'Ankur Moitra', 'Ewin Tang'],
    year: 2024,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2310.02243',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Nearly tight bounds for testing tree tensor network states',
    authors: ['Benjamin Lovitz', 'Angus Lowe'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2410.21417',
    keywords: ['property testing']
  },
  {
    title: 'Efficient Hamiltonian, structure and trace distance learning of Gaussian states',
    authors: ['Marco Fanizza', 'Cambyse Rouzé', 'Daniel Stilck França'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2411.03163',
    keywords: ['state learning', 'hamiltonian learning', 'continuous-variable']
  },
  {
    title: 'A Survey of Quantum Property Testing',
    authors: ['Ashley Montanaro', 'Ronald de Wolf'],
    year: 2018,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/1310.2035',
    keywords: ['property testing', 'survey']
  },
  {
    title: 'Optimal trace-distance bounds for free-fermionic states: Testing and improved tomography',
    authors: ['Lennart Bittel', 'Antonio Anna Mele', 'Jens Eisert', 'Lorenzo Leone'],
    year: 2025,
    venue: 'PRX Quantum',
    link: 'https://arxiv.org/abs/2409.17953',
    keywords: ['state learning', 'property testing', 'fermionic']
  },
  {
    title: 'Optimal estimates of trace distance between bosonic Gaussian states and applications to learning',
    authors: ['Lennrt Bittael', 'Francesco Anna Mele', 'Antonio Anna Mele', 'Salvatore Tirone', 'Ludovico Lami'],
    year: 2025,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2411.02368',
    keywords: ['state learning', 'continuous-variable']
  },
  {
    title: 'PAC-learning of free-fermionic states is NP-hard',
    authors: ['Lennrt Bittael', 'Antonio A. Mele', 'Jens Eisert', 'Lorenzo Leone'],
    year: 2025,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2404.03585',
    keywords: ['state learning', 'fermionic']
  },
  {
    title: 'Efficient learning of quantum states prepared with few fermionic non-Gaussian gates',
    authors: ['Antonio Anna Mele', 'Yaroslav Herasymenko'],
    year: 2025,
    venue: 'PRX Quantum',
    link: 'https://arxiv.org/abs/2402.18665',
    keywords: ['state learning', 'fermionic']
  },
  {
    title: 'Resource-efficient algorithm for estimating the trace of quantum state powers',
    authors: ['Myeongjin Shin', 'Junseo Lee', 'Seungwoo Lee', 'Kabgyun Jeong'],
    year: 2025,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2408.00314',
    keywords: ['property testing']
  },
  {
    title: 'Efficient Tomography of Non-Interacting Fermion States',
    authors: ['Scott Aaronson', 'Sabee Grewal'],
    year: 2023,
    venue: 'TQC',
    link: 'https://arxiv.org/abs/2102.10458',
    keywords: ['state learning', 'fermionic']
  },
  {
    title: 'Heisenberg-limited Hamiltonian learning continuous variable systems via engineered dissipation',
    authors: ['Tim Möbus', 'Andreas Bluhm', 'Tuvia Gefen', 'Yu Tong', 'Albert H. Werner', 'Cambyse Rouzé'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2506.00606',
    keywords: ['hamiltonian learning', 'continuous-variable']
  },
  {
    title: 'Learning k-body Hamiltonians via compressed sensing',
    authors: ['Muzhou Ma', 'Steven T. Flammia', 'John Preskill', 'Yu Tong'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2410.18928',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Heisenberg-limited Hamiltonian learning for interacting bosons',
    authors: ['Haoya Li', 'Yu Tong', 'Hongkang Ni', 'Tuvia Gefen', 'Lexing Ying'],
    year: 2024,
    venue: 'npj Quantum Information',
    link: 'https://arxiv.org/abs/2307.04690',
    keywords: ['hamiltonian learning', 'continuous-variable']
  },
  {
    title: 'Learning unitaries with quantum statistical queries',
    authors: ['Armando Angrisani'],
    year: 2025,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2310.02254',
    keywords: ['process learning']
  },
  {
    title: 'Learning junta distributions, quantum junta states, and QAC0 circuits',
    authors: ['Jinge Bao', 'Francisco Escudero-Gutiérrez'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2410.15822v2',
    keywords: ['state learning', 'process learning']
  },
  {
    title: 'How to Construct Random Unitaries',
    authors: ['Fermi Ma', 'Hsin-Yuan Huang'],
    year: 2025,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2410.10116',
    keywords: ['pseudorandomness']
  },
  {
    title: 'Sample Optimal and Memory Efficient Quantum State Tomography',
    authors: ['Yanglin Hu', 'Enrique Cervero-Martín', 'Elias Theil', 'Laura Mančinska', 'Marco Tomamichel'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2410.16220',
    keywords: ['state learning']
  },
  {
    title: 'Optimal Fidelity Estimation from Binary Measurements for Discrete and Continuous Variable Systems',
    authors: ['Omar Fawzi', 'Aadil Oufkir', 'Robert Salzmann'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2409.04189',
    keywords: ['property testing', 'continuous-variable']
  },
  {
    title: 'Learning State Preparation Circuits for Quantum Phases of Matter',
    authors: ['Hyun-Soo Kim', 'Isaac H. Kim', 'Daniel Ranard'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2410.23544',
    keywords: ['process learning']
  },
  {
    title: 'Learning quantum states prepared by shallow circuits in polynomial time',
    authors: ['Zeph Landau', 'Yunchao Liu'],
    year: 2025,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2410.23618',
    keywords: ['process learning']
  },
  {
    title: 'Efficient approximate unitary designs from random Pauli rotations',
    authors: ['Jeongwan Haah', 'Yunchao Liu', 'Xinyu Tan'],
    year: 2024,
    venue: 'FOCS',
    link: 'https://arxiv.org/abs/2402.05239',
    keywords: ['pseudorandomness']
  },
  {
    title: 'The learnability of Pauli noise',
    authors: ['Senrui Chen', 'Yunchao Liu', 'Matthew Otten', 'Alireza Seif', 'Bill Fefferman', 'Liang Jiang'],
    year: 2023,
    venue: 'Nature Communications',
    link: 'https://arxiv.org/abs/2206.06362',
    keywords: ['process learning']
  },
  {
    title: 'Learning the structure of any Hamiltonian from minimal assumptions',
    authors: ['Andrew Zhao'],
    year: 2025,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2410.21635',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Fermionic partial tomography via classical shadows',
    authors: ['Andrew Zhao', 'Nicholas C. Rubin', 'Akimasa Miyake'],
    year: 2021,
    venue: 'PRL',
    link: 'https://arxiv.org/abs/2010.16094',
    keywords: ['state learning', 'fermionic']
  },
  {
    title: 'Compression of quantum shallow-circuit states',
    authors: ['Yuxiang Yang'],
    year: 2025,
    venue: 'PRL',
    link: 'https://arxiv.org/abs/2404.11177',
    keywords: ['state learning']
  },
  {
    title: 'Qudit Shadow Estimation Based on the Clifford Group and the Power of a Single Magic Gate',
    authors: ['Chengsi Mao', 'Changhao Yi', 'Huangjun Zhu'],
    year: 2025,
    venue: 'PRL',
    link: 'https://arxiv.org/abs/2410.13572',
    keywords: ['property testing']
  },
  {
    title: 'Efficient self-consistent learning of gate set Pauli noise',
    authors: ['Senrui Chen', 'Zhihan Zhang', 'Liang Jiang', 'Steven T. Flammia'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2410.03906',
    keywords: ['process learning']
  },
  {
    title: 'Quantum advantages for Pauli channel estimation',
    authors: ['Senrui Chen', 'Sisi Zhou', 'Alireza Seif', 'Liang Jiang'],
    year: 2022,
    venue: 'PRA',
    link: 'https://arxiv.org/abs/2108.08488',
    keywords: ['process learning']
  },
  {
    title: 'Robust shadow estimation',
    authors: ['Senrui Chen', 'Wenjun Yu', 'Pei Zeng', 'Steven T. Flammia'],
    year: 2021,
    venue: 'PRX Quantum',
    link: 'https://arxiv.org/abs/2011.09636',
    keywords: ['property testing', 'state learning']
  },
  {
    title: 'Entanglement-enhanced learning of quantum processes at scale',
    authors: ['Alireza Seif', 'Senrui Chen', 'Swarnadeep Majumder', 'Haoran Liao', 'Derek S. Wang', 'Moein Malekakhlagh', 'Ali Javadi-Abhari', 'Liang Jiang', 'Zlatko K. Minev'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2408.03376',
    keywords: ['process learning', 'property testing']
  },
  {
    title: 'Learning stabilizer structure of quantum states',
    authors: ['Srinivasan Arunachalam', 'Arkopal Dutt'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2510.05890',
    keywords: ['state learning', 'agnostic learning']
  },
  {
    title: 'Distributed inner product estimation with limited quantum communication',
    authors: ['Srinivasan Arunachalam', 'Louis Schatzki'],
    year: 2025,
    venue: 'STACS',
    link: 'https://arxiv.org/abs/2410.12684',
    keywords: ['property testing']
  },
  {
    title: 'Testing and learning structured Hamiltonians',
    authors: ['Srinivasan Arunachalam', 'Arkopal Dutt', 'Francisco Escudero Gutiérrez'],
    year: 2025,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2411.00082',
    keywords: ['hamiltonian learning', 'property testing']
  },
  {
    title: 'Polynomial-time tolerant testing stabilizer states',
    authors: ['Srinivasan Arunachalam', 'Arkopal Dutt'],
    year: 2025,
    venue: 'STOC',
    link: 'https://arxiv.org/abs/2408.06289',
    keywords: ['property testing']
  },
  {
    title: 'Quantum hardness of learning shallow classical circuits',
    authors: ['Srinivasan Arunachalam', 'Alex B. Grilo', 'Aarthi Sundaram'],
    year: 2021,
    venue: 'SICOMP',
    link: 'https://arxiv.org/abs/1903.02840',
    keywords: ['function learning', 'PAC learning']
  },
  {
    title: 'Quantum hardness of learning shallow classical circuits',
    authors: ['Srinivasan Arunachalam', 'Arkopal Dutt', 'Francisco Escudero Gutiérrez', 'Carlos Palazuelos'],
    year: 2024,
    venue: 'ICALP',
    link: 'https://arxiv.org/abs/2405.10933',
    keywords: ['process learning', 'function learning']
  },
  {
    title: 'Efficient tomography of a quantum many-body system',
    authors: ['B. P. Lanyon', 'C. Maier', 'M. Holzäpfel', 'T. Baumgratz', 'C. Hempel', 'P. Jurcevic', 'I. Dhand', 'A. S. Buyskikh', 'A. J. Daley', 'M. Cramer', 'M. B. Plenio', 'R. Blatt', 'C. F. Roos'],
    year: 2017,
    venue: 'Nature Physics',
    link: 'https://arxiv.org/abs/1612.08000',
    keywords: ['state learning']
  },
  {
    title: 'Learning finitely correlated states: stability of the spectral reconstruction',
    authors: ['Marco Fanizza', 'Niklas Galke', 'Josep Lumbreras', 'Cambyse Rouzé', 'Andreas Winter'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2312.07516',
    keywords: ['state learning']
  },
  {
    title: 'Learning t-doped stabilizer states',
    authors: ['Lorenzo Leone', 'Salvatore F. E. Oliviero', 'Alioscia Hamma'],
    year: 2024,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2305.15398',
    keywords: ['state learning']
  },
  {
    title: 'Learning efficient decoders for quasi-chaotic quantum scramblers',
    authors: ['Lorenzo Leone', 'Salvatore F.E. Oliviero', 'Seth Lloyd', 'Alioscia Hamma'],
    year: 2024,
    venue: 'PRA',
    link: 'https://arxiv.org/abs/2212.11338',
    keywords: ['process learning']
  },
  {
    title: 'Fast state tomography with optimal error bounds',
    authors: ['Madalin Guta', 'Jonas Kahn', 'Richard Kueng', 'Joel A. Tropp'],
    year: 2020,
    venue: 'JPA',
    link: 'https://arxiv.org/abs/1809.11162',
    keywords: ['state learning']
  },
  {
    title: 'Strong random unitaries and fast scrambling',
    authors: ['Thomas Schuster', 'Fermi Ma', 'Alex Lombardi', 'Fernando Brandao', 'Hsin-Yuan Huang'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2509.26310',
    keywords: ['pseudorandomness']
  },
  {
    title: 'Will it glue? On short-depth designs beyond the unitary group',
    authors: ['Lorenzo Grevink', 'Jonas Haferkamp', 'Markus Heinrich', 'Jonas Helsen', 'Marcel Hinsche', 'Thomas Schuster', 'Zoltán Zimborás'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://www.arxiv.org/abs/2506.23925',
    keywords: ['pseudorandomness']
  },
  {
    title: 'The advantage of quantum control in many-body Hamiltonian learning',
    authors: ['Alicja Dutkiewicz', 'Thomas E. O’Brien', 'Thomas Schuster'],
    year: 2024,
    venue: 'Quantum',
    link: 'https://arxiv.org/abs/2304.07172',
    keywords: ['hamiltonian learning']
  },
  {
    title: 'Learning quantum systems via out-of-time-order correlators',
    authors: ['Thomas Schuster', 'Murphy Niu', 'Jordan Cotler', 'Thomas E. O’Brien', 'Jarrod R. McClean', 'Masoud Mohseni'],
    year: 2023,
    venue: 'PRR',
    link: 'https://arxiv.org/abs/2208.02254',
    keywords: ['property testing', 'hamiltonian learning']
  },
  {
    title: 'Quantum Algorithmic Measurement',
    authors: ['Dorit Aharonov', 'Jordan Cotler', 'Xiao-Liang Qi'],
    year: 2022,
    venue: 'Nature Communications',
    link: 'https://arxiv.org/abs/2101.04634',
    keywords: ['property testing', 'hamiltonian learning']
  },
  {
    title: 'Hamiltonian Property Testing',
    authors: ['Andreas Bluhm', 'Matthias C. Caro', 'Aadil Oufkir'],
    year: 2024,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2403.02968',
    keywords: ['property testing', 'hamiltonian learning']
  },
  {
    title: 'Unitarity estimation for quantum channels',
    authors: ['Kean Chen', 'Qisheng Wang', 'Peixun Long',' Mingsheng Ying'],
    year: 2023,
    venue: 'IEEE Transactions on Information Theory',
    link: 'https://arxiv.org/abs/2212.09319',
    keywords: ['process learning']
  },
  {
    title: 'Quantum Channel Certification with Incoherent Strategies',
    authors: ['Omar Fawzi', 'Nicolas Flammarion', 'Aurélien Garivier', 'Aadil Oufkir'],
    year: 2023,
    venue: 'COLT',
    link: 'https://arxiv.org/abs/2303.01188',
    keywords: ['certification']
  },
  {
    title: 'Few Single-Qubit Measurements Suffice to Certify Any Quantum State',
    authors: ['Meghal Gupta', 'William He', 'Ryan O’Donnell'],
    year: 2025,
    venue: 'arXiv',
    link: 'https://arxiv.org/abs/2506.11355',
    keywords: ['certification']
  },
  {
    title: 'Low rank matrix recovery from rank one measurements',
    authors: ['Richard Kueng', 'Holger Rauhut', 'Ulrich Terstiege'],
    year: 2017,
    venue: 'Applied and Computational Harmonic Analysis',
    link: 'https://arxiv.org/abs/1410.6913',
    keywords: ['state learning']
  },
  {
    title: 'Quantum Event Learning and Gentle Random Measurements',
    authors: ['Adam Bene Watts', 'John Bostanci'],
    year: 2024,
    venue: 'ITCS',
    link: 'https://arxiv.org/abs/2210.09155',
    keywords: ['state learning', 'property testing']
  },
  {
    title: 'Testing matrix product states',
    authors: ['Mehdi Soleimanifar', 'John Wright'],
    year: 2022,
    venue: 'SODA',
    link: 'https://arxiv.org/abs/2410.21417',
    keywords: ['property testing']
  },
  {
    title: 'Lower bounds for testing complete positivity and quantum separability',
    authors: ['Costin Bădescu', 'Ryan O’Donnell'],
    year: 2020,
    venue: 'LATIN',
    link: 'https://arxiv.org/abs/1905.01542',
    keywords: ['property testing']
  },
  {
    title: 'Quantum tomography using state-preparation unitaries',
    authors: ['Joran van Apeldoorn', 'Arjan Cornelissen', 'András Gilyén', 'Giacomo Nannicini'],
    year: 2023,
    venue: 'SODA',
    link: 'https://arxiv.org/abs/2207.08800',
    keywords: ['state learning']
  },

];



const $list = document.getElementById('list');
const $q = document.getElementById('q');
const $fYear = document.getElementById('fYear');
const $bar = document.getElementById('keywordBar');
const $count = document.getElementById('resultCount');
const selectedKeywords = new Set();

function buildKeywordBar(){
  KEYWORDS.forEach(({key, label})=>{
    const chip = document.createElement('span');
    chip.className = 'chip';
    chip.textContent = label;
    chip.title = label + ' (toggle)';
    chip.addEventListener('click', ()=>{
      if (selectedKeywords.has(key)) selectedKeywords.delete(key); else selectedKeywords.add(key);
      chip.classList.toggle('on');
      render();
    });
    $bar.appendChild(chip);
  });
}

function hydrateYearOptions(){
  const years = [...new Set(PAPERS.map(p=>p.year))].sort((a,b)=>b-a);
  const all = document.createElement('option'); all.value=''; all.textContent='All years'; $fYear.appendChild(all);
  years.forEach(y=>{ const o=document.createElement('option'); o.value=String(y); o.textContent=String(y); $fYear.appendChild(o); });
}

function matchQuery(p, q){
  if (!q) return true;
  const hay = [p.title, p.venue, p.authors.join(' '), (p.tags||[]).join(' '), (p.note||''), (p.keywords||[]).join(' ')].join(' ').toLowerCase();
  return q.split(/\s+/).every(tok => hay.includes(tok));
}

function matchKeywords(p){
  if (selectedKeywords.size === 0) return true;
  const ks = new Set(p.keywords||[]);
  for (const k of selectedKeywords){ if (!ks.has(k)) return false; }
  return true;
}

function groupByYear(items){
  const map = new Map();
  for (const it of items){
    if (!map.has(it.year)) map.set(it.year, []);
    map.get(it.year).push(it);
  }

  for (const [year, list] of map.entries()){
    list.sort((a, b) => a.title.localeCompare(b.title));
  }

  return [...map.entries()].sort((a,b)=>b[0]-a[0]);
}


function render(){
  const q = ($q.value||'').trim().toLowerCase();
  const y = $fYear.value;

  const filtered = PAPERS.filter(p => matchQuery(p, q) && matchKeywords(p) && (!y || String(p.year) === y));

  $count.textContent = `${filtered.length} result${filtered.length===1?'':'s'}`;
  $list.innerHTML = '';
  const grouped = groupByYear(filtered);
  if (grouped.length === 0){
    $list.innerHTML = '<p style="color:#666">No results. Try removing a keyword or clearing the search box.</p>';
    return;
  }
  for (const [year, items] of grouped){
    const g = document.createElement('section'); g.className='year-group';
    const h = document.createElement('div'); h.className='year-header'; h.textContent = year; g.appendChild(h);
    for (const p of items){ g.appendChild(renderPub(p)); }
    $list.appendChild(g);
  }
}

function renderPub(p){
  const el = document.createElement('article'); el.className='pub';
  const left = document.createElement('div');
  const right = document.createElement('div'); right.className='actions';
  left.innerHTML = `
    <div class="pub-title"><a href="${p.link||'#'}" target="_blank" rel="noopener">${p.title}</a></div>
    <div class="pub-meta">${p.authors.join(', ')} · ${p.venue || ''}</div>
    ${p.note ? `<div class="pub-meta" style="margin-top:4px">${p.note}</div>` : ''}
    <div class="tagline">${(p.keywords||[]).map(t=>`<span class='tag'>${t}</span>`).join('')} ${(p.tags||[]).map(t=>`<span class='tag'>${t}</span>`).join('')}</div>
  `;
  if (p.link){
    const btn = document.createElement('a'); btn.className='btn'; btn.href=p.link; btn.target='_blank'; btn.rel='noopener'; btn.textContent='arXiv'; right.appendChild(btn);
  }
  el.appendChild(left); el.appendChild(right);
  return el;
}

$q.addEventListener('input', render);
$fYear.addEventListener('input', render);
buildKeywordBar();
hydrateYearOptions();
render();

</script>
</body>
</html>