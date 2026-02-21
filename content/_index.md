---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded

  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        My research focuses on stratified flows, hydrodynamic instabilities, turbulence, internal waves, environmental and geophysical fluid dynamics, and the development of ocean modeling frameworks. I have extensive experience applying a wide range of fluid dynamics and ocean modeling codes to address complex fluid mechanical problems.

        I am seeking motivated graduate students who are interested in simulating turbulent flows. Feel free to explore my projects and publications to learn more about my work and contributions to the field.
    design:
      columns: '1'

  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Postdoctoral Scholar
          company: Department of Earth System Science, University of California, Irvine
          company_url: 'https://www.ess.uci.edu/'
          company_logo: 'UCI'
          location: Irvine, USA
          date_start: '2024-02-01'
          date_end: '2026-02-01'
          description: |2-
            
            * Understanding the primary steady energy pathway from barotropic tides to the internal wave continuum and the upslope mean flow generated from tidally-driven mixing in the bottom boundary layer. 

            * Developing a parameterization method for spatial variation of internal wave breaking efficiency and irreversible mixing efficiency.

            * Strengthening [Julia programming](https://julialang.org/) skills by contributing to [Oceananigans.jl](https://clima.github.io/OceananigansDocumentation/stable/) through source code debugging, developing a customized internal tide simulation (including postprocessing functions), and actively engaging with software developers.
            
            * Extensively utilized high-performance computing and optimized resource allocation.

            * Enhancing data analysis and visualization skills.

        - title: Fluid Dynamics of Sustainability and the Environment Summer School
          company: Department of Applied Mathematics and Theoretical Physics, University of Cambridge
          company_url: 'http://www.fdse.org/'
          company_logo: 'cambridge'
          location: Cambridge, UK
          date_start: '2023-09-03'
          date_end: '2023-09-15'
          description: |2-
            
            * Participated in an intensive two-week program focused on cutting-edge theories and applications in fluid dynamics.

            * Enhanced technical, communication and collaboration skills through hands-on computational and laboratory experiments.

            * Built valuable professional connections by engaging with talented peers and leading experts.
        - title: Graduate Research Assistant
          company: College of Earth, Ocean, and Atmospheric Sciences, Oregon State University
          company_url: 'https://ceoas.oregonstate.edu/'
          company_logo: 'OSU'
          location: Corvallis, USA
          date_start: '2019-09-01'
          date_end: '2023-11-30'
          description: |2-
            
            * Under the supervision of [Bill Smyth](https://blogs.oregonstate.edu/salty/) and collaboration with [Alexis Kaminski](https://akkaminski.github.io/). [Projects](https://liuchihl.github.io/#projects) includes studying the impact on shear instability and turbulence under three conditions: (1) altering the initial random noise (butterfly effect), (2) when a stratified shear layer is near a solid boundary, and (3) when a stratified shear layer is close to another shear layer.
            
            * Enhanced analytical capabilities through the derivation of mathematical theories, improved numerical proficiency by customizing FORTRAN code, and refined coding skills through postprocessing and organizing DNS outputs using MATLAB.
            
            * Extensively utilized high-performance computing and optimized resource allocation.

            * Developed strong critical thinking and problem-solving abilities, alongside effective communication skills, by participating in conferences and publishing research in Journal of Fluid Mechanics.

        - title: Faculty Research Assistant
          company: Institute of Oceanography, National Taiwan University
          company_url: 'http://www.oc.ntu.edu.tw/oceng/'
          company_logo: 'IONTU'
          location: Taipei, Taiwan
          date_start: '2018-10-01'
          date_end: '2019-09-01'
          description: |2-
          
            * Developed a 3D nested model using [MITgcm](https://mitgcm.org/public/docs.html) to simulate oil spill pollution, improving predictive capabilities for environmental impact assessments and response strategies for the Central Weather Bureau, Taiwan.

            * Leveraged MATLAB programming skills and modeling skills to develop a 2D simulation analyzing interactions between the Kuroshio current and the I-Lan Ridge, east of Taiwan. This work collabrates with observational team in optimizing field data collection strategies and interpretation during an oceanic research cruise focused on measuring turbulence.
        - title: Substitute Military Service (Obligatory Service)
          company: 
          company_url: 
          company_logo: 
          location: Chiayi, Taiwan
          date_start: '2017-10-01'
          date_end: '2018-10-01'
          description: |2-

            * Delivered care to elderly residents in a nursing home.

            * Enhanced soft skills such as communication, adaptability, time management, and teamwork.

        - title: Graduate Research Assistant
          company: Institute of Oceanography, National Taiwan University
          company_url: 'http://www.oc.ntu.edu.tw/oceng/'
          company_logo: 'IONTU'
          location: Taipei, Taiwan
          date_start: '2015-09-01'
          date_end: '2017-08-11'
          description: |2-

            * Collaborated with [Ming-Huei Chang](https://minghueichang.wixsite.com/smallocean) on advanced island wake modeling projects.

            * Conducted in-depth analysis of the Kuroshio current using numerical simulations and field observations, providing actionable insights into oceanographic dynamics.

            * Participated in research cruises to collect and analyze ocean hydrology and dynamics data, enhancing data-driven decision-making processes.
    design:
      columns: '2'
      view: compact

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
      # buttons:
      #   - name: All
      #     tag: '*'
      #   - name: Deep Learning
      #     tag: Deep Learning
      #   - name: Other
      #     tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false

  - block: collection
    id: featured
    content:
      title: Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: list

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
      email: chihlul1@uci.edu
      # phone: 888 888 88 88
      # appointment_url: 'https://calendly.com'
      # address:
      #   street: 450 Serra Mall
      #   city: 
      #   region: 
      #   postcode: '94305'
      #   country: United States
      #   country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      # # Choose a map provider in `params.yaml` to show a map from these coordinates
      # coordinates:
      #   latitude: '37.4275'
      #   longitude: '-122.1697'  
      # contact_links:
      #   - icon: twitter
      #     icon_pack: fab
      #     name: DM Me
      #     link: 'https://twitter.com/Twitter'
      #   - icon: skype
      #     icon_pack: fab
      #     name: Skype Me
      #     link: 'skype:echo123?call'
      #   - icon: video
      #     icon_pack: fas
      #     name: Zoom Me
      #     link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    # design:
    #   columns: '2'
---
