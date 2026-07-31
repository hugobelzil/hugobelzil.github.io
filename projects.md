---
title: Projects
subtitle: Selected computational mathematics and quantitative finance projects.
permalink: /projects/
wide: true
math: true
---

<section class="projects-list" aria-label="Selected projects">
  <article class="project-entry project-entry--brief">
    <figure class="project-figure project-figure--merton">
      <img src="{{ '/assets/img/projects/merton-training-curves.png' | relative_url }}" alt="Merton fixed-policy critic training summary" loading="lazy">
    </figure>
    <div class="project-copy">
      <p class="project-meta">ETH Zürich - Advanced ML - May 2026</p>
      <h2>Merton-ctrl: Temporal-Difference Methods for the Merton Problem</h2>
      <p>
        A collaborative implementation of the continuous-time Merton consumption-investment problem, comparing TD, differential TD (dTD), and beta-dTD value critics against the closed-form solution.
      </p>
      <p class="project-links">
        <a href="https://github.com/hugobelzil/Merton-ctrl">GitHub repository</a>
        <a href="{{ '/assets/reports/continuous-time-rl-report.pdf' | relative_url }}">Consult the report</a>
      </p>
    </div>
  </article>

  <article class="project-entry">
    <figure class="project-figure project-figure--eikonal">
      <div class="project-image-crop">
        <img src="{{ '/assets/img/projects/eikonal-path-planning.png' | relative_url }}" alt="Optimal Eikonal path planning around obstacles and corresponding solution surface" loading="lazy">
      </div>
    </figure>
    <div class="project-copy">
      <p class="project-meta">MATH 478 - Computational Methods for Applied Mathematics - APR 2025</p>
      <h2>The Fast-Sweeping Method for Eikonal Equations and an Application to Optimal Control</h2>
      <p>
        This project studies numerical methods for two-dimensional Eikonal equations and uses the resulting value functions for optimal path planning. The fast-sweeping method is implemented in Python and tested on distance functions, variable-speed media, light refraction through Snell's law, and obstacle-avoidance examples.
      </p>
      <div class="project-equation">
        $$
        \begin{cases}
        |\nabla u(x,y)| = f(x,y), & (x,y)\in\Omega,\\
        u(x,y)=\phi(x,y), & (x,y)\in\Gamma.
        \end{cases}
        $$
      </div>
      <p>
        Once the solution \(u\) is computed, optimal paths are recovered by backtracking along the descent direction,
        $$\dot X(t)=-\nabla u(X(t)).$$
      </p>
      <p class="project-links">
        <a href="{{ '/assets/reports/eikonal-project.pdf' | relative_url }}">Final report PDF</a>
        <a href="https://github.com/hugobelzil/eikonal_project">GitHub repository</a>
      </p>
    </div>
  </article>

  <article class="project-entry project-entry--reverse">
    <figure class="project-figure project-figure--garch">
      <div class="project-image-crop">
        <img src="{{ '/assets/img/projects/garch-volatility-clustering.png' | relative_url }}" alt="Daily log-return plot showing volatility clustering" loading="lazy">
      </div>
    </figure>
    <div class="project-copy">
      <p class="project-meta">MATH 598 - Extreme Value Analysis - DEC 2024</p>
      <h2>Analysis of Financial Data: Investigation of GARCH(1,1) Models on the Dow Jones Index and Extreme Value Results</h2>
      <p>
        This project investigates the tail behavior and extreme value properties of GARCH(1,1) models, with a focus on financial return series where volatility clusters over time and extreme events dominate risk. The work combines theoretical tail-index calculations with numerical experiments and an application to Dow Jones daily log-returns.
      </p>
      <div class="project-equation">
        $$
        X_t=\sigma_t Z_t,\qquad
        \sigma_t^2=\alpha_0+\alpha_1 X_{t-1}^2+\beta_1\sigma_{t-1}^2.
        $$
      </div>
      <p>
        The main numerical task is computing the tail index \(\kappa\), including through the fixed-point equation
        $$\mathbb{E}\left[(\alpha_1 Z_t^2+\beta_1)^{\kappa/2}\right]=1,$$
        and comparing these estimates with the Block Maxima method from Extreme Value Theory.
      </p>
      <p class="project-links">
        <a href="{{ '/assets/reports/evt-garch-final-project-v2.pdf' | relative_url }}">Final report PDF</a>
        <a href="https://github.com/hugobelzil/evt_garch_project">GitHub repository</a>
      </p>
    </div>
  </article>
</section>
