---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    content:
      title: Skills
      items:
        - name: R
          description: 100%
          icon: r-project
          icon_pack: fab
        - name: Statistics
          description: 100%
          icon: chart-line
          icon_pack: fas
        - name: Python
          description: 100% 
          icon: camera-retro
          icon_pack: fas
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Graduate Professional Asssistant
          company: Purdue University
          company_url: ''
          company_logo: org-gc
          location: West Lafayette, IN, USA
          date_start: '2023-06-22'
          date_end: ''
          description: |2-
              Responsibilities include:
              * Public Relations 
              * Strategic Communication
        - title: Graduate Research Assistant
          company: Purdue University
          company_url: ''
          company_logo: org-x
          location: West Lafayette, IN, USA
          date_start: '2023-06-22'
          date_end: ''
          description: |2-
              Responsibilities include:
              * Write Code for a Google Funded Project
              * Write Publications
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.coursera.org/account/accomplishments/specialization/certificate/ZWTWTRAE6GUV
          date_end: ''
          date_start: '2019-09-30'
          description: Modules include Neural Networks and Deep Learning, Improving Deep Neural Networks with Hyperparameter Tuning, Regularization and Optimization, Structuring Machine Learning Projects, Convolutional Neural Networks, Sequence Models. 
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Deep Learning
          url: https://www.coursera.org/account/accomplishments/specialization/certificate/ZWTWTRAE6GUV
        - certificate_url: https://www.coursera.org/account/accomplishments/specialization/certificate/G3JGQU7DNH4L
          date_end: ''
          date_start: '2019-07-30'
          description: Modules include Machine Learning Foundations with A Case Study Approach, Machine Learning with Regression, Machine Learning with Classification, Machine Learning with Clustering and Retrieval. 
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Machine Learning
          url: https://www.coursera.org/account/accomplishments/specialization/certificate/G3JGQU7DNH4L
    design:
      columns: '2'
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
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
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
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        I am always open to collaborations and exciting opportunities. 
      # Contact (add or remove contact options as necessary)
      email: jcheoh@purdue.edu
      appointment_url: 'https://calendly.com'
      address:
        city: West Lafayette
        region: IN
        postcode: '47906'
        country: United States
        country_code: US
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/jialincheoh'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
