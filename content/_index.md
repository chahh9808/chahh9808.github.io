---
title: ""
date: 2022-10-24
type: landing

design:
  spacing: "4rem"

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: ""
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: monochrome-hero

  - block: news
    id: news
    content:
      title: 'News'
      count: 10
      items:
        - date: 'Apr. 2026'
          icon: '✈️'
          text: >-
            ICLR '26 @ Rio de Janeiro, Brazil (Apr. 23 - 27)
        - date: 'Feb. 2026'
          icon: '🌟'
          text: >-
            Won Stars of Tomorrow award at Microsoft Research Asia
        - date: 'Jan. 2026'
          icon: '🌟'
          text: >-
            Invited Talk at <a href="https://hyperconnect.com/en/">Hyperconnect AI</a> (Thesis: TTA for Clients)
        - date: 'Jan. 2026'
          icon: '📝'
          text: >-
            Our paper 'Beyond Hearing' is accepted at ICLR '26
        - date: 'Nov. 2025'
          icon: '🌟'
          text: >-
            Won First Place at Microsoft Global Hackathon 2025
        - date: 'Oct. 2025'
          icon: '📝'
          text: >-
            First author paper 'SNAP' is accepted at NeurIPS '25
        - date: 'Jul. 2025'
          icon: '📚'
          text: >-
            Research Internship at <a href="https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/">Microsoft Research Asia</a>, Shanghai, China
        - date: 'Mar. 2025'
          icon: '📝'
          text: >-
            Our paper 'From Vision to Motion' is accepted at IEEE TMC
        - date: 'Jan. 2025'
          icon: '🌟'
          text: >-
            Received Inseong (Character) Scholarship at KAIST
        - date: 'Jun. 2024'
          icon: '✈️'
          text: >-
            MobiSys '24 @ Tokyo, Japan (Jun. 3 - 7)
        - date: 'Jun. 2024'
          icon: '🌟'
          text: >-
            Graduate Student Council President of KAIST EE
        - date: 'Apr. 2024'
          icon: '📝'
          text: >-
            First author poster 'TESLA' accepted at MobiSys '24
        - date: 'Aug. 2023'
          icon: '📝'
          text: >-
            Submitted paper 'Sherlock'
        - date: 'Mar. 2022'
          icon: '📚'
          text: >-
            Joined Mobile Intelligence & Interaction Lab at KAIST
        - date: 'Feb. 2022'
          icon: '📚'
          text: >-
            Received B.S. degree at KAIST with Magna Cum Laude
        - date: 'Aug. 2020'
          icon: '📚'
          text: >-
            Research Internship (Team leader) at <a href="https://inbodyusa.com/">InBody.co.</a>, Seoul, Korea
  - block: collection
    id: projects
    content:
      title: Projects
      text: ""
      count: 0
      filters:
        folders:
          - post
        exclude_featured: false
    design:
      view: project-list
  - block: collection
    id: papers
    content:
      title: Publications
      text: ""
      count: 0
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: markdown
    id: professional-experience
    content:
      title: Professional Experiences
      text: |
        <div class="experience-section">
          <p><strong>07/2025 – 01/2026</strong></p>
          <h3>Microsoft Research Asia, Wireless Communication and Sensing Group (Mentor: <a href="https://www.cs.utexas.edu/~lili/">Lili Qiu</a>)</h3>
          <p>Research Intern</p>
          <p class="location">Shanghai, China</p>
        
          <p><strong>02/2021 – 02/2022</strong></p>
          <h3>KAIST, Mobile Intelligence & Interaction Lab</h3>
          <p>Undergraduate Research Intern</p>
          <p class="location">Daejeon, Republic of Korea</p>

          <p><strong>02/2020 – 08/2020</strong></p>
          <h3>InBody Co., Future Innovation Team</h3>
          <p>Research Intern</p>
          <p class="location">Seoul, Republic of Korea</p>

          <p><strong>08/2019 – 09/2019</strong></p>
          <h3>KAIST, Smart and Mobile System Lab</h3>
          <p>Individual Research Intern</p>
          <p class="location">Daejeon, Republic of Korea</p>
        </div>

  - block: markdown
    id: leadership-experience
    content:
      title: Leadership Experiences
      text: |
        <div class="leadership-section">
          <p><strong>2024 – 2024</strong></p>
          <h3>Graduate Student Council President</h3>
          <p>KAIST School of Electrical Engineering</p>

          <p><strong>2020 – 2020</strong></p>
          <h3>Team Leader</h3>
          <p>InBody Co., Future Innovation Team</p>

          <p><strong>2018 – 2019</strong></p>
          <h3>Undergraduate Student Council President</h3>
          <p>KAIST School of Electrical Engineering</p>

          <p><strong>2018 – 2019</strong></p>
          <h3>Freshman Program Designer</h3>
          <p>Korea Advanced Institute of Science and Technology</p>
          <p>Design and operate special classes and programs for KAIST freshmen</p>
        </div>

  - block: markdown
    id: honors
    content:
      title: Honors
      text: |
        <div class="awards-section">
          <p><strong>2026</strong></p>
          <h3>Stars of Tomorrow Award</h3>
          <p>Microsoft Research Asia</p>

          <p><strong>2022</strong></p>
          <h3>Magna Cum Laude</h3>
          <p>Korea Advanced Institute of Science and Technology</p>

          <p><strong>2019</strong></p>
          <h3>Noyeop Cultural Foundation Scholarship</h3>
          <p>Noyeop Cultural Foundation</p>
          <p>One person per department, provided until graduation</p>

          <p><strong>2017</strong></p>
          <h3>Dean's list</h3>
          <p>Korea Advanced Institute of Science and Technology</p>
          <p>Outstanding student in the department</p>
        </div>

  - block: markdown
    id: skills
    content:
      title: Skills
      text: |
        <div class="skills-section">
          <p><span class="skill-category">Programming</span> — Python, C, C++, Java</p>
          <p><span class="skill-category">Machine Learning</span> — Pytorch, Tensorflow, Tensorflow Lite</p>
          <p><span class="skill-category">Hardware Prototyping</span> — Arduino, RaspberryPi, Qorvo</p>
          <p><span class="skill-category">Network Simulation</span> — NS3 simulator</p>
        </div>

---
