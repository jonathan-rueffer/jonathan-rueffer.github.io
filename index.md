---
layout: page
title: Hi, I'm Jonathan
subtitle: M.S. Student in Computer Science · University of Maryland
---

I'm a first-year M.S. student in Computer Science at the University of Maryland,
broadly interested in the intersection of AI and security.

Before UMD, I earned a B.A. in Computer Science and Mathematics, with a minor in
History, from The College of Wooster. My senior thesis examined how to make parameter 
selection for CKKS homomorphic encryption more practical in the context of privacy-preserving 
machine learning.

## Updates

<div class="news-scroll" markdown="1">

- **Aug 2026** Started my M.S. in Computer Science at the University of Maryland.
- **May 2026** Graduated from The College of Wooster with a B.A. in Computer Science and Mathematics, earning departmental honors in both.
- **May 2026** Received Honors, Wooster's highest evaluation, for my senior thesis on CKKS parameter selection (check it out [here](https://github.com/jonathan-rueffer/ckks-parameter-selection)).
- **Feb 2026** Awarded The College of Wooster's Elizabeth Sidwell Wagner Prize in Mathematics, given annually to the student judged most likely to succeed in mathematics.

</div>

<style>
.news-scroll {
  --news-accent: #008AFF;
  max-height: 280px;
  overflow-y: auto;
  padding: 0.5rem 0.75rem 2.5rem 0.25rem;
  scrollbar-width: thin;
  scrollbar-color: rgba(128, 128, 128, 0.35) transparent;
  -webkit-mask-image: linear-gradient(to bottom, #000 80%, transparent);
  mask-image: linear-gradient(to bottom, #000 80%, transparent);
}
.news-scroll::-webkit-scrollbar { width: 6px; }
.news-scroll::-webkit-scrollbar-thumb {
  background: rgba(128, 128, 128, 0.35);
  border-radius: 3px;
}
.news-scroll ul {
  list-style: none;
  margin: 0 0 0 0.4rem;
  padding: 0;
  border-left: 2px solid rgba(128, 128, 128, 0.2);
}
.news-scroll li {
  position: relative;
  margin: 0;
  padding: 0 0 1.1rem 1.4rem;
  line-height: 1.5;
}
.news-scroll li::before {
  content: "";
  position: absolute;
  left: -7px;
  top: 0.3rem;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: #fff;
  border: 2px solid var(--news-accent);
}
.news-scroll li > strong:first-child {
  display: block;
  font-size: 0.75rem;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--news-accent);
  margin-bottom: 0.1rem;
}
</style>
