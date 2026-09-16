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

I have since extended this work with additional experiments, and a manuscript is in preparation.

[Code](https://github.com/jonathan-rueffer/ckks-parameter-selection) · [Thesis (PDF)](https://github.com/jonathan-rueffer/ckks-parameter-selection/blob/main/docs/RuefferJonathan_SeniorIS.pdf)

</div>

<div class="project-card" markdown="1">

### Music Journal: A Platform for Song-Based Memories
<p class="project-meta">Junior Independent Study & Personal Project · 2025–Present</p>

A full-stack application for associating songs with personal memories, organized by when and where a song was heard, the emotions it evokes, and the life events it belongs to. I developed the original web application as my Junior Independent Study at The College of Wooster, using KeyBERT keyword extraction to generate title suggestions from journal entries.

I have since begun rebuilding it as a multi-user mobile application with Spotify OAuth authentication and per-user data isolation enforced through PostgreSQL row-level security. The architecture is serverless: the client communicates directly with the database, a serverless function manages token refresh so credentials never ship in the app, and a relational schema supports many-to-many relationships between songs and user-defined life events.

[Mobile App Code](https://github.com/jonathan-rueffer/music-journal-mobile) · [Web App Code](https://github.com/jonathan-rueffer/music-journal-web)


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
