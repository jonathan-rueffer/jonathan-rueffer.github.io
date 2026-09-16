---
layout: page
title: Projects
subtitle: Research and things I've built
share-title: Projects
---

<div class="project-card" markdown="1">

### Privacy-Preserving Machine Learning: An Automated, Data-Driven Approach to Parameter Selection for Homomorphic Encryption
<p class="project-meta">Senior Independent Study Thesis · The College of Wooster · 2025-2026</p>

Homomorphic encryption enables machine learning inference on data it never sees, making it particularly useful in privacy-critical contexts, such as in finance or healthcare. However, schemes like CKKS are hard to use in practice because choosing encryption parameters requires extensive domain expertise and manual tuning to balance security, precision, and speed.

I developed a framework that automates this process. From the application-specific dataset and model, it generates candidate parameter configurations, evaluates them using privacy-preserving test vectors, identifies Pareto-optimal trade-offs between runtime and precision at each security level, allowing a user to make informed decisions about various trade-offs.

Awarded Honors, Wooster's highest evaluation, and presented as a talk and poster at the Wooster's 2026 Independent Study Symposium.

[Code](https://github.com/jonathan-rueffer/ckks-parameter-selection) · [Thesis (PDF)](https://github.com/jonathan-rueffer/ckks-parameter-selection/blob/main/docs/RuefferJonathan_SeniorIS.pdf)

<figure class="project-figure">
  <img src="/assets/img/Diabetes_full.png" alt="Pareto frontier of runtime versus precision for candidate CKKS parameter sets">
  <figcaption>Runtime vs. precision trade-offs across candidate parameter sets.</figcaption>
</figure>

I have since extended this work during the summer of 2026 with additional experiments, and a manuscript is in preparation.

</div>

<div class="project-card" markdown="1">

### JuniorIS: Music Journaling App
<p class="project-meta">Junior Independent Study · The College of Wooster · 2025</p>

[One or two sentences on what the app does and how it uses NLP.]
[Optional: a sentence on the current rebuild.]

<p class="project-tags"><span>[Language/Framework]</span><span>NLP</span><span>Mobile</span></p>

[Code](LINK)

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
