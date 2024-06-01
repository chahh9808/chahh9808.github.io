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
  - block: collection
    id: news
    content:
      title: News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      # view: citation
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 7, 0]


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
    content:
      title: '📚 News'
      subtitle: ''
      text: |-
        <ul>
          <li>Apr. 2024 <span class="icon">📚</span> Technical Programm Committee at FairComp @ UbiComp/ISWC '24</li>
          <li>Mar. 2024 <span class="icon">📚</span> Technical Programm Committee at UbiComp/ISWC '24</li>
          <li>Mar. 2024 <span class="icon">📚</span> Artifact Evaluation Committee at ACM MobiSys '24</li>
          <li>Mar. 2024 <span class="icon">📚</span> Visiting Scholar at the <a href="https://www.cam.ac.uk/">University of Cambridge</a>, Cambridge, UK</li>
          <li>Feb. 2024 <span class="icon">📝</span> Paper accepted at CVPR '24</li>
          <li>Jan. 2024 <span class="icon">🎤</span> <a href="https://hsn.org/">Session Speaker at HSN '24</a></li>
          <li>Dec. 2023 <span class="icon">✈️</span> NeurIPS '23 @ New Orleans, LA (Dec. 10 - Dec. 15)</li>
          <li>Oct. 2023 <span class="icon">📝</span> Paper accepted at ACM UbiComp '24</li>
          <li>Oct. 2023 <span class="icon">🎤</span> <a href="https://ictc.org/">Special Session Speaker at ICTC '23</a></li>
          <li>Oct. 2023 <span class="icon">✈️</span> UbiComp '23 @ Cancun, Mexico (Oct. 8 - 12)</li>
          <li>Sep. 2023 <span class="icon">📝</span> Paper accepted at NeurIPS '23</li>
          <li>Aug. 2023 <span class="icon">📚</span> Artifact Evaluation Committee at ACM MobiCom '23</li>
          <li>Jun. 2023 <span class="icon">📚</span> Full-time Research Scientist at <a href="https://www.bell-labs.com/">Nokia Bell Labs</a>, Cambridge, UK</li>
          <li>May. 2023 <span class="icon">📝</span> Paper accepted at INTERSPEECH '23</li>
          <li>Apr. 2023 <span class="icon">📝</span> Paper accepted at ACM UbiComp '23</li>
          <li>Feb. 2023 <span class="icon">🏆</span> Best Ph.D. Dissertation Award from KAIST College of Engineering</li>
          <li>Feb. 2023 <span class="icon">🏆</span> Best Ph.D. Dissertation Award from KAIST School of Computing</li>
          <li>Jan. 2023 <span class="icon">🌟</span> <a href="https://aics.ee/">AI/CS/EE Rising Stars</a></li>
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
