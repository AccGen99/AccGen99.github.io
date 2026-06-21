---
layout: page
title: Scalable Multi-Robot Informative Path Planning for Target Mapping via Deep Reinforcement Learning
description: Scalable Multi-Robot Informative Path Planning for Target Mapping via Deep Reinforcement Learning
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

  .project-authors {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    column-gap: 0.45rem;
    row-gap: 0.3rem;
    margin: -0.25rem auto 1.25rem;
    text-align: center;
    font-size: 1rem;
    line-height: 1.6;
    }
    
  .project-authors a {
    color: var(--global-theme-color);
    font-weight: 400;
    text-decoration: none;
    }
    
  .project-authors a:hover {
    text-decoration: underline;
    }
    
  .author-separator {
    color: var(--global-text-color-light);
    }

  .bibtex-box {
    max-width: 850px;
    margin: 1.25rem auto 3rem;
    padding: 1.25rem;
    overflow-x: auto;
    border: 1px solid var(--global-divider-color, rgba(127, 127, 127, 0.25));
    border-radius: 8px;
    background-color: var(--global-code-bg-color, rgba(127, 127, 127, 0.08));
    text-align: left;
    }
    
  .bibtex-box code {
    display: block;
    padding: 0;
    background: transparent;
    color: var(--global-text-color);
    font-size: 0.88rem;
    line-height: 1.6;
    white-space: pre;
    }


---

<div class="project-authors">
  <a
    href="{{ '/' | relative_url }}"
    aria-label="Apoorva Vashisth's profile"
  >
    Apoorva Vashisth
  </a>

  <span class="author-separator">&middot;</span>

  <a
    href="https://manavkulshrestha.github.io/"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Manav Kulshrestha's profile"
  >
    Manav Kulshrestha
  </a>

  <span class="author-separator">&middot;</span>

  <a
    href="https://scholar.google.com/citations?user=laN6vmAAAAAJ&hl=en"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Damon Conover's profile"
  >
    Damon Conover
  </a>

  <span class="author-separator">&middot;</span>

  <a
    href="https://www.marmotlab.org/bio.html"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Guillaume Sartoretti's profile"
  >
    Guillaume Sartoretti
  </a>

  <span class="author-separator">&middot;</span>

  <a
    href="https://www.cs.purdue.edu/homes/ab/"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Aniket Bera's profile"
  >
    Aniket Bera
  </a>
</div>

<div class="project-links">
  <a
    class="project-link-button"
    href="{{ '/assets/pdf/vashisth2026scalable.pdf' | relative_url }}"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Open MRIPP PDF"
  >
    <i class="fa-solid fa-file-pdf" aria-hidden="true"></i>
    <span>PDF</span>
  </a>

  <a
    class="project-link-button"
    href="https://github.com/AccGen99/marl_ipp"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Open GitHub repository"
  >
    <i class="fa-brands fa-github" aria-hidden="true"></i>
    <span>GitHub</span>
  </a>
</div>

<div class="project-video">
  <iframe
    src="https://www.youtube-nocookie.com/embed/VxzqdquyzqY?autoplay=1&playsinline=1"
    title="Overview of our approach along with simulation videos and real robot experiments"
    loading="eager"
    allow="autoplay; encrypted-media; picture-in-picture; fullscreen"
    allowfullscreen
  ></iframe>
</div>

<h2 class="project-section-title">Abstract</h2>

<p class="project-text">
Autonomous robots are widely utilized for mapping and exploration tasks due to their cost-effectiveness. Multi-robot systems offer scalability and efficiency, especially in terms of the number of robots deployed in more complex environments. These tasks belong to the set of Multi-Robot Informative Path Planning (MRIPP) problems. In this paper, we propose a deep reinforcement learning approach for the MRIPP problem.
We aim to maximize the number of discovered stationary targets in an unknown 3D environment while operating under resource constraints (such as path length). Here, each robot aims to maximize discovered targets, avoid unknown static obstacles, and prevent inter-robot collisions while operating under communication and resource constraints. We utilize the centralized training and decentralized execution paradigm to train a single policy neural network. A key aspect of our approach is our coordination graph that prioritizes visiting regions not yet explored by other robots. Our learned policy can be copied onto any number of robots for deployment in more complex environments not seen during training. Our approach outperforms state-of-the-art approaches by at least 26.2% in terms of the number of discovered targets while requiring a planning time of less than 2 sec per step. We present results for more complex environments with up to 64 robots and compare success rates against baseline planners.
</p>

<h2 class="project-section-title">Overview</h2>

<img
  class="project-image"
  src="{{ '/assets/pdf/mripp_overview.pdf' | relative_url }}"
  alt="Overview of our approach"
/>

<p class="project-text">
Overview of our deep reinforcement learning approach for the multi-robot informative path planning problem. At each time-step, our approach samples collision-free candidate actions in the robot's local region. Our coordination graph associates each candidate action with a utility value, the uncertainty of the utility value, and the exploration features modeling the regions visited by other robots. Our policy network relies on these features to output the robot's state value and the next action to execute, leading to the generation of reward and observations from the environment. Here, the black arrows indicate the robot control loop, green arrows and green boxes are the variables stored in the experience buffer for on-policy training of our policy network. 
</p>

<h2 class="project-section-title">Results</h2>

<img
  class="project-image"
  src="{{ '/assets/pdf/mripp_results.pdf' | relative_url }}"
  alt="Experimental results for our approach"
/>

<p class="project-text">
Comparison of our approach with other baselines in an urban environment. Our performance metric is the percentage of targets discovered during the episode. The solid lines represent the mean values across 250 trials, while the shaded areas denote the standard deviations.
</p>

<h2 class="project-section-title">Cite</h2>

<pre class="bibtex-box"><code>@article{vashisth2026scalable,
  title     = {Scalable Multi-Robot Informative Path Planning for Target Mapping via Deep Reinforcement Learning},
  author    = {Vashisth, Apoorva and
               Kulshrestha, Manav and
               Conover, Damon and
               Bera, Aniket},
  journal   = {IEEE Robotics and Automation Letters},
  year      = {2026},
  publisher = {IEEE}
}</code></pre>
