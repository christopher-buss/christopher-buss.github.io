---
layout: blocks
title: Homepage
date: 2021-01-22T19:30:00.000+00:00
page_sections:
- template: navigation-header-w-button
  block: header-2
  logo: "/uploads/forestry-full.svg"
  navigation:
  - link: "/"
    link_text: Home
  - link: "#about"
    link_text: About
  - link: "#skills"
    link_text: Skills
  - link: "#projects"
    link_text: Projects
  - link: "#blocks"
    link_text: Blocks
  cta:
    url: mailto:christopher.buss+portfolio@protonmail.com
    button_text: Contact Me
- template: hero-banner-w-image
  block: hero-2
  slug: features
  headline: i am<br><strong>game developer.</strong>
  content: Aspiring Software Engineer.<br>You'll probably find me either coding or
    playing video games.
  cta:
    enabled: true
    url: https://github.com/christopher-buss/
    button_text: My Github
  image:
    image: "/uploads/product-shot-1.png"
    alt_text: Intro
  background_image: "/uploads/hero-2-bg.png"
- template: content-feature
  block: feature-1
  media_alignment: Left
  slug: about
  headline: "<strong>About Me</strong>"
  content: Student at Royal Holloway, University of London.<br><br>Interested in how
    mainstream methodologies can be applied to the games industry pipeline to improve
    development practices and reduce crunch.<br><br>Advocate for clean, consistent
    code, automated testing, and the use of behaviour-driven development.
  media:
    image: "/blocks/blocks-split.png"
    alt_text: uBuild Blocks Mock-Up
- template: content-feature
  block: feature-1
  media_alignment: Right
  slug: skills
  headline: <strong>Customize Blocks</strong><span class="light">&nbsp;to make quick
    edits throughout your new site</span>
  content: Each block comes with custom Front Matter that can be edited in Forestry
    CMS.
  media:
    image: "/uploads/2018/06/21/edit.gif"
    alt_text: Customize Blocks
- template: 1-column-text
  block: one-column-1
  slug: projects
  headline: 16 Fully Responsive Design Blocks
  content: |
    The Design Blocks can be used without Forestry but to harness the power
    of Blocks we recommend using <a href="https://forestry.io">Forestry</a>. Once the site is imported you can immediately
    create new sites and make them fully customizable.
- template: full-width-media-element
  block: media-1
  image: "/uploads/2018/06/21/theme.png"
  caption: All Available Blocks
  slug: blocks
- template: detail-content
  block: text-1
  headline: Steps to Build a Site!
  content: <p>uBuild is an open-source Jekyll based demo that doubles as a builder
    tool inside the Forestry content manager.</p><ol><li><p><a href="https://app.forestry.io/quick-start?repo=forestryio/ubuild-jekyll&provider=github&engine=jekyll">Import
    this demo in Forestry</a>.</p></li><li><p>Read <a href="https://forestry.io/blog/ubuild-a-new-theme-for-static-sites-using-blocks/">our
    article</a> and create your own Blocks.</p></li><li><p>Add and customize the available
    Blocks and preview them as you go along.</p></li></ol>
- template: simple-footer
  block: footer-1
  content: Made with ❤︎ by <a href="https://jekyllthemes.io/theme/ubuild-jekyll-theme"
    title="">Jekyll</a>

---
