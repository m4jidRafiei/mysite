---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
    design:
     columns: '2'    
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
        - title: Data and Process Scientist (PhD Candidate)
          company: RWTH Aachen University
          company_url: www.pads.rwth-aachen.de
          company_logo: rwth
          location: Aachen, Germany
          date_start: '2018-08-01'
          date_end: '2023-11-24'
          description: |2-
              Responsibilities include:

              * Internal lead of the machine learning for process mining project (ML4ProM) at PADS
              * Internal lead of the AI study buddy project (AIStudyBuddy) at PADS
              * Researching on reponsible data science
              * Researching on process-aware data science over SAP focusing on object-centric event data
              * Researching on federated (inter-organizational) process mining
              * Designing and implementing state-of-the-art privacy preservation techniques
              * Teaching on process and data science
        - title: SAP Technical Consultant
          company: NAK - Mobile Company of Iran (MCI)
          company_url: https://www.nak-mci.ir/en
          company_logo: NAK
          location: Tehran, Iran
          date_start: '2015-10-01'
          date_end: '2018-07-30'
          description: |2-
              Responsibilities include:

              * Developing SAP ABAP applications for FI, MM, and SD modules
              * Designing and developing SAP PI/PO projects
              * Designing and developing SAP Fiori apps
        - title: Software Developer
          company: Freelance
          company_logo: freelance
          location: Tehran, Iran
          date_start: '2008-01-01'
          date_end: '2015-01-01'
          description: |2-
              Some projects:

              * Developing a web-based app for user account management (PHP)
              * Developing a database search engine tool (C#)
              * Developing a scheduling system for FMS (C#)
              * Enhancing FileZilla FTP Server by adding new commands (C++)
              * Developing a Gmail reader tool (Perl)
              
    design:
      columns: '2'
  - block: accomplishments
    id: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Awards & Honors'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: ''
          date_end: ''
          date_start: '2011-08-01'
          description: 'University Entrance Exam (Master’s Degree)'
          organization: National Organization of Educational Testing
          organization_url: ''
          title: Among Top 0.05% Students of CS
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2018-12-15'
          description: SIMPDA Conference
          organization: International Symposium on Data-Driven Process Discovery and Analysis (SIMPDA)
          organization_url: ''
          title: Best Paper Award
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2020-05-25'
          description: 'RCIS Conference'
          organization: International Conference on Research Challenges in Information Science (RCIS)
          organization_url: ''
          title: 'Destinguished Paper Award'
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2022-10-05'
          description: 'CoopIS Conference'
          organization: International Conference on Cooperative Information Systems (CoopIS)
          organization_url: ''
          title: 'Best Paper Award Runner-Up'
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2022-10-25'
          description: 'The RPM Workshop of ICPM Conference'
          organization: International Conference on Process Mining (ICPM) - Workshop on Responsible Process Mining (RPM) 
          organization_url: ''
          title: 'Best Paper Award'
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2023-10-23'
          description: 'The EduPM Workshop of ICPM Conference'
          organization: International Conference on Process Mining (ICPM) - Workshop on Education meets Process Mining (EduPM) 
          organization_url: ''
          title: 'Best Paper Award'
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2023-11-14'
          description: 'The ICT Young Researcher Award of RWTH Aachen University - PhD Category'
          organization: RWTH Aachen University 
          organization_url: ''
          title: 'The ICT Young Researcher Award'
          url: ''
    design:
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
        - name: PPPM
          tag: 'Privacy Preservation'
        - name: PM-SAP
          tag: 'SAP'
        - name: Expert Finding
          tag: 'Expert Finding'
        - name: AIStudyBuddy
          tag: 'AIStudyBuddy'
        - name: ML4ProM
          tag: 'ML4ProM'
        - name: SAP Technical
          tag: 'sapTechnical'
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: publications
    content:
      title: Publications
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
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
      # Contact (add or remove contact options as necessary)
      email: majid <dot> rafiei <at> sap <dot> com 
      #phone: 888 888 88 88
      #appointment_url: 'https://calendly.com'
      #address:
      #  street: Ahornstrasse
      #  city: Aachen
        #region: NRW
      #  postcode: '52074'
      #  country: Germany
      #  country_code: DE
      #directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      #office_hours:
      #  - 'Monday 10:00 to 13:00'
      #  - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/MajidRafiei4'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'm4jid.rafiei'
        #- icon: video
        #  icon_pack: fas
        #  name: Zoom Me
        #  link: 'https://rwth.zoom.us/j/6768788333?pwd=OXkrUko3T1hmN1N5eFFCWHhISWw4dz09'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: true
    design:
      columns: '2'
---
