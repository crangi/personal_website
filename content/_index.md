---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Welcome!
      username: admin
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
  - block: collection
    id: featured
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
  - block: contact
    id: contact
    content:
      title: Contact
      email: rchakri25@gmail.com
      address:
        street: 280, James W. Nicholsan Hall
        city: Baton Rouge
        region: LA
        postcode: '70808'
        country: United States
        country_code: US
      coordinates:
        latitude: '30.412489659787003' 
        longitude: '-91.17835321752626'
      contact_links:
        - icon: linkedin
          icon_pack: fab
          name: Chakradhar Rangi
          link: https://www.linkedin.com/in/chakradhar-rangi/
        - icon: github
          icon_pack: fab
          name: crangi
          link: 'https://github.com/crangi'  
      # Automatically link email and phone or display as text?
      autolink: true
    design:
      columns: '2'
--- 
