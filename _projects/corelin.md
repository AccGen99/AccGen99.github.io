---
layout: page
title: CoReLIN - Constraint-based reasoning for lifelong interactive navigation
description: CoReLIN - Constraint-based reasoning for lifelong interactive navigation
permalink: /projects/corelin/
img: assets/img/12.jpg
importance: 1
category: work
related_publications: false

_styles: |
  .post-header {
    text-align: center;
  }

  .post-title {
    font-weight: 700;
    text-align: center;
    margin-bottom: 1rem;
  }

  .post-description {
    display: none;
  }

  .project-section-title {
    text-align: center;
    font-size: 1.25rem;
    font-weight: 400;
    margin-top: 2.75rem;
    margin-bottom: 1.25rem;
  }

  .project-text {
    text-align: justify;
    text-justify: inter-word;
    line-height: 1.75;
    margin-bottom: 2rem;
  }

  .project-image {
    display: block;
    width: 100%;
    max-width: 850px;
    height: auto;
    margin: 1.5rem auto 2rem;
    border-radius: 8px;
  }

  .project-video {
    position: relative;
    width: 100%;
    max-width: 850px;
    aspect-ratio: 16 / 9;
    margin: 2.5rem auto;
    overflow: hidden;
    border-radius: 8px;
  }

  .project-video iframe {
    width: 100%;
    height: 100%;
    border: 0;
  }

  .project-links {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 0.75rem;
    margin: 0 auto 2.5rem;
    }
    
  .project-link-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.45rem;
    padding: 0.55rem 1rem;
    border: 1px solid var(--global-theme-color);
    border-radius: 6px;
    color: var(--global-theme-color);
    background: transparent;
    font-size: 0.95rem;
    font-weight: 500;
    text-decoration: none;
    transition:
    background-color 0.2s ease,
    color 0.2s ease,
    transform 0.2s ease;
    }
    
  .project-link-button:hover {
    color: #ffffff;
    background-color: var(--global-theme-color);
    text-decoration: none;
    transform: translateY(-1px);
    }
    
  .project-link-button i {
    font-size: 1rem;
    }

---

<div class="project-links">
  <a
    class="project-link-button"
    href="{{ '/assets/pdf/vashisth2026move.pdf' | relative_url }}"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Open CoReLIN PDF"
  >
    <i class="fa-solid fa-file-pdf" aria-hidden="true"></i>
    <span>PDF</span>
  </a>

  <a
    class="project-link-button"
    href="https://github.com/IDEAS-Lab-Purdue/CoReLIN/tree/main/DATASET"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Open CoReLIN dataset"
  >
    <i class="fa-solid fa-database" aria-hidden="true"></i>
    <span>Dataset</span>
  </a>

  <a
    class="project-link-button"
    href="https://github.com/IDEAS-Lab-Purdue/CoReLIN"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Open CoReLIN GitHub repository"
  >
    <i class="fa-brands fa-github" aria-hidden="true"></i>
    <span>GitHub</span>
  </a>
</div>

<div class="project-video">
  <iframe
    src="https://www.youtube-nocookie.com/embed/zeKxXmRHS-A"
    title="CoReLIN real-robot experiment video"
    loading="lazy"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
  ></iframe>
</div>

<h2 class="project-section-title">Abstract</h2>

<p class="project-text">
Robot navigation typically assumes an obstacle-free path
exists between start and goal. In real environments, however, clutter
may block all routes. We introduce Lifelong Interactive Navigation,
where a mobile robot with manipulation capabilities must move objects
to forge paths and complete sequential object-placement tasks. Because
environment modifications persist, decisions impact future navigability
and task difficulty. We propose CoReLIN, an LLM-driven constraint-
based reasoning framework with active perception. CoReLIN reasons
over a structured scene graph to decide which objects to relocate, where
to place them, and where to explore next. A standard motion planner ex-
ecutes reliable navigation and manipulation primitives. To evaluate long-
horizon behavior, we introduce 2 new metrics - Long-term Efficiency
Score (LES), a unified metric capturing success, execution efficiency,
environment optimality, captured by Price of Clutter. In ProcTHOR-
10k, CoReLIN outperforms best baseline by 16% under standard metrics
and LES, and transfers to real-world hardware.
</p>

<h2 class="project-section-title">Overview</h2>

<img
  class="project-image"
  src="{{ '/assets/pdf/corelin_overview.pdf' | relative_url }}"
  alt="Overview of the CoReLIN framework"
/>

<p class="project-text">
Overview of our constraint-based planning framework for interactive navigation. At each timestep, our agent receives observations from the environment, which are utilized by our perception module to update the scene graph. Our scene graph contains the observed objects of the environment as nodes and the blocking relation among them as edges. Each node has its own attributes, which provide additional navigability and manipulability context to the LLM. The LLM then decides whether to explore the environment further to collect additional information or to attempt to complete the given task based on the scene graph content and the environment constraints.
</p>

<h2 class="project-section-title">Results</h2>

<img
  class="project-image"
  src="{{ '/assets/img/corelin_results.png' | relative_url }}"
  alt="Experimental results for CoReLIN"
/>

<p class="project-text">
Baseline comparison of our approach CoReLIN with other methods across different floorplans (rooms 1 through 10) and varying episode horizons g={10,15,20} (where g is the total number of tasks per episode). Bold indicates best performing method and underline indicates second-best performing approach.
</p>

