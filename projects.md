---
layout: page
title: Projects
subtitle: Research and selected projects
share-title: Projects
---

## Research

<div class="project-card" markdown="1">

### Automated Parameter Selection for Privacy-Preserving Machine Learning
<p class="project-meta">Senior Independent Study Thesis · The College of Wooster · 2025-2026</p>

Homomorphic encryption enables machine learning inference on data it never sees, making it particularly valuable in privacy-critical domains, such as finance or healthcare. In practice, however, schemes like CKKS are hard to use because choosing encryption parameters requires extensive domain expertise and manual tuning to balance security, precision, and speed.

I developed a framework that automates this process. Given an application's dataset and model, it generates candidate parameter configurations, evaluates them using privacy-preserving test vectors, and identifies the Pareto-optimal trade-offs between runtime and precision at each security level. From the recommended configurations, users can make an informed decision about parameters that reflect the underlying workload context.

The thesis was awarded Honors, Wooster's highest evaluation, and presented as a talk and poster at Wooster's 2026 Independent Study Symposium.

Advised by Prof. Alex Nord.

I have since extended this work with additional experiments, and a manuscript is in preparation.

<div class="project-figure-row">
  <figure class="project-figure figure-main">
    <img src="/assets/img/Diabetes_full.png" alt="Pareto frontier of runtime versus precision for candidate CKKS parameter sets">
    <figcaption>Candidate parameter sets for encrypted inference on the Wisconsin Diabetes dataset, plotted by runtime and error and colored by security level. Open circles mark Pareto-optimal configurations; ✕ marks the tool's recommendation at each level.</figcaption>
  </figure>
  <figure class="project-figure figure-secondary">
    <img src="/assets/img/IS_Symposium.jpg" alt="Jonathan Rueffer presenting his thesis poster at Wooster's Independent Study Symposium">
    <figcaption>Presenting the project at Wooster's 2026 Independent Study Symposium.</figcaption>
  </figure>
</div>

<div class="project-links">
<a href="https://openworks.wooster.edu/independentstudy/13425/" target="_blank" rel="noopener">Thesis</a> <a href="https://github.com/jonathan-rueffer/ckks-parameter-selection" target="_blank" rel="noopener">Code</a> <a href="https://github.com/jonathan-rueffer/ckks-parameter-selection/blob/main/docs/IS_Symposium_Poster_JonathanRueffer.pdf" target="_blank" rel="noopener">Poster</a> <a href="https://github.com/jonathan-rueffer/ckks-parameter-selection/blob/main/docs/IS_Symposium_OralPresentation_JonathanRueffer.pdf" target="_blank" rel="noopener">Slides</a>
</div>

</div>

<div class="project-card" markdown="1">

### Computer Hardware Analysis for Automated System Modeling
<p class="project-meta">Summer Research Associate · AMRE Program, The College of Wooster · 2024</p>

Under a funded contract with the University of Maryland's Laboratory for Physical Sciences, our three-student team explored how to identify the hardware characteristics of an unknown computer system using only performance measurements.

The developed microbenchmarks in C and Python probe CPU and cache behavior, and we designed timing-based methods for detecting properties such as cache size and associativity. Our team delivered a final technical report, a client presentation, and a documented codebase.

Advised by Prof. Robert Kelvey (The College of Wooster) and Prof. Nathan Sommer (Xavier University).

<div class="project-links">
<a href="https://github.com/AMRE-LPS/AMRE-2024-LPS" target="_blank" rel="noopener">Code</a> <a href="https://wooster.edu/news/2024/11/08/amre-team-laboratory-for-physical-sciences" target="_blank" rel="noopener">Project Summary</a>
</div>

</div>

## Other Projects

<div class="project-card minor" markdown="1">

### Inventory Management App
<p class="project-meta">IT Intern · Nucleonova, Valencia, Spain · 2025</p>

Nucleonova is a nuclear engineering procurement company. Its inventory lived in a large Excel spreadsheet that was slow to load and couldn't easily be shared with potential clients. I replaced it with an Android app and a web app that let staff quickly search and browse the company's inventory.

I built multi-field search and composable filters over the company's raw engineering codes, with English and Spanish localization for a bilingual team and clientele. I shipped features in weekly cycles and refined the interface based on feedback from stakeholders.

</div>

<div class="project-card minor" markdown="1">

### Music Journal: A Platform for Song-Based Memories
<p class="project-meta">Junior Independent Study & Personal Project · The College of Wooster · 2025-2026</p>

A full-stack application for associating songs with personal memories, organized by when and where a song was heard, the emotions it evokes, and the life events it belongs to. I developed the original web application as part of my Junior Independent Study on NLP and Information Extraction at The College of Wooster. The application integrates the Spotify API for song information and uses KeyBERT keyword extraction to generate title suggestions from journal entries. 

<div class="project-links">
<a href="https://github.com/jonathan-rueffer/music-journal-web" target="_blank" rel="noopener">Code (Web)</a> <a href="https://github.com/jonathan-rueffer/music-journal-web/blob/main/docs/JuniorIS_JonathanRueffer.pdf" target="_blank" rel="noopener">Paper</a> <a href="https://github.com/jonathan-rueffer/music-journal-web/blob/main/docs/JuniorIS_JonathanRueffer_Presentation.pdf" target="_blank" rel="noopener">Presentation</a>
</div>

I have since begun rebuilding it as a multi-user mobile application with Spotify OAuth authentication and per-user data isolation enforced through PostgreSQL row-level security. The architecture is serverless: the client communicates directly with the database, a serverless function manages token refresh so credentials never ship in the app, and a relational schema supports many-to-many relationships between songs and user-defined life events.

