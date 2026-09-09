---
layout: archive
title: "Research Interests"
permalink: /research/
author_profile: true
---

<style>
  /* =========================================================
     Page-wide design
     ========================================================= */

  .research-page {
    --research-text: #303640;
    --research-muted: #6b7280;
    --research-border: #e4e7eb;
    --research-soft-border: #eef0f2;
    --research-background: #ffffff;
    --research-soft-background: #f8f9fa;
    --research-accent: #3f5268;
    --research-accent-dark: #303d4d;
    --research-gold: #c59628;
    --research-gold-background: #fff9e9;

    color: var(--research-text);
  }

  .research-page a {
    transition:
      color 0.2s ease,
      background-color 0.2s ease,
      border-color 0.2s ease,
      transform 0.2s ease;
  }


  /* =========================================================
     Research hero
     ========================================================= */

  .research-hero {
    position: relative;
    margin-bottom: 2.4rem;
    padding: 1.7rem 1.8rem;
    overflow: hidden;
    border: 1px solid var(--research-border);
    border-left: 5px solid var(--research-gold);
    border-radius: 9px;
    background:
      linear-gradient(
        135deg,
        rgba(255, 249, 233, 0.9),
        rgba(248, 249, 250, 0.75)
      );
    box-shadow: 0 3px 12px rgba(31, 41, 55, 0.04);
  }

  .research-hero::after {
    content: "";
    position: absolute;
    top: -80px;
    right: -70px;
    width: 210px;
    height: 210px;
    border-radius: 50%;
    background: rgba(197, 150, 40, 0.055);
    pointer-events: none;
  }

  .research-eyebrow {
    position: relative;
    z-index: 1;
    margin-bottom: 0.65rem;
    color: #8a6817;
    font-size: 0.74em;
    font-weight: 800;
    letter-spacing: 0.1em;
    text-transform: uppercase;
  }

  .research-hero-title {
    position: relative;
    z-index: 1;
    max-width: 760px;
    margin: 0 0 0.8rem;
    color: var(--research-text);
    font-size: 1.3em;
    line-height: 1.45;
  }

  .research-hero-description {
    position: relative;
    z-index: 1;
    max-width: 800px;
    margin: 0;
    color: #555d68;
    font-size: 0.94em;
    line-height: 1.75;
  }

  .research-principles {
    position: relative;
    z-index: 1;
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-top: 1.1rem;
  }

  .principle-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.3rem 0.7rem;
    color: #4b515b;
    background-color: rgba(255, 255, 255, 0.75);
    border: 1px solid #dfe2e6;
    border-radius: 999px;
    font-size: 0.76em;
    font-weight: 650;
  }


  /* =========================================================
     Section headings
     ========================================================= */

  .research-section-heading {
    display: flex;
    align-items: center;
    gap: 0.55rem;
    margin: 2.7rem 0 1.2rem;
    padding-bottom: 0.6rem;
    color: var(--research-text);
    border-bottom: 1px solid var(--research-border);
  }

  .research-section-heading:first-of-type {
    margin-top: 0;
  }


  /* =========================================================
     Research overview
     ========================================================= */

  .research-overview {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 0.9rem;
    margin-bottom: 2.7rem;
  }

  .overview-card {
    display: flex;
    flex-direction: column;
    min-height: 205px;
    padding: 1.1rem;
    color: inherit !important;
    background-color: var(--research-background);
    border: 1px solid var(--research-border);
    border-radius: 8px;
    text-decoration: none !important;
    box-shadow: 0 2px 8px rgba(31, 41, 55, 0.035);
    transition:
      transform 0.2s ease,
      border-color 0.2s ease,
      box-shadow 0.2s ease;
  }

  .overview-card:hover {
    transform: translateY(-3px);
    border-color: #c8cdd4;
    box-shadow: 0 8px 18px rgba(31, 41, 55, 0.07);
    text-decoration: none !important;
  }

  .overview-number {
    display: inline-block;
    margin-bottom: 0.55rem;
    color: var(--research-gold);
    font-size: 0.74em;
    font-weight: 800;
    letter-spacing: 0.09em;
  }

  .overview-card h3 {
    margin: 0 0 0.55rem;
    color: var(--research-text);
    font-size: 0.97em;
    line-height: 1.45;
  }

  .overview-card p {
    margin: 0;
    color: var(--research-muted);
    font-size: 0.83em;
    line-height: 1.6;
  }

  .overview-link {
    margin-top: auto;
    padding-top: 0.8rem;
    color: var(--research-accent);
    font-size: 0.76em;
    font-weight: 700;
  }


  /* =========================================================
     Detailed research areas
     ========================================================= */

  .research-area {
    margin-bottom: 1.3rem;
    padding: 1.45rem 1.5rem;
    border: 1px solid var(--research-border);
    border-radius: 9px;
    background-color: var(--research-background);
    box-shadow: 0 2px 10px rgba(31, 41, 55, 0.035);
    scroll-margin-top: 90px;
  }

  .research-area-header {
    display: grid;
    grid-template-columns: 52px minmax(0, 1fr);
    gap: 0.9rem;
    align-items: start;
    margin-bottom: 1rem;
  }

  .research-area-number {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 46px;
    height: 46px;
    color: #ffffff;
    background: linear-gradient(
      135deg,
      var(--research-accent),
      var(--research-accent-dark)
    );
    border: 1px solid rgba(197, 150, 40, 0.75);
    border-radius: 50%;
    font-size: 0.78em;
    font-weight: 800;
    letter-spacing: 0.04em;
    box-shadow: 0 3px 8px rgba(48, 61, 77, 0.15);
  }

  .research-area-kicker {
    margin-bottom: 0.25rem;
    color: var(--research-gold);
    font-size: 0.7em;
    font-weight: 800;
    letter-spacing: 0.09em;
    text-transform: uppercase;
  }

  .research-area-title {
    margin: 0;
    color: var(--research-text);
    font-size: 1.15em;
    line-height: 1.4;
  }

  .research-question {
    margin: 0.9rem 0 1.15rem;
    padding: 0.8rem 1rem;
    color: #394858;
    background-color: #f5f7f9;
    border-left: 3px solid var(--research-accent);
    border-radius: 0 6px 6px 0;
    font-size: 0.89em;
    font-weight: 650;
    line-height: 1.6;
  }

  .research-area-body {
    color: #4e5661;
    line-height: 1.75;
  }

  .research-area-body p {
    margin: 0 0 0.9rem;
  }

  .research-area-body p:last-child {
    margin-bottom: 0;
  }

  .research-area-body strong {
    color: var(--research-text);
  }


  /* =========================================================
     Research topic tags
     ========================================================= */

  .topic-label {
    margin-top: 1.2rem;
    margin-bottom: 0.55rem;
    color: var(--research-muted);
    font-size: 0.72em;
    font-weight: 800;
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }

  .topic-list {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
  }

  .topic-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.28rem 0.68rem;
    color: #454c56;
    background-color: var(--research-soft-background);
    border: 1px solid #dfe2e6;
    border-radius: 999px;
    font-size: 0.76em;
    font-weight: 600;
    line-height: 1.3;
  }


  /* =========================================================
     Research approach
     ========================================================= */

  .research-approach {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 0;
    margin: 2.7rem 0;
    overflow: hidden;
    border: 1px solid var(--research-border);
    border-radius: 9px;
    background-color: var(--research-soft-background);
  }

  .approach-step {
    position: relative;
    padding: 1.15rem;
    border-right: 1px solid var(--research-border);
  }

  .approach-step:last-child {
    border-right: none;
  }

  .approach-step-number {
    display: block;
    margin-bottom: 0.35rem;
    color: var(--research-gold);
    font-size: 0.72em;
    font-weight: 800;
    letter-spacing: 0.08em;
  }

  .approach-step h3 {
    margin: 0 0 0.4rem;
    color: var(--research-text);
    font-size: 0.93em;
  }

  .approach-step p {
    margin: 0;
    color: var(--research-muted);
    font-size: 0.8em;
    line-height: 1.6;
  }


  /* =========================================================
     Collaboration section
     ========================================================= */

  .collaboration-box {
    margin-top: 2.7rem;
    padding: 1.5rem 1.6rem;
    color: #ffffff;
    background: linear-gradient(
      135deg,
      var(--research-accent-dark),
      var(--research-accent)
    );
    border: 1px solid rgba(197, 150, 40, 0.65);
    border-radius: 9px;
    box-shadow: 0 5px 18px rgba(48, 61, 77, 0.15);
  }

  .collaboration-eyebrow {
    margin-bottom: 0.4rem;
    color: #e7ca78;
    font-size: 0.72em;
    font-weight: 800;
    letter-spacing: 0.09em;
    text-transform: uppercase;
  }

  .collaboration-box h2 {
    margin: 0 0 0.6rem;
    color: #ffffff;
    font-size: 1.16em;
  }

  .collaboration-box p {
    max-width: 780px;
    margin: 0;
    color: rgba(255, 255, 255, 0.84);
    font-size: 0.88em;
    line-height: 1.7;
  }

  .contact-button {
    display: inline-flex;
    align-items: center;
    gap: 0.35rem;
    margin-top: 1rem;
    padding: 0.42rem 0.85rem;
    color: #2f3b49 !important;
    background-color: #ffffff;
    border: 1px solid #ffffff;
    border-radius: 999px;
    font-size: 0.78em;
    font-weight: 750;
    text-decoration: none !important;
  }

  .contact-button:hover {
    color: #ffffff !important;
    background-color: transparent;
    text-decoration: none !important;
    transform: translateY(-1px);
  }


  /* =========================================================
     Responsive design
     ========================================================= */

  @media (max-width: 900px) {
    .research-overview {
      grid-template-columns: 1fr;
    }

    .overview-card {
      min-height: auto;
    }

    .research-approach {
      grid-template-columns: 1fr;
    }

    .approach-step {
      border-right: none;
      border-bottom: 1px solid var(--research-border);
    }

    .approach-step:last-child {
      border-bottom: none;
    }
  }

  @media (max-width: 600px) {
    .research-hero {
      padding: 1.35rem 1.2rem;
    }

    .research-hero-title {
      font-size: 1.12em;
    }

    .research-area {
      padding: 1.2rem 1.05rem;
    }

    .research-area-header {
      grid-template-columns: 42px minmax(0, 1fr);
      gap: 0.75rem;
    }

    .research-area-number {
      width: 39px;
      height: 39px;
    }

    .research-area-title {
      font-size: 1.02em;
    }

    .collaboration-box {
      padding: 1.3rem 1.2rem;
    }
  }


  /* =========================================================
     Dark mode
     ========================================================= */

  @media (prefers-color-scheme: dark) {
    .research-page {
      --research-text: #eeeeee;
      --research-muted: #b3b7bd;
      --research-border: #444951;
      --research-soft-border: #343940;
      --research-background: rgba(255, 255, 255, 0.025);
      --research-soft-background: rgba(255, 255, 255, 0.05);
      --research-gold-background: rgba(197, 150, 40, 0.12);
    }

    .research-hero {
      background:
        linear-gradient(
          135deg,
          rgba(197, 150, 40, 0.1),
          rgba(255, 255, 255, 0.02)
        );
      box-shadow: none;
    }

    .research-hero-title {
      color: var(--research-text);
    }

    .research-hero-description {
      color: #c1c4c9;
    }

    .research-eyebrow {
      color: #d5b55d;
    }

    .principle-tag {
      color: #dddddd;
      background-color: rgba(255, 255, 255, 0.045);
      border-color: #555b64;
    }

    .overview-card,
    .research-area {
      background-color: var(--research-background);
      box-shadow: none;
    }

    .overview-card:hover,
    .research-area:hover {
      border-color: #60666f;
      box-shadow: none;
    }

    .overview-card h3,
    .research-area-title,
    .approach-step h3 {
      color: var(--research-text);
    }

    .research-question {
      color: #d4dae0;
      background-color: rgba(255, 255, 255, 0.045);
      border-left-color: #8aa3bb;
    }

    .research-area-body {
      color: #c2c5ca;
    }

    .research-area-body strong {
      color: #eeeeee;
    }

    .topic-tag {
      color: #dddddd;
      background-color: var(--research-soft-background);
      border-color: #555b64;
    }

    .research-approach {
      background-color: rgba(255, 255, 255, 0.025);
    }

    .collaboration-box {
      background:
        linear-gradient(
          135deg,
          rgba(32, 42, 53, 0.98),
          rgba(55, 70, 87, 0.98)
        );
    }
  }
