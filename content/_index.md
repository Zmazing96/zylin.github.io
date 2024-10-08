---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-09-02
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin

  - block: collection
    id: featured
    content:
      title: Featured Publications
      count: 3
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card

  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
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
    content:
      title: Recent Publications
      count: 5
      text: |-
        {{% callout note %}}
        You can filter all publications by clicking [here](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
      
  - block: contact
    id: contact-me
    content:
      title: Contact
      email: ziyulin96@gmail.com
      address:
        city: Suwon
        postcode: '60439'
        country: South Korea
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '37.243183608381464'
        longitude: '127.08011688090518'  
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
    design:
      columns: '2'
---
