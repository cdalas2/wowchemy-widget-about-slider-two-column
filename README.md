## 🌈 Add the Widget to your Site

1. Install the widget by referencing it in your `config/_defaults/config.yaml`:
   ```yaml
   module:
     imports:
       - path: github.com/cdalas2/wowchemy-widget-about-slider-two-column
   ```
   
2. Create an instance of your widget in `content/home/`, for example let's create `content/home/github.cdalas2.about-avatar-caption.md`:
```markdown
---
# An instance of the About Slider Two Column widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: github.cdalas2.about-slider-two-column

# Activate this widget? true/false
active: true

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 1

design:
  # Slide height is automatic unless you force a specific height (e.g. '400px')
  slide_height: ''
  is_fullscreen: true
  # Automatically transition through slides?
  loop: true
  # Duration of transition between slides (in ms)
  interval: 3000

content:
  slides:
    - title: 👋 Welcome to the group
      content: Take a look at what we're working on...
      align: center
      background:
        position: center
        color: '#666'
        brightness: 0.7
        media: 2707951.jpg
        fit: cover
    - title: Lunch & Learn ☕️
      content: 'Share your knowledge with the group and explore exciting new topics together!'
      align: left
      background:
        position: center
        color: '#555'
        brightness: 0.7
        media: icon.png
        fit: cover
    - title: World-Class Semiconductor Lab
      content: 'Just opened last month!'
      align: right
      background:
        position: right
        color: '#333'
        brightness: 0.7
        media: maxresdefault.jpg
        fit: cover
      link:
        icon: graduation-cap
        icon_pack: fas
        text: Join Us
        url: ''

author: "admin"
---
```

3. Create an instance of an author profile in `content/authors/`, for example let's create `content/authors/admin/_index.md`:
```markdown
---
# Display name
title: About Me
# Is this the primary user of the site?
superuser: true

# Role/position/tagline
#role: Doctoral Research Assistant of Biophysics

#organizations:
# - name: University of Southern California
#    url: https://www.usc.edu/
#  - name: Haselwandter Research Group
#    url: https://www.haselwandterlab.com/PhD-students-and-postdocs

# Short bio (displayed in user profile at end of posts)
bio: My research interests include membrane-protein interactions, protein organization, and bacteria mechanics.

#interests:
 # - Membrane Physics
 # - Bacteria Dynamics
 # - Data Science
 # - High Performance Computing

#education:
#  courses:
#    - course: PhD in Physics
#      institution: University of Southern California
#      year: Expected 2023 Graduation
#    - course: MSc in Computer Science High Performance Computing
#      institution: University of Southern California
#      year: Expected 2023 Graduation
#    - course: BSc Physics w/ Minor in Mathematics
#      institution: California Polytechnic State University, San Luis Obispo
#      year: 2017

# Social/Academic Networking
# For available icons, see: https://wowchemy.com/docs/getting-started/page-builder/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "/#contact" for contact widget.
social:
  - icon: envelope
    icon_pack: fas
    link: 'mailto:calas@usc.edu'
  - icon: google-scholar
    icon_pack: ai
    link: 'https://scholar.google.com/citations?hl=en&user=4XnI2mgAAAAJ'
  - icon: github
    icon_pack: fab
    link: https://github.com/cdalas2
  - icon: linkedin
    icon_pack: fab
    link: https://www.linkedin.com/in/carlos-alas-6a4643160/
 # - icon: cv
#    icon_pack: ai
#    link: uploads/Resume_CDA.pdf

# Enter email to display Gravatar (if Gravatar enabled in Config)
email: ''

# Highlight the author in author lists? (true/false)
highlight_name: true

caption: Carlos Alas is a doctoral research assistant of biophysics in the <a href="https://www.haselwandterlab.com">Haselwandter research group</a> at [University of Southern California](https://www.usc.edu). His research interests include membrane-protein interactions, protein organization, and bacteria mechanics. His work currently consists of modeling the impact of protein shape on bilayer deformations, temperature sensing of cells through protein-membrane interactions, and the role of protein organization in muscle degenerative diseases.
---
```
