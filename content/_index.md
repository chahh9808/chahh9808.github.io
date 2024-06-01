---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: true
  # - block: collection
  #   id: news
  #   content:
  #     title: News
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     # view: citation
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 7, 0]


  # - block: 'github.juiceleee.news'
  #   id: news
  #   content:
  #     title: News
  #     username: admin
  # - block: 'github.juiceleee.publication'
  #   id: publication
  #   content:
  #     title: Publications
  #     # Choose a user profile to display (a folder name within `content/authors/`)
  #     username: admin
  # - block: 'github.juiceleee.honor'
  #   id: honor
  #   content:
  #     title: Honors
  #     username: admin
  # - block: 'github.juiceleee.project'
  #   id: project
  #   content:
  #     title: Projects
  #     username: admin
  
  - block: markdown
    id: news
    content:
      title: 'News'
      subtitle: ''
      text: |-
        <ul style="font-size: 16px;">
          <li>Jun. 2024 <span class="icon">✈️</span> MobiSys '24 @ Tokyo, Japan (Jun. 3 - 7)</li>
          <li>Jun. 2024 <span class="icon">🌟</span> Graduate Student Council President of KAIST EE</li>
          <li>Apr. 2024 <span class="icon">📝</span> Poster accepted at MobiSys '24</li>
          <li>Feb. 2024 <span class="icon">📝</span> Submitted paper IMG2IMU </li>
          <li>Aug. 2023 <span class="icon">📝</span> Submitted paper Sherlock </li>
          <li>Mar. 2022 <span class="icon">📚</span> Joined Networking & Mobile System Lab at KAIST</li>
          <li>Feb. 2022 <span class="icon">📚</span> Received B.S. degree at KAIST with Magna Cum Laude</li>
          <li>Aug. 2020 <span class="icon">📚</span> Research Internship (Team leader) at <a href="https://inbodyusa.com/">InBody.co.</a>, Seoul, Korea</li>
        </ul>
    design:
      columns: '1'
  # - block: collection
  #   id: papers
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     view: article-grid
  #     columns: 2
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
      view: compact
  - block: collection
    id: papers
    content:
      title: Publications
      text: ""
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
        <style>
          .experience-section {
            border-top: 2px solid #059669;
            padding-top: 10px;
          }
          .experience-section h3 {
            margin: 0;
            font-size: 18px;
            color: #059669;
          }
          .experience-section p {
            margin: 5px 0;
            font-size: 14px;
          }
          .experience-section .location {
            font-style: italic;
            color: gray;
          }
        </style>
        <div class="experience-section">
          <p><strong>02/2021 – 02/2022</strong></p>
          <h3>KAIST, Network and Mobile System Lab</h3>
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
        <style>
          .leadership-section {
            border-top: 2px solid #059669;
            padding-top: 10px;
          }
          .leadership-section h3 {
            margin: 0;
            font-size: 18px;
            color: #059669;
          }
          .leadership-section p {
            margin: 5px 0;
            font-size: 14px;
          }
        </style>
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
          <p>Korea Institute of Science and Technology</p>
          <p>Design and operate special classes and programs for KAIST freshmen</p>
        </div>

  - block: markdown
    id: honors
    content:
      title: Honors
      text: |
        <style>
          .awards-section {
            border-top: 2px solid #059669;
            padding-top: 10px;
          }
          .awards-section h3 {
            margin: 0;
            font-size: 18px;
            color: #059669;
          }
          .awards-section p {
            margin: 5px 0;
            font-size: 14px;
          }
        </style>
        <div class="awards-section">
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
        <style>
          .skills-section {
            border-top: 2px solid #059669;
            padding-top: 10px;
          }
          .skills-section p {
            margin: 5px 0;
            font-size: 14px;
          }
          .skills-section .skill-category {
            font-weight: bold;
          }
        </style>
        <div class="skills-section">
          <p><span class="skill-category">Programming</span> — Python, C, C++, Java</p>
          <p><span class="skill-category">Machine Learning</span> — Pytorch, Tensorflow, Tensorflow Lite</p>
          <p><span class="skill-category">Hardware Prototyping</span> — Arduino, RaspberryPi, Qorvo</p>
          <p><span class="skill-category">Network Simulation</span> — NS3 simulator</p>
        </div>


  # - block: markdown
  #   id: professional-experience
  #   content:
  #     title: PROFESSIONAL EXPERIENCE
  #     text: |
  #       **02/2021 – 02/2022**  
  #       **KAIST, Network and Mobile System Lab**  
  #       *Undergraduate Research Intern*  
  #       Daejeon, Republic of Korea

  #       **02/2020 – 08/2020**  
  #       **InBody Co., Future Innovation Team**  
  #       *Research Intern*  
  #       Seoul, Republic of Korea

  #       **08/2019 – 09/2019**  
  #       **KAIST, Smart and Mobile System Lab**  
  #       *Individual Research Intern*  
  #       Daejeon, Republic of Korea

  # - block: markdown
  #   id: awards-honors
  #   content:
  #     title: AWARDS & HONORS
  #     text: |
  #       **2022**  
  #       **Magna Cum Laude**  
  #       *Korea Advanced Institute of Science and Technology*

  #       **2019**  
  #       **Noyeop Cultural Foundation Scholarship**  
  #       *Noyeop Cultural Foundation*  
  #       One person per department, provided until graduation

  #       **2017**  
  #       **Dean's list**  
  #       *Korea Advanced Institute of Science and Technology*  
  #       Outstanding student in the department

  # - block: markdown
  #   id: leadership-experience
  #   content:
  #     title: LEADERSHIP EXPERIENCE
  #     text: |
  #       **2024 – 2024**  
  #       **Graduate Student Council President**  
  #       *KAIST School of Electrical Engineering*

  #       **2020 – 2020**  
  #       **Team Leader**  
  #       *InBody Co., Future Innovation Team*

  #       **2018 – 2019**  
  #       **Undergraduate Student Council President**  
  #       *KAIST School of Electrical Engineering*

  #       **2018 – 2019**  
  #       **Freshman Program Designer**  
  #       *Korea Institute of Science and Technology*  
  #       Design and operate special classes and programs for KAIST freshmen

  # - block: markdown
  #   id: skills
  #   content:
  #     title: SKILLS
  #     text: |
  #       **Programming** — Python, C, C++, Java  
  #       **Machine Learning** — Pytorch, Tensorflow, Tensorflow Lite  
  #       **Hardware Prototyping** — Arduino, RaspberryPi, Qorvo  
  #       **Network Simulation** — NS3 simulator

  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     view: article-grid
  #     columns: 1
  
  # - block: cta-card
  #   demo: true # Only display this section in the Hugo Blox Builder demo site
  #   content:
  #     title: 👉 Build your own academic website like this
  #     text: |-
  #       This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

  #       <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

  #       Easily build anything with blocks - no-code required!
        
  #       From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
  #     button:
  #       text: Get Started
  #       url: https://hugoblox.com/templates/
  #   design:
  #     card:
  #       # Card background color (CSS class)
  #       css_class: "bg-primary-700"
  #       css_style: ""
---
