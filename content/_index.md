---
date: "2025-08-23"
title: null
type: landing
sections:
- block: hero
  content:
    title: MAPA Project
    image:
      filename: mapa_workflow.png
    design:
      background:
        gradient_start: '#5e4580'
        gradient_end: '#bc89ff'
        text_color_light: true
    text: |
      <br>
      
      MAPA is a software for pathway-enrichment analysis and enrichment result interpretation using Large Language Modes (LLMs) that turns complex multi-omics datasets into clear biological insight.
      
      📚 Citation: [mapa preprint](https://www.biorxiv.org/content/10.1101/2025.08.23.671949v1)
      📖 Tutorial: [MAPA tutorial](https://www.shen-lab.org/mapa-tutorial/)
      ☁️ Online MAPA Shiny: [MAPA Shiny](https://mapashiny.jaspershenlab.com/)
      
      <a class="github-button" href="https://github.com/jaspershen-lab/mapa" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star Wowchemy Website Builder for Hugo">Star MAPA project</a>
      <br>
      <a class="github-button" href="https://github.com/jaspershen-lab/mapashiny" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star Wowchemy Website Builder for Hugo">Star MAPA Shiny</a>
      <br>
      <a class="github-button" href="https://github.com/jaspershen-lab/mapa-tutorial" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star the Project Docs template">Star MAPA tutorial</a>
      <script async defer src="https://buttons.github.io/buttons.js"></script>
      
- block: people
  id: team
  content:
    sort_ascending: true
    sort_by: Params.last_name
    title: TEAM
    subtitle: ":point_right: [All Team Members](./team/)"
    # text: |-
    #   {{% callout note %}}
    #   [All team members](./team/).
    #   {{% /callout %}}
    user_groups:
    - Authors
  design:
    show_interests: false
    show_role: true
    show_social: true


- block: contact
  id: contact
  content:
    title: CONTACT
    # subtitle: ":point_right: [More social media](./contact/)"
    text: 
    # Contact (add or remove contact options as necessary)
    email: xiaotao.shen@outlook.com
    phone: +65 83042333
    # appointment_url: 'https://calendly.com'
    address:
      street: 59 Nanyang Dr
      city: Singapore
      region: Singapore
      postcode: '636921'
      country: Singapore
      country_code: SG
    # office_hours:
    #   - 'Weekdays 9:00 to 18:00'
    contact_links:
      # - icon: video
      #   icon_pack: fas
      #   name: Zoom Me
      #   link: 'https://zoom.com'
      - icon: weixin
        icon_pack: fab
        name: Follow us on WeChat
        link: 'https://jaspershen.github.io/image/wechat_QR.jpg'
      - icon: twitter
        icon_pack: fab
        name: Follow us on X
        link: https://twitter.com/xiaotaoshen1990
      - icon: github
        icon_pack: fab
        name: Follow us on Github
        link: https://github.com/jaspershen-lab
    # Automatically link email and phone or display as text?
    autolink: true
    # Email form provider
    form:
      formspree:
        id: xpzgpjby
      netlify:
        captcha: false
      provider: formspree
      netlify:
        # Enable CAPTCHA challenge to reduce spam?
        captcha: false
      # Coordinates to display a map - set your map provider in `params.yaml`
      coordinates:
        latitude: '37.4275'
        longitude: '-122.1697'
  design:
    columns: '2'


- block: collection
  id: news
  content:
    count: 10
    filters:
      folders:
        - news
      exclude_featured: false
    offset: 0
    order: desc
    subtitle:
    title: NEWS
    text: 
  design:
    columns: "2"
    view: list
    background:
      image:
        filename: 
        filters:
          brightness: 1
      #  Image fit. Options are `cover` (default), `contain`, or `actual` size.
      size: cover
      # Image focal point. Options include `left`, `center` (default), or `right`.
      position: center
      # Use a fun parallax-like fixed background effect on desktop? true/false
      parallax: true
      # Text color (true=light, false=dark, or remove for the dynamic theme color).
      text_color_light: false    

---