</style>


<div class="research-page">

  <!-- =======================================================
       Research agenda
       ======================================================= -->

  <section class="research-hero">
    <div class="research-eyebrow">Research Agenda</div>

    <h2 class="research-hero-title">
      Building reliable and interpretable language technologies
      for complex, high-stakes domains
    </h2>

    <p class="research-hero-description">
      My research lies at the intersection of
      <strong>mechanistic interpretability</strong>,
      <strong>trustworthy language models</strong>, and
      <strong>structured document intelligence</strong>,
      with a particular focus on Legal AI and patent intelligence.
      I study how language models reason, represent complex information,
      and make decisions in settings where reliability, transparency,
      and domain validity are essential.
    </p>

    <div class="research-principles">
      <span class="principle-tag">Interpretability</span>
      <span class="principle-tag">Reliability</span>
      <span class="principle-tag">Structural Coherence</span>
      <span class="principle-tag">Domain Validity</span>
      <span class="principle-tag">Decision Support</span>
    </div>
  </section>


  <!-- =======================================================
       Research overview
       ======================================================= -->

  <h2 class="research-section-heading">Research Focus</h2>

  <div class="research-overview">

    <a class="overview-card" href="#mechanistic-interpretability">
      <span class="overview-number">01</span>

      <h3>
        Mechanistic Interpretability and Trustworthy LLMs
      </h3>

      <p>
        Understanding internal model mechanisms and identifying the
        representations associated with reasoning, robustness, and failure.
      </p>

      <span class="overview-link">Explore this area ↓</span>
    </a>


    <a class="overview-card" href="#structured-document-intelligence">
      <span class="overview-number">02</span>

      <h3>
        Structured Document Intelligence
      </h3>

      <p>
        Developing models that preserve the hierarchical, semantic,
        and functional structures of legal and technical documents.
      </p>

      <span class="overview-link">Explore this area ↓</span>
    </a>


    <a class="overview-card" href="#patent-intelligence">
      <span class="overview-number">03</span>

      <h3>
        AI for Patent Intelligence and Decision Support
      </h3>

      <p>
        Transforming complex patent information into interpretable
        and actionable evidence for intellectual-property decisions.
      </p>

      <span class="overview-link">Explore this area ↓</span>
    </a>

  </div>


  <!-- =======================================================
       Research area 1
       ======================================================= -->

  <article class="research-area" id="mechanistic-interpretability">

    <header class="research-area-header">
      <div class="research-area-number">01</div>

      <div>
        <div class="research-area-kicker">Understanding Model Behavior</div>

        <h2 class="research-area-title">
          Mechanistic Interpretability and Trustworthy LLMs
        </h2>
      </div>
    </header>

    <div class="research-question">
      How do language models internally represent information, produce
      decisions, and become sensitive to irrelevant contextual variations?
    </div>

    <div class="research-area-body">
      <p>
        I investigate how language models internally represent information
        and produce decisions, particularly when their outputs are sensitive
        to irrelevant context, role framing, or subtle variations in input.
        My research combines behavioral evaluation with mechanistic analysis
        to identify the internal components and representations associated
        with model reasoning and failure.
      </p>

      <p>
        The broader goal is to develop language models that are not only
        accurate, but also <strong>robust, interpretable, and appropriately
        calibrated</strong> for high-stakes decision-making.
      </p>
    </div>

    <div class="topic-label">Research Topics</div>

    <div class="topic-list">
      <span class="topic-tag">Mechanistic Interpretability</span>
      <span class="topic-tag">Representation Analysis</span>
      <span class="topic-tag">Representation Intervention</span>
      <span class="topic-tag">Robustness</span>
      <span class="topic-tag">Uncertainty</span>
      <span class="topic-tag">Causal Analysis</span>
      <span class="topic-tag">Reliable Reasoning</span>
    </div>

  </article>


  <!-- =======================================================
       Research area 2
       ======================================================= -->

  <article class="research-area" id="structured-document-intelligence">

    <header class="research-area-header">
      <div class="research-area-number">02</div>

      <div>
        <div class="research-area-kicker">Modeling Complex Structure</div>

        <h2 class="research-area-title">
          Structured Document Intelligence
        </h2>
      </div>
    </header>

    <div class="research-question">
      How can language models generate, represent, and evaluate specialized
      documents while preserving their hierarchical and semantic structure?
    </div>

    <div class="research-area-body">
      <p>
        Legal and technical documents often contain complex hierarchical
        structures, dependencies, and domain-specific constraints that
        conventional language models do not explicitly capture. I develop
        methods for generating, representing, and evaluating such documents
        while preserving their structural and semantic coherence.
      </p>

      <p>
        This research explores structure-aware generation, hierarchical
        document representation, constrained decoding, and domain-grounded
        evaluation. The objective is to move beyond surface-level text
        quality toward models that respect the
        <strong>logical organization, functional relationships, and formal
        requirements</strong> of specialized documents.
      </p>
    </div>

    <div class="topic-label">Research Topics</div>

    <div class="topic-list">
      <span class="topic-tag">Structured Generation</span>
      <span class="topic-tag">Hierarchical Representation</span>
      <span class="topic-tag">Controllable Decoding</span>
      <span class="topic-tag">Document Evaluation</span>
      <span class="topic-tag">Representation Intervention</span>
      <span class="topic-tag">Domain-Grounded Evaluation</span>
    </div>

  </article>


  <!-- =======================================================
       Research area 3
       ======================================================= -->

  <article class="research-area" id="patent-intelligence">

    <header class="research-area-header">
      <div class="research-area-number">03</div>

      <div>
        <div class="research-area-kicker">Supporting Expert Decisions</div>

        <h2 class="research-area-title">
          AI for Patent Intelligence and Decision Support
        </h2>
      </div>
    </header>

    <div class="research-question">
      How can AI transform complex patent information into transparent,
      legally grounded, and actionable evidence?
    </div>

    <div class="research-area-body">
      <p>
        Patents provide a challenging environment for AI because they combine
        technical knowledge, legal reasoning, economic value, and highly
        structured language. I develop AI methods for patent generation,
        evaluation, similarity assessment, classification, and valuation.
      </p>

      <p>
        My research aims to transform complex patent information into
        transparent and actionable evidence for tasks such as prior-art
        analysis, claim assessment, technology evaluation, and
        intellectual-property decision-making. A central priority is ensuring
        that AI-based patent analysis remains
        <strong>interpretable, legally grounded, and aligned with expert
        judgment</strong>.
      </p>
    </div>

    <div class="topic-label">Research Topics</div>

    <div class="topic-list">
      <span class="topic-tag">Patent Generation</span>
      <span class="topic-tag">Patent Evaluation</span>
      <span class="topic-tag">Patent Similarity</span>
      <span class="topic-tag">Legal Validity Assessment</span>
      <span class="topic-tag">Explainable Valuation</span>
      <span class="topic-tag">Prior-Art Analysis</span>
      <span class="topic-tag">IP Decision Support</span>
    </div>

  </article>


  <!-- =======================================================
       Research approach
       ======================================================= -->

  <h2 class="research-section-heading">Research Approach</h2>

  <div class="research-approach">

    <div class="approach-step">
      <span class="approach-step-number">STEP 01</span>

      <h3>Analyze</h3>

      <p>
        Identify behavioral patterns, internal representations, structural
        limitations, and domain-specific failure modes.
      </p>
    </div>


    <div class="approach-step">
      <span class="approach-step-number">STEP 02</span>

      <h3>Intervene</h3>

      <p>
        Develop structure-aware and mechanism-informed methods that improve
        model reliability, control, and interpretability.
      </p>
    </div>


    <div class="approach-step">
      <span class="approach-step-number">STEP 03</span>

      <h3>Validate</h3>

      <p>
        Evaluate model behavior against domain requirements, expert judgment,
        and real-world decision-making objectives.
      </p>
    </div>

  </div>


  <!-- =======================================================
       Collaboration
       ======================================================= -->

  <section class="collaboration-box">
    <div class="collaboration-eyebrow">Research Collaboration</div>

    <h2>Interested in working together?</h2>

    <p>
      I welcome research collaborations at the intersection of trustworthy AI,
      mechanistic interpretability, structured document intelligence, Legal AI,
      and patent intelligence.
    </p>

    <a class="contact-button"
       href="mailto:yooyongmin91@gmail.com">
      Contact me
      <span aria-hidden="true">↗</span>
    </a>
  </section>

</div>
