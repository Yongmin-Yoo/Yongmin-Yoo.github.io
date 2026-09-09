---
permalink: /
title: "👨‍🎓About Me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
  /* =========================================================
     Page-wide design
     ========================================================= */

  .profile-page {
    --page-text: #303640;
    --page-muted: #6b7280;
    --page-border: #e4e7eb;
    --page-soft-border: #eef0f2;
    --page-background: #ffffff;
    --page-soft-background: #f8f9fa;
    --page-accent: #3f5268;
    --page-accent-dark: #303d4d;
    --page-gold: #c59628;
    --page-gold-background: #fff9e9;

    color: var(--page-text);
  }

  .profile-page a {
    transition:
      color 0.2s ease,
      background-color 0.2s ease,
      border-color 0.2s ease,
      transform 0.2s ease;
  }

  .profile-intro {
    margin-bottom: 2.8rem;
    line-height: 1.78;
  }

  .profile-intro p {
    margin-bottom: 1.15rem;
  }

  .profile-intro p:last-child {
    margin-bottom: 0;
  }

  .profile-intro a {
    color: #41678b;
    font-weight: 500;
    text-decoration: none;
    border-bottom: 1px solid rgba(65, 103, 139, 0.35);
  }

  .profile-intro a:hover {
    color: #243b55;
    border-bottom-color: #243b55;
  }

  .section-title {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    margin-top: 3rem;
    margin-bottom: 1.3rem;
    padding-bottom: 0.6rem;
    border-bottom: 1px solid var(--page-border);
  }


  /* =========================================================
     Research interests
     ========================================================= */

  .research-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 0.9rem;
    margin-bottom: 2.5rem;
  }

  .research-card {
    position: relative;
    padding: 1.15rem 1.1rem;
    overflow: hidden;
    border: 1px solid var(--page-border);
    border-radius: 8px;
    background-color: var(--page-background);
    box-shadow: 0 2px 8px rgba(31, 41, 55, 0.035);
    transition:
      transform 0.2s ease,
      border-color 0.2s ease,
      box-shadow 0.2s ease;
  }

  .research-card:hover {
    transform: translateY(-2px);
    border-color: #c9ced5;
    box-shadow: 0 6px 16px rgba(31, 41, 55, 0.07);
  }

  .research-number {
    display: inline-block;
    margin-bottom: 0.55rem;
    color: var(--page-gold);
    font-size: 0.75em;
    font-weight: 800;
    letter-spacing: 0.08em;
  }

  .research-card h3 {
    margin: 0 0 0.55rem;
    color: var(--page-text);
    font-size: 0.98em;
    line-height: 1.4;
  }

  .research-card p {
    margin: 0;
    color: var(--page-muted);
    font-size: 0.86em;
    line-height: 1.65;
  }


  /* =========================================================
     News timeline
     ========================================================= */

  .news-list {
    position: relative;
    margin: 0 0 2.5rem;
  }

  .news-item {
    display: grid;
    grid-template-columns: 95px minmax(0, 1fr);
    gap: 1rem;
    padding: 1.25rem 0;
    border-bottom: 1px solid var(--page-soft-border);
  }

  .news-item:first-child {
    padding-top: 0.2rem;
  }

  .news-item:last-child {
    border-bottom: none;
  }

  .news-date {
    padding-top: 0.08rem;
    color: var(--page-muted);
    font-size: 0.82em;
    font-weight: 750;
    letter-spacing: 0.015em;
    white-space: nowrap;
  }

  .news-content {
    min-width: 0;
    line-height: 1.65;
  }

  .news-summary {
    color: var(--page-text);
  }

  .news-venue {
    color: #41678b !important;
    font-weight: 650;
    text-decoration: none !important;
    border-bottom: 1px solid rgba(65, 103, 139, 0.35);
  }

  .news-venue:hover {
    color: #243b55 !important;
    border-bottom-color: #243b55;
  }

  .news-paper-title {
    margin-top: 0.65rem;
    color: #404650;
    font-size: 0.94em;
    line-height: 1.55;
  }

  .author-role {
    display: inline-flex;
    align-items: center;
    margin-top: 0.55rem;
    padding: 0.25rem 0.65rem;
    color: #74570d;
    background-color: var(--page-gold-background);
    border: 1px solid rgba(197, 150, 40, 0.35);
    border-radius: 999px;
    font-size: 0.77em;
    font-weight: 650;
    line-height: 1.35;
  }

  .paper-button {
    display: inline-flex;
    align-items: center;
    gap: 0.3rem;
    margin-top: 0.7rem;
    padding: 0.32rem 0.75rem;
    color: #3f4652 !important;
    background-color: transparent;
    border: 1px solid #aeb4bd;
    border-radius: 999px;
    font-size: 0.77em;
    font-weight: 650;
    line-height: 1.2;
    text-decoration: none !important;
  }

  .paper-button:hover {
    color: #ffffff !important;
    background-color: #3f4652;
    border-color: #3f4652;
    text-decoration: none !important;
    transform: translateY(-1px);
  }

  .paper-button:focus {
    outline: 2px solid #6f89a8;
    outline-offset: 2px;
  }

  .external-arrow {
    font-size: 0.95em;
    transition: transform 0.2s ease;
  }

  .paper-button:hover .external-arrow {
    transform: translate(1px, -1px);
  }


  /* =========================================================
     Service
     ========================================================= */

  .service-group {
    margin: 1.5rem 0 2.2rem;
  }

  .service-heading {
    margin: 0 0 0.55rem;
    padding-bottom: 0.5rem;
    color: var(--page-text);
    border-bottom: 1px solid var(--page-border);
    font-size: 1.02em;
    font-weight: 750;
  }

  .service-row {
    display: grid;
    grid-template-columns: 95px minmax(0, 1fr);
    gap: 1rem;
    align-items: start;
    padding: 0.9rem 0;
    border-bottom: 1px solid var(--page-soft-border);
  }

  .service-row:last-child {
    border-bottom: none;
  }

  .service-row.highlighted-service {
    margin-top: 0.85rem;
    padding: 1rem 1.05rem;
    border: 1px solid var(--page-border);
    border-left: 4px solid var(--page-gold);
    border-radius: 7px;
    background: linear-gradient(
      90deg,
      rgba(255, 249, 233, 0.85),
      rgba(255, 255, 255, 0.5)
    );
    box-shadow: 0 2px 8px rgba(31, 41, 55, 0.035);
  }

  .service-date {
    padding-top: 0.08rem;
    color: var(--page-muted);
    font-size: 0.82em;
    font-weight: 750;
    letter-spacing: 0.015em;
    white-space: nowrap;
  }

  .service-content {
    min-width: 0;
    line-height: 1.6;
  }

  .service-role {
    color: var(--page-text);
    font-weight: 750;
  }

  .service-event {
    color: #41678b !important;
    font-weight: 650;
    text-decoration: none !important;
    border-bottom: 1px solid rgba(65, 103, 139, 0.35);
  }

  .service-event:hover {
    color: #243b55 !important;
    border-bottom-color: #243b55;
  }

  .service-description {
    margin-top: 0.25rem;
    color: var(--page-muted);
    font-size: 0.85em;
  }

  .service-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
  }

  .service-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.27rem 0.68rem;
    color: #434a55 !important;
    background-color: var(--page-soft-background);
    border: 1px solid #dfe2e6;
    border-radius: 999px;
    font-size: 0.78em;
    font-weight: 650;
    line-height: 1.3;
    text-decoration: none !important;
  }

  .service-tag:hover {
    color: #ffffff !important;
    background-color: #3f4652;
    border-color: #3f4652;
    text-decoration: none !important;
    transform: translateY(-1px);
  }


  /* =========================================================
     Responsive design
     ========================================================= */

  @media (max-width: 900px) {
    .research-grid {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 600px) {
    .section-title {
      margin-top: 2.5rem;
    }

    .news-item,
    .service-row {
      grid-template-columns: 1fr;
      gap: 0.4rem;
    }

    .news-date,
    .service-date {
      padding-top: 0;
    }

    .service-row.highlighted-service {
      gap: 0.45rem;
    }
  }


  /* =========================================================
     Dark mode
     ========================================================= */

  @media (prefers-color-scheme: dark) {
    .profile-page {
      --page-text: #eeeeee;
      --page-muted: #b3b7bd;
      --page-border: #444951;
      --page-soft-border: #343940;
      --page-background: rgba(255, 255, 255, 0.025);
      --page-soft-background: rgba(255, 255, 255, 0.05);
      --page-gold-background: rgba(197, 150, 40, 0.12);
    }

    .profile-intro a,
    .news-venue,
    .service-event {
      color: #9ab6d2 !important;
      border-bottom-color: rgba(154, 182, 210, 0.45);
    }

    .profile-intro a:hover,
    .news-venue:hover,
    .service-event:hover {
      color: #c5d8e9 !important;
      border-bottom-color: #c5d8e9;
    }

    .research-card {
      background-color: var(--page-background);
      box-shadow: none;
    }

    .research-card:hover {
      border-color: #626871;
      box-shadow: none;
    }

    .research-card h3,
    .news-summary,
    .news-paper-title,
    .service-heading,
    .service-role {
      color: var(--page-text);
    }

    .author-role {
      color: #e1c36d;
      background-color: var(--page-gold-background);
      border-color: rgba(197, 150, 40, 0.38);
    }

    .paper-button {
      color: #dddddd !important;
      background-color: transparent;
      border-color: #737983;
    }

    .paper-button:hover {
      color: #222222 !important;
      background-color: #dddddd;
      border-color: #dddddd;
    }

    .service-row.highlighted-service {
      background: linear-gradient(
        90deg,
        rgba(197, 150, 40, 0.1),
        rgba(255, 255, 255, 0.015)
      );
      border-color: #474c54;
      border-left-color: var(--page-gold);
      box-shadow: none;
    }

    .service-tag {
      color: #dddddd !important;
      background-color: var(--page-soft-background);
      border-color: #555b64;
    }

    .service-tag:hover {
      color: #222222 !important;
      background-color: #dddddd;
      border-color: #dddddd;
    }
  }
</style>


<div class="profile-page">

  <!-- =======================================================
       About Me
       ======================================================= -->

  <div class="profile-intro">
    <p>
      <strong>Yongmin Yoo (유용민)</strong> is an AI researcher and PhD candidate at
      <a href="https://www.mq.edu.au/"
         target="_blank"
         rel="noopener noreferrer">Macquarie University</a>,
      affiliated with the
      <a href="https://www.mq.edu.au/research/research-centres-groups-and-facilities/centres/frontier-ai-research"
         target="_blank"
         rel="noopener noreferrer">Frontier AI Research Centre</a>.
      His research spans mechanistic interpretability and trustworthy LLMs,
      structured document intelligence, and AI-driven patent intelligence.
      By combining his academic background in law and industrial engineering
      with research and industry experience in NLP, he develops reliable and
      interpretable language technologies for high-stakes legal and technical domains.
    </p>

    <p>
      Before pursuing his PhD, he worked as an NLP researcher at
      <a href="https://www.nhn.com/en-US"
         target="_blank"
         rel="noopener noreferrer">NHN</a>
      for three years. He holds a master’s degree in Industrial Engineering from
      <a href="https://www.inha.ac.kr/eng/"
         target="_blank"
         rel="noopener noreferrer">Inha University</a>
      and bachelor’s degrees in Law and Industrial Engineering from
      <a href="https://kscms.ks.ac.kr/eng/Main.do"
         target="_blank"
         rel="noopener noreferrer">Kyungsung University</a>,
      providing a distinctive interdisciplinary foundation for his research
      at the intersection of AI, technology, and law.
    </p>

    <p>
      He is one of the few interdisciplinary AI researchers with formal degrees
      in both law and industrial engineering, complemented by doctoral training
      in computing and professional experience in NLP research and development.
      His distinctive strength lies in his ability to understand legal principles
      and institutional requirements while critically examining the inner workings
      and technical limitations of modern language models. Drawing on this rare
      combination of expertise, he bridges law and NLP to develop trustworthy and
      interpretable AI for high-stakes legal and technical domains.
    </p>
  </div>


  <!-- =======================================================
       Research Interests
       ======================================================= -->

  <h2 class="section-title">🔍 Research Interests</h2>

  <div class="research-grid">

    <article class="research-card">
      <span class="research-number">01</span>
      <h3>Mechanistic Interpretability and Trustworthy LLMs</h3>
      <p>
        Understanding how language models internally represent and process
        information to improve their robustness, reliability, and transparency
        in high-stakes domains.
      </p>
    </article>

    <article class="research-card">
      <span class="research-number">02</span>
      <h3>Structured Document Intelligence</h3>
      <p>
        Developing reliable methods for generating, representing, and evaluating
        complex legal and technical documents with hierarchical structures.
      </p>
    </article>

    <article class="research-card">
      <span class="research-number">03</span>
      <h3>AI for Patent Intelligence and Decision Support</h3>
      <p>
        Applying language models and machine learning to patent analysis,
        evaluation, similarity assessment, valuation, and innovation strategy.
      </p>
    </article>

  </div>

<!-- =======================================================
     News
     ======================================================= -->

<h2 class="section-title">💡 News</h2>

<div class="news-list">

  <article class="news-item">
    <div class="news-date">Sep 2026</div>

    <div class="news-content">
      <div class="news-summary">
        Paper accepted at
        <a class="news-venue"
           href="https://2026.aaclnet.org/"
           target="_blank"
           rel="noopener noreferrer">AACL-IJCNLP 2026</a>
        🎉🎉
      </div>

      <div class="author-role">
        Corresponding Author
      </div>

      <div class="news-paper-title">
        <em>
          Domain-Agnostic Neural Topic Modeling with Contextual Token-Level
          Semantic Graph Representation
        </em>
      </div>

      <a class="paper-button"
         href="https://arxiv.org/abs/2608.16269"
         target="_blank"
         rel="noopener noreferrer">
        View paper
        <span class="external-arrow" aria-hidden="true">↗</span>
      </a>
    </div>
  </article>


  <article class="news-item">
    <div class="news-date">Aug 2026</div>

    <div class="news-content">
      <div class="news-summary">
        Paper accepted at
        <a class="news-venue"
           href="https://2026.emnlp.org/"
           target="_blank"
           rel="noopener noreferrer">EMNLP 2026</a>
        🎉🎉
      </div>

      <div class="author-role">
        First Author
      </div>

      <div class="news-paper-title">
        <em>
          Adaptive Cost-Efficient Evaluation for Reliable Patent Claim Validation
        </em>
      </div>

      <a class="paper-button"
         href="https://arxiv.org/abs/2604.04295"
         target="_blank"
         rel="noopener noreferrer">
        View paper
        <span class="external-arrow" aria-hidden="true">↗</span>
      </a>
    </div>
  </article>


  <article class="news-item">
    <div class="news-date">May 2026</div>

    <div class="news-content">
      <div class="news-summary">
        Paper accepted at
        <a class="news-venue"
           href="https://www.sciencedirect.com/science/article/pii/S030645732600289X"
           target="_blank"
           rel="noopener noreferrer">Information Processing &amp; Management 2026</a>
        <span>(SSCI/SCIE Q1; #3 in Information Systems)</span>
        🎉🎉
      </div>

      <div class="author-role">
        First Author
      </div>

      <div class="news-paper-title">
        <em>
          ERA: Aligning Semantic Models with Revealed Economic Preference
          for Real-Time and Explainable Patent Valuation
        </em>
      </div>

      <a class="paper-button"
         href="https://www.sciencedirect.com/science/article/pii/S030645732600289X"
         target="_blank"
         rel="noopener noreferrer">
        View paper
        <span class="external-arrow" aria-hidden="true">↗</span>
      </a>
    </div>
  </article>


  <article class="news-item">
    <div class="news-date">Apr 2026</div>

    <div class="news-content">
      <div class="news-summary">
        Paper accepted at
        <a class="news-venue"
           href="https://2026.aclweb.org/"
           target="_blank"
           rel="noopener noreferrer">ACL 2026</a>
        🎉🎉
      </div>

      <div class="author-role">
        First Author
      </div>

      <div class="news-paper-title">
        <em>
          PatentMind: A Multi-Aspect Reasoning Graph for Patent Similarity Evaluation
        </em>
      </div>

      <a class="paper-button"
         href="https://aclanthology.org/2026.findings-acl.735/"
         target="_blank"
         rel="noopener noreferrer">
        View paper
        <span class="external-arrow" aria-hidden="true">↗</span>
      </a>
    </div>
  </article>


  <article class="news-item">
    <div class="news-date">Nov 2025</div>

    <div class="news-content">
      <div class="news-summary">
        Paper accepted at
        <a class="news-venue"
           href="https://2025.emnlp.org/"
           target="_blank"
           rel="noopener noreferrer">EMNLP 2025</a>
        🎉🎉
      </div>

      <div class="author-role">
        First Author
      </div>

      <div class="news-paper-title">
        <em>
          PatentScore: Multi-Dimensional Evaluation of LLM-Generated Patent Claims
        </em>
      </div>

      <a class="paper-button"
         href="https://aclanthology.org/2025.emnlp-main.1564/"
         target="_blank"
         rel="noopener noreferrer">
        View paper
        <span class="external-arrow" aria-hidden="true">↗</span>
      </a>
    </div>
  </article>


  <article class="news-item">
    <div class="news-date">Feb 2024</div>

    <div class="news-content">
      <div class="news-summary">
        Started PhD program in the School of Computing at
        <a class="news-venue"
           href="https://www.mq.edu.au/"
           target="_blank"
           rel="noopener noreferrer">Macquarie University</a>.
      </div>
    </div>
  </article>

</div>


  <!-- =======================================================
       Service
       ======================================================= -->

  <h2 class="section-title">💻 Service</h2>


  <section class="service-group">
    <h3 class="service-heading">
      Conference Organization &amp; Leadership
    </h3>

    <div class="service-row highlighted-service">
      <div class="service-date">Nov 2026</div>

      <div class="service-content">
        <span class="service-role">Special Session Chair</span>
        at
        <a class="service-event"
           href="https://besc-conf.org/2026/special-session-2"
           target="_blank"
           rel="noopener noreferrer">BESC 2026</a>

        <div class="service-description">
          “Integrated Smart Systems and Data-Driven AI”
        </div>
      </div>
    </div>
  </section>


  <section class="service-group">
    <h3 class="service-heading">
      Program Committee (PC) Member
    </h3>

    <div class="service-row">
      <div class="service-date">2026</div>

      <div class="service-tags">
        <a class="service-tag"
           href="https://neurips.cc/"
           target="_blank"
           rel="noopener noreferrer">NeurIPS</a>

        <a class="service-tag"
           href="https://aaai.org/conference/aaai/aaai-27/"
           target="_blank"
           rel="noopener noreferrer">AAAI</a>

        <a class="service-tag"
           href="https://2026.ijcai.org/"
           target="_blank"
           rel="noopener noreferrer">IJCAI</a>

        <a class="service-tag"
           href="https://www.pakdd2026.org/"
           target="_blank"
           rel="noopener noreferrer">PAKDD</a>

        <a class="service-tag"
           href="https://cikm2026.diag.uniroma1.it/"
           target="_blank"
           rel="noopener noreferrer">CIKM</a>

        <a class="service-tag"
           href="https://www.acml-conf.org/2026/"
           target="_blank"
           rel="noopener noreferrer">ACML</a>
      </div>
    </div>

    <div class="service-row">
      <div class="service-date">2025</div>

      <div class="service-tags">
        <a class="service-tag"
           href="https://2025.ijcai.org/"
           target="_blank"
           rel="noopener noreferrer">IJCAI</a>

        <a class="service-tag"
           href="https://iconip2025.apnns.org/"
           target="_blank"
           rel="noopener noreferrer">ICONIP</a>
      </div>
    </div>

    <div class="service-row">
      <div class="service-date">2024</div>

      <div class="service-tags">
        <a class="service-tag"
           href="https://iconip2024.org/"
           target="_blank"
           rel="noopener noreferrer">ICONIP</a>
      </div>
    </div>
  </section>


  <section class="service-group">
    <h3 class="service-heading">
      Journal Reviewer
    </h3>

    <div class="service-row">
      <div class="service-date">2026</div>

      <div class="service-tags">
        <a class="service-tag"
           href="https://link.springer.com/journal/11192"
           target="_blank"
           rel="noopener noreferrer">Scientometrics</a>

        <a class="service-tag"
           href="https://link.springer.com/journal/10994"
           target="_blank"
           rel="noopener noreferrer">Machine Learning (MLJ)</a>
      </div>
    </div>
  </section>

</div>
