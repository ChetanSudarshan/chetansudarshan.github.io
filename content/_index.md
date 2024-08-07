---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: hero
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: Hugo Academic Theme
      image:
        filename: hero-academic.png
      cta:
        label: '**Get Started**'
        url: https://hugoblox.com/templates/
      cta_alt:
        label: Ask a question
        url: https://discord.gg/z8wNYzb
      cta_note:
        label: >-
          <div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star Hugo Blox Builder</a></div><div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/theme-academic-cv" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star the Academic template</a></div>
      text: |-
        **Generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 500,000+ sites.**

        **Easily build anything with blocks - no-code required!**

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true
  - block: about.biography
    id: about
    content:
      title: About me
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  #- block: skills
  #  content:
  #    title: Skills
  #    text: ''
  #    # Choose a user to display skills from (a folder name within `content/authors/`)
  #    username: admin
  #  design:
  #    columns: '1'
  #C- block: experience
  #C  content:
  #C    title: Experience
  #C    # Date format for experience
  #C    #   Refer to https://docs.hugoblox.com/customization/#date-format
  #C    date_format: Jan 2006
  #C    # Experiences.
  #C    #   Add/remove as many `experience` items below as you like.
  #C    #   Required fields are `title`, `company`, and `date_start`.
  #C    #   Leave `date_end` empty if it's your current employer.
  #C    #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #C    items:
  #C      - title: CEO
  #C        company: GenCoin
  #C        company_url: ''
  #C        company_logo: org-gc
  #C        location: California
  #C        date_start: '2021-01-01'
  #C        date_end: ''
  #C        description: |2-
  #C            Responsibilities include:
  #C
  #C            * Analysing
  #C            * Modelling
  #C            * Deploying
  #C      - title: Professor of Semiconductor Physics
  #C        company: University X
  #C        company_url: ''
  #C        company_logo: org-x
  #C        location: California
  #C        date_start: '2016-01-01'
  #C        date_end: '2020-12-31'
  #C        description: Taught electronic engineering and researched semiconductor physics.
  #C  design:
  #C    columns: '2'
  #C - block: accomplishments
  #C   content:
  #C     # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
  #C     title: 'Accomplish&shy;ments'
  #C     subtitle:
  #C     # Date format: https://docs.hugoblox.com/customization/#date-format
  #C     date_format: Jan 2006
  #C     # Accomplishments.
  #C     #   Add/remove as many `item` blocks below as you like.
  #C     #   `title`, `organization`, and `date_start` are the required parameters.
  #C     #   Leave other parameters empty if not required.
  #C     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #C     items:
  #C       - certificate_url: https://www.coursera.org
  #C         date_end: ''
  #C         date_start: '2021-01-25'
  #C         description: ''
  #C         icon: coursera
  #C         organization: Coursera
  #C         organization_url: https://www.coursera.org
  #C         title: Neural Networks and Deep Learning
  #C         url: ''
  #C       - certificate_url: https://www.edx.org
  #C         date_end: ''
  #C         date_start: '2021-01-01'
  #C         description: Formulated informed blockchain models, hypotheses, and use cases.
  #C         icon: edx
  #C         organization: edX
  #C         organization_url: https://www.edx.org
  #C         title: Blockchain Fundamentals
  #C         url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
  #C       - certificate_url: https://www.datacamp.com
  #C         date_end: '2020-12-21'
  #C         date_start: '2020-07-01'
  #C         description: ''
  #C         icon: datacamp
  #C         organization: DataCamp
  #C         organization_url: https://www.datacamp.com
  #C         title: 'Object-Oriented Programming in R'
  #C         url: ''
  #C   design:
  #C     columns: '2'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      columns: '2'
      view: citation
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Sustainable Computing
          tag: Sustainable Computing
        #- name: Other
        #  tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  #C- block: collection
  #C  id: talks
  #C  content:
  #C    title: Recent & Upcoming Talks
  #C    filters:
  #C      folders:
  #C        - event
  #C  design:
  #C    columns: '2'
  #C    view: compact
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
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
      view: compact
      columns: '2'
 
  #C- block: markdown
  #C  content:
  #C    title: Gallery
  #C    subtitle: ''
  #C    text: |-
  #C      {{< gallery album="demo" >}}
  #C  design:
  #C    columns: '1'


  #C - block: tag_cloud
  #C   content:
  #C    title: Popular Topics
  #C  design:
  #C    columns: '2'
  #C- block: contact
  #C  id: contact
  #C  content:
  #C    title: Contact
  #C    subtitle:
  #C    text: |-
  #C      Feel free to contact me for collaborations or to discuss my research !!
      # Contact (add or remove contact options as necessary)
      #C email: cchoppal@asu.edu
      #C phone: 
      #C appointment_url: 'https://calendly.com'
      #C address:
      #C   street: 781 S Terrace Rd
      #C   city: Tempe
      #C   region: AZ
      #C   postcode: '85281'
      #C   country: United States
      #C   country_code: US
      #directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      #office_hours:
      #  - 'Monday 10:00 to 13:00'
      #  - 'Wednesday 09:00 to 10:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      #C coordinates:
      #C   latitude: '33.418339034099446'
      #C   longitude: '-111.928423120922'  
#C      contact_links:
#C        - icon: at-symbol
#C          url: 'mailto:cchoppal@asu.com'
#C          label: E-mail Me
#C        - icon: twitter
#C          icon_pack: fab
#C          name: DM Me
#C          link: 'https://twitter.com/ChetanSudarshan'
        #C - icon: skype
        #C   icon_pack: fab
        #C   name: Skype Me
        #C   link: 'skype:echo123?call'
        #C - icon: video
        #C   icon_pack: fas
        #C   name: Zoom Me
        #C   link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      #C# Email form provider
      #Cform:
      #C  provider: netlify
      #C  formspree:
      #C    id:
      #C  netlify:
      #C    # Enable CAPTCHA challenge to reduce spam?
      #C    captcha: true
#C    design:
#C      columns: '2'
---
