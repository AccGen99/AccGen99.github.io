---
layout: page
title: Deep Reinforcement Learning with Dynamic Graphs for Adaptive Informative Path Planning
description: Deep Reinforcement Learning with Dynamic Graphs for Adaptive Informative Path Planning
permalink: /projects/dynagr/
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
    href="https://www.ipb.uni-bonn.de/people/julius-rueckin/index.html"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Julius's profile"
  >
    Julius Rückin
  </a>

  <span class="author-separator">&middot;</span>

  <a
    href="https://www.ipb.uni-bonn.de/people/federico-magistri/"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Federico Magistri's profile"
  >
    Federico Magistri
  </a>

  <span class="author-separator">&middot;</span>

  <a
    href="https://www.ipb.uni-bonn.de/people/cyrill-stachniss/index.html"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Cyrill Stachniss's profile"
  >
    Cyrill Stachniss
  </a>

  <span class="author-separator">&middot;</span>

  <a
    href="https://www.ce.cit.tum.de/en/itr/events/winterschool/marija-popovich/"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Marija Popović's profile"
  >
    Marija Popović
  </a>

</div>

<div class="project-links">
  <a
    class="project-link-button"
    href="{{ '/assets/pdf/vashisth2024deep.pdf' | relative_url }}"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Open PDF"
  >
    <i class="fa-solid fa-file-pdf" aria-hidden="true"></i>
    <span>PDF</span>
  </a>

  <a
    class="project-link-button"
    href="https://github.com/dmar-bonn/ipp-rl-3d"
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
    src="https://www.youtube-nocookie.com/embed/qfCqNXtt2rU?autoplay=1&playsinline=1"
    title="Overview of our approach along with simulation videos and real robot experiments"
    loading="eager"
    allow="autoplay; encrypted-media; picture-in-picture; fullscreen"
    allowfullscreen
  ></iframe>
</div>

<h2 class="project-section-title">Abstract</h2>

<p class="project-text">
Autonomous robots are often employed for data collection due to their efficiency and low labour costs. A key task in robotic data acquisition is planning paths through an initially unknown environment to collect observations given platform-specific resource constraints, such as limited battery life. Adaptive online path planning in 3D environments is challenging due to the large set of valid actions and the presence of unknown occlusions. To address these issues, we propose a novel deep reinforcement learning approach for adaptively replanning robot paths to map targets of interest in unknown 3D environments. A key aspect of our approach is a dynamically constructed graph that restricts planning actions local to the robot, allowing us to react to newly discovered static obstacles and targets of interest. For replanning, we propose a new reward function that balances between exploring the unknown environment and exploiting online-discovered targets of interest. Our experiments show that our method enables more efficient target discovery compared to state-of-the-art learning and non-learning baselines. We also showcase our approach for orchard monitoring using an unmanned aerial vehicle in a photorealistic simulator.
</p>

<h2 class="project-section-title">Overview</h2>

<img
  class="project-image"
  src="{{ '/assets/img/dynagr_overview.png' | relative_url }}"
  alt="Overview of our approach"
/>

<p class="project-text">
At each mission timestep t, our approach samples collision-free waypoints in the robot’s local environment. These waypoints, with considered yaw directions, generate action nodes. Each action node is associated with utility value and uncertainty of the utility value, regressed from the Gaussian process, to generate the dynamic graph. Our actor-critic network uses the dynamic graph to output the robot’s state value and predicts the next action to execute, which generates a reward and observations from the environment. Blue arrows indicate the robot control loop and green indicate variables stored in the experience buffer to train the actor-critic network via on-policy learning.
</p>

<h2 class="project-section-title">Results</h2>

<img
  class="project-image"
  src="{{ '/assets/img/dynagr_base_comp.png' | relative_url }}"
  alt="Experimental results for our approach"
/>

<p class="project-text">
Comparison of our approach against baselines in a UAV-based fruit monitoring scenario. Solid lines indicate means over 500 trials and shaded regions show standard deviations. In our approach, using our exploration-exploitation reward function with a dynamic graph action space for reinforcement learning enables more efficiently discovering targets of interest (fruit) during a mission.
</p>

<img
  class="project-image"
  src="{{ '/assets/img/dynagr_sim_img.png' | relative_url }}"
  alt="Simulation experiment visualization for our approach"
/>

<p class="project-text">
Our reinforcement learning approach for adaptive informative path planning applied in an orchard monitoring scenario using an unmanned aerial vehicle (UAV). Blue squares are candidate waypoints output by our planner, while the green square is the chosen next waypoint to visit. The inset windows show the onboard camera view and semantic segmentation for discovering apples. By planning collision-free paths for the UAV online, we maximise the number of apple fruits discovered under flight-length constraints.
</p>

<h2 class="project-section-title">Cite</h2>

<pre class="bibtex-box"><code>@article{vashisth2024deep,
  title     = {Deep reinforcement learning with dynamic graphs for adaptive informative path planning},
  author    = {Vashisth, Apoorva and
               R{\"u}ckin, Julius and
               Magistri, Federico and
               Stachniss, Cyrill and
               Popovi{\'c}, Marija},
  journal   = {IEEE Robotics and Automation Letters},
  year      = {2024},
  volume    = {9},
  number    = {9},
  pages     = {7747--7754},
  publisher = {IEEE}
}</code></pre>
