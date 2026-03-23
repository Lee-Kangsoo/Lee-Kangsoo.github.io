---
layout: default
title: Home
---

<section class="hero">
  <p class="hero__eyebrow">AI Engineer · Computer Vision · Generative AI</p>
  <h1>Kangsoo Lee</h1>
  <p class="hero__body">
    Bridging real-time perception systems and generative AI for real-world applications.
    7년 이상 컴퓨터 비전과 생성형 AI를 다루며, 실시간 인지 시스템과 diffusion 기반 생성 모델을 함께 설계해 왔습니다.
  </p>
  <div class="hero__facts">
    <span>7+ years experience</span>
    <span>BEV · Sensor Fusion · Diffusion</span>
    <span>C/C++ · Python · Docker · Kubernetes</span>
  </div>
  <div class="hero__actions">
    <a class="button button--primary" href="mailto:leeks733@naver.com">Email</a>
    <a class="button button--ghost" href="https://github.com/Lee-Kangsoo">GitHub</a>
    <a class="button button--ghost" href="https://www.linkedin.com/in/kang-soo-lee-b48563192/">LinkedIn</a>
  </div>
</section>

<section class="section-grid section-grid--compact">
  <article class="panel">
    <p class="panel__label">Current Focus</p>
    <h2>Perception + Generative AI</h2>
    <p>실시간 perception 시스템과 controllable image generation을 연결해 실제 문제에 적용하는 일을 하고 있습니다.</p>
  </article>
  <article class="panel">
    <p class="panel__label">Strength</p>
    <h2>System-Oriented AI Engineering</h2>
    <p>모델 성능만이 아니라 latency, memory, deployment constraints까지 함께 보는 쪽에 강점이 있습니다.</p>
  </article>
  <article class="panel">
    <p class="panel__label">Domain</p>
    <h2>Autonomous Driving to GenAI</h2>
    <p>Lane tracking, parking detection, BEV, ego-motion, synthetic data generation까지 이어지는 경험을 갖고 있습니다.</p>
  </article>
</section>

<section class="resume-section">
  <div class="section-heading">
    <p class="section-heading__eyebrow">Professional Summary</p>
    <h2>What I Work On</h2>
  </div>
  <div class="statement-card">
    <p>
      AI Engineer with 7+ years of experience in computer vision and generative AI.
      Specialized in real-time perception systems, BEV transformation, sensor fusion, and diffusion-based image generation.
      I focus on translating strong research ideas into robust production-ready systems.
    </p>
  </div>
</section>

<section class="resume-section">
  <div class="section-heading">
    <p class="section-heading__eyebrow">Core Competencies</p>
    <h2>Technical Areas</h2>
  </div>
  <div class="skill-grid">
    <article class="panel">
      <p class="panel__label">Computer Vision & 3D AI</p>
      <h2>Perception Systems</h2>
      <p>Lane tracking, parking detection, BEV transformation, ego-motion estimation, sensor fusion.</p>
    </article>
    <article class="panel">
      <p class="panel__label">Generative AI</p>
      <h2>Diffusion and Control</h2>
      <p>Stable Diffusion, LoRA, ControlNet, VLM-guided training, synthetic data generation pipelines.</p>
    </article>
    <article class="panel">
      <p class="panel__label">Engineering</p>
      <h2>Implementation</h2>
      <p>C/C++, Python, real-time optimization, Docker, Kubernetes, deployable AI system design.</p>
    </article>
  </div>
</section>

<section class="resume-section">
  <div class="section-heading">
    <p class="section-heading__eyebrow">Experience</p>
    <h2>Selected Roles</h2>
  </div>
  <div class="timeline">
    <article class="timeline-item">
      <div class="timeline-item__meta">Apr.2022 - Present</div>
      <div class="timeline-item__body">
        <h3>GenGenAI</h3>
        <p class="timeline-item__role">AI Engineer · Generative AI</p>
        <p>Designed diffusion-based synthetic data pipelines, built CycleGAN ISP simulation, developed transformer-based BEV segmentation, generated IR datasets, and integrated VLM guidance into diffusion training.</p>
      </div>
    </article>
    <article class="timeline-item">
      <div class="timeline-item__meta">Mar.2019 - Mar.2022</div>
      <div class="timeline-item__body">
        <h3>StradVision</h3>
        <p class="timeline-item__role">Computer Vision Engineer</p>
        <p>Built real-time lane tracking, parking detection, ego-motion estimation, and 4-view BEV transformation pipelines while improving least squares computation by about 10x and reducing runtime memory overhead.</p>
      </div>
    </article>
    <article class="timeline-item">
      <div class="timeline-item__meta">Mar.2017 - Feb.2019</div>
      <div class="timeline-item__body">
        <h3>Chungbuk National University</h3>
        <p class="timeline-item__role">Graduate Researcher</p>
        <p>Worked on camera, LiDAR, and radar sensor fusion for detection and tracking, including Kalman filter-based tracking and LiDAR perception with RANSAC and segmentation.</p>
      </div>
    </article>
  </div>
</section>

<section class="section-grid">
  <article class="panel">
    <p class="panel__label">Awards</p>
    <h2>Recognition</h2>
    <p>1st Place in an Autonomous Driving Competition, additional autonomous driving award, and Academic Excellence Award at Chungbuk National University.</p>
  </article>
  <article class="panel">
    <p class="panel__label">Certification</p>
    <h2>Functional Safety Engineer</h2>
    <p>TUV Rheinland certified in ISO 26262 functional safety with ASIL-oriented system understanding.</p>
  </article>
  <article class="panel">
    <p class="panel__label">Education</p>
    <h2>M.S. and B.S. at CBNU</h2>
    <p>M.S. in Control and Robotics Engineering, B.S. in Electronics Engineering, with strong academic performance including rank 1st out of 113.</p>
  </article>
</section>

<section class="recent-posts" id="recent-posts">
  <div class="section-heading">
    <p class="section-heading__eyebrow">Writing</p>
    <h2>Recent Notes</h2>
  </div>
  {% assign recent_posts = site.posts | slice: 0, 4 %}
  {% if recent_posts.size > 0 %}
    <div class="post-cards">
      {% for post in recent_posts %}
        <article class="post-card">
          <p class="post-card__meta">{{ post.date | date: "%Y.%m.%d" }}{% if post.categories.size > 0 %} · {{ post.categories | join: ", " }}{% endif %}</p>
          <h3><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h3>
          {% if post.excerpt %}
            <p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
          {% endif %}
        </article>
      {% endfor %}
    </div>
  {% else %}
    <div class="empty-state">
      <p>기술 노트가 아직 많지는 않지만, 이후 이력서 기반 경험과 연결되는 기록을 계속 쌓아갈 예정입니다.</p>
    </div>
  {% endif %}
</section>
