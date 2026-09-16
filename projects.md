---
layout: page
title: Projects
subtitle: Research and things I've built
share-title: Projects
---

<div class="project-card" markdown="1">

### Privacy-Preserving Machine Learning: An Automated, Data-Driven Approach to Parameter Selection for Homomorphic Encryption
<p class="project-meta">Senior Independent Study Thesis · The College of Wooster · 2025-2026</p>

Homomorphic encryption enables machine learning inference on data it never sees, making it particularly valuable in privacy-critical domains, such as finance or healthcare. In practice, however, schemes like CKKS are hard to use because choosing encryption parameters requires extensive domain expertise and manual tuning to balance security, precision, and speed.

I developed a framework that automates this process. Given an application's dataset and model, it generates candidate parameter configurations, evaluates them using privacy-preserving test vectors, and identifies the Pareto-optimal trade-offs between runtime and precision at each security level. From the recommended configurations, users can make an informed decision about parameters that reflect the underlying workload context.

The thesis was awarded Honors, Wooster's highest evaluation, and presented as a talk and poster at the Wooster's 2026 Independent Study Symposium.

<figure class="project-figure">
  <img src="/assets/img/Diabetes_full.png" alt="Pareto frontier of runtime versus precision for candidate CKKS parameter sets">
  <figcaption>Candidate parameter sets for encrypted inference on the Wisconsin Diabetes dataset, plotted by runtime and error and colored by security level. Open circles mark Pareto-optimal configurations; ✕ marks the tool's recommendation at each level.</figcaption>
</figure>

Advised by Prof. Alex Nord.

I have since extended this work with additional experiments, and a manuscript is in preparation.

[Code](https://github.com/jonathan-rueffer/ckks-parameter-selection) · [Thesis](https://github.com/jonathan-rueffer/ckks-parameter-selection/blob/main/docs/RuefferJonathan_SeniorIS.pdf) · [Poster](https://github.com/jonathan-rueffer/ckks-parameter-selection/blob/main/docs/IS_Symposium_Poster_JonathanRueffer.pdf) · [Slides](https://github.com/jonathan-rueffer/ckks-parameter-selection/blob/main/docs/IS_Symposium_OralPresentation_JonathanRueffer.pdf)

</div>

<div class="project-card" markdown="1">

### Computer Hardware Analysis for Automated System Modeling
<p class="project-meta">Summer Research Associate · AMRE Program, The College of Wooster · 2024</p>

Under a funded contract with the University of Maryland's Laboratory for Physical Sciences, our three-student team explored how to identify the hardware characteristics of an unknown computer system using only performance measurements.

The developed microbenchmarks in C and Python probe CPU and cache behavior, and we designed timing-based methods for detecting properties such as cache size and associativity. Our team delivered a final technical report, a client presentation, and a documented codebase.

Advised by Prof. Robert Kelvey (The College of Wooster) and Prof. Nathan Sommer (Xavier University).

[Code](https://github.com/AMRE-LPS/AMRE-2024-LPS) · [Project Summary](https://wooster.edu/news/2024/11/08/amre-team-laboratory-for-physical-sciences)

</div>

<div class="project-card" markdown="1">

### Inventory Management App
<p class="project-meta">IT Intern · Nucleonova, Valencia, Spain · 2025</p>

Nucleonova is a nuclear engineering procurement company. Its inventory lived in a large Excel spreadsheet that was slow to load and couldn't easily be shared with potential clients. I replaced it with an Android app and a web app that let staff quickly search and browse the company's inventory.

I built multi-field search and composable filters over the company's raw engineering codes, with English and Spanish localization for a bilingual team and clientele. I shipped features in weekly cycles and refined the interface based on feedback from stakeholders.

</div>

<div class="project-card" markdown="1">

### Music Journal: A Platform for Song-Based Memories
<p class="project-meta">Junior Independent Study & Personal Project · The College of Wooster · 2025-2026</p>

A full-stack application for associating songs with personal memories, organized by when and where a song was heard, the emotions it evokes, and the life events it belongs to. I developed the original web application as part of my Junior Independent Study on NLP and Information Extraction at The College of Wooster. The application integrates the Spotify API for song information and uses KeyBERT keyword extraction to generate title suggestions from journal entries. 

[Code](https://github.com/jonathan-rueffer/music-journal-web) · [Paper](https://github.com/jonathan-rueffer/music-journal-web/blob/main/docs/JuniorIS_JonathanRueffer.pdf) · [Presentation](https://github.com/jonathan-rueffer/music-journal-web/blob/main/docs/JuniorIS_JonathanRueffer_Presentation.pdf) 

---

I have since begun rebuilding it as a multi-user mobile application with Spotify OAuth authentication and per-user data isolation enforced through PostgreSQL row-level security. The architecture is serverless: the client communicates directly with the database, a serverless function manages token refresh so credentials never ship in the app, and a relational schema supports many-to-many relationships between songs and user-defined life events.

[Code](https://github.com/jonathan-rueffer/music-journal-mobile) 


</div>


<style>
.project-card {
  padding: 1.25rem 1.5rem;
  margin-bottom: 1.5rem;
  border: 1px solid rgba(128, 128, 128, 0.25);
  border-radius: 10px;
}
.project-card h3 {
  margin-top: 0;
  margin-bottom: 0.25rem;
  font-size: 1.2rem;
}
.project-meta {
  font-size: 0.8rem;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #008AFF;
  margin-bottom: 0.75rem;
}
.project-tags {
  margin: 0.75rem 0 0.5rem;
}
.project-tags span {
  display: inline-block;
  font-size: 0.75rem;
  padding: 0.15rem 0.6rem;
  margin: 0 0.35rem 0.35rem 0;
  border-radius: 999px;
  background: rgba(0, 138, 255, 0.1);
  color: #0066bb;
}
  .project-figure {
  margin: 0.75rem 0 1rem;
  text-align: center;
}
.project-figure img {
  max-width: 100%;
  height: auto;
  border-radius: 6px;
  border: 1px solid rgba(128, 128, 128, 0.2);
}
.project-figure figcaption {
  font-size: 0.8rem;
  color: #777;
  margin-top: 0.4rem;
}
</style>