<div class="project-links">
<a href="https://github.com/jonathan-rueffer/music-journal-mobile" target="_blank" rel="noopener">Code (Mobile)</a>
</div>

</div>

## Writing

<p class="project-meta">Science Section Editor · The Wooster Voice · 2025-2026</p>

<ul class="writing-list">
  <li><a href="https://thewoostervoice.spaces.wooster.edu/2026/04/17/what-does-accept-all-cookies-actually-mean/" target="_blank" rel="noopener">What does "accept all cookies" actually mean?</a><span class="writing-date">2026</span></li>
  <li><a href="https://thewoostervoice.spaces.wooster.edu/2026/02/27/what-is-the-ai-bubble-and-what-if-it-bursts/" target="_blank" rel="noopener">What is the AI bubble and what if it bursts?</a><span class="writing-date">2026</span></li>
  <li><a href="https://thewoostervoice.spaces.wooster.edu/2026/02/27/theres-more-to-math-than-numbers/" target="_blank" rel="noopener">There’s more to math than numbers</a><span class="writing-date">2026</span></li>
  <li><a href="https://thewoostervoice.spaces.wooster.edu/2025/11/14/what-is-cloud-computing-and-how-does-it-work/" target="_blank" rel="noopener">What is cloud computing and how does it work?</a><span class="writing-date">2025</span></li>
  <li><a href="https://thewoostervoice.spaces.wooster.edu/2025/10/03/what-is-chatgpt-and-how-does-it-work/" target="_blank" rel="noopener">What is ChatGPT and how does it work?</a><span class="writing-date">2025</span></li>
  <li><a href="https://thewoostervoice.spaces.wooster.edu/2025/02/21/deepseek-chinas-challenge-to-u-s-ai-domination/" target="_blank" rel="noopener">DeepSeek: China's challenge to U.S. AI domination</a><span class="writing-date">2025</span></li>
</ul>

<div class="project-links">
<a href="https://thewoostervoice.spaces.wooster.edu/author/jrueffer26/" target="_blank" rel="noopener">More articles</a>
</div>


<style>
/* Widen the page content area beyond the theme's default column */
@media (min-width: 992px) {
  .col-lg-10 { flex: 0 0 91.6667%; max-width: 91.6667%; }
  .offset-lg-1 { margin-left: 4.1667%; }
}
@media (min-width: 1200px) {
  .col-xl-8 { flex: 0 0 83.3333%; max-width: 83.3333%; }
  .offset-xl-2 { margin-left: 8.3333%; }
}

h2 {
  margin: 3.5rem 0 2rem;
  padding-top: 2.5rem;
  border-top: 1px solid #dcdcdc;
  font-size: 1.05rem;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #1a1a1a;
}
h2:first-of-type {
  margin-top: 1.5rem;
}
.project-card {
  padding: 0 0 2.25rem;
  margin-bottom: 2.25rem;
  border-bottom: 1px solid #dcdcdc;
}
.project-card:has(+ h2) {
  border-bottom: none;
  margin-bottom: 0;
  padding-bottom: 0;
}
.project-card h3 {
  margin-top: 0;
  margin-bottom: 0.3rem;
  font-size: 1.25rem;
  font-weight: 700;
  line-height: 1.35;
  color: #1a1a1a;
}
.project-card.minor h3 {
  font-size: 1.05rem;
}
.project-card p {
  margin: 0 0 0.85rem;
  line-height: 1.6;
}
.project-meta {
  font-size: 0.85rem;
  font-weight: 400;
  color: #6b6b6b;
  margin-bottom: 0.9rem;
}
.project-figure-row {
  display: flex;
  flex-wrap: wrap;
  gap: 1.25rem;
  align-items: center;
}
.project-figure-row .project-figure {
  margin: 0.75rem 0 1rem;
}
.project-figure-row .figure-main,
.project-figure-row .figure-secondary {
  flex: 1 1 220px;
}
.project-figure {
  margin: 0.75rem 0 1rem;
  text-align: center;
}
.project-figure img {
  max-width: 100%;
  height: auto;
  border-radius: 2px;
  border: 1px solid #d5d5d5;
}
.project-figure figcaption {
  font-size: 0.8rem;
  color: #777;
  margin-top: 0.4rem;
}
.project-links {
  display: flex;
  flex-wrap: wrap;
  row-gap: 0.4rem;
  margin: 0.9rem 0;
  font-size: 0.9rem;
}
.project-links a {
  color: #1a1a1a;
  font-weight: 600;
  text-decoration: underline;
  text-underline-offset: 3px;
  text-decoration-color: #b8b8b8;
  transition: text-decoration-color 0.15s ease;
  padding: 0 1rem;
  border-right: 1px solid #d5d5d5;
  line-height: 1;
}
.project-links a:first-child {
  padding-left: 0;
}
.project-links a:last-child {
  border-right: none;
  padding-right: 0;
}
.project-links a:hover {
  text-decoration-color: #1a1a1a;
}
.writing-list {
  list-style: none;
  margin: 0;
  padding: 0;
}
.writing-list li {
  display: flex;
  flex-wrap: wrap;
  align-items: baseline;
  justify-content: space-between;
  gap: 0.35rem 1rem;
  padding: 0.75rem 0;
  border-bottom: 1px solid #e2e2e2;
}
.writing-list li:first-child {
  padding-top: 0.1rem;
}
.writing-list li:last-child {
  border-bottom: none;
  padding-bottom: 0.1rem;
}
.writing-list a {
  font-weight: 600;
  color: #1a1a1a;
  text-decoration: none;
}
.writing-list a:hover {
  text-decoration: underline;
  text-underline-offset: 3px;
}
.writing-date {
  font-size: 0.8rem;
  color: #6b6b6b;
  white-space: nowrap;
}
</style>
