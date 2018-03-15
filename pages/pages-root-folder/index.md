---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: header_roadmap_2.jpg
widget1:
  title: "Why Hyku?"
  url: '/why-hyku/'
  image: widget-1-302x182.jpg
  text: 'Are you looking for an open-source platform for your digital library or institutional repository? <em>Hyku</em> offers a hyrax-in-a-box system to let you hit the ground running.'
widget2:
  title: "Our Partners"
  url: '/our-partners/'
  image: widget-2-302x182.jpg
  text: 'Bridge2Hyku is a project by The University of Houston (UH) Libraries, in partnership and consultation with Indiana University at Bloomington (IUB) and Indiana University-Purdue University Indianapolis (IUPUI), The University of Victoria (UVic), and the University of Miami (UM).'
widget3:
  title: "Toolkit"
  url: 'https://github.com/Bridge2Hyku'
  image: widget-github-303x182.jpg
  text: 'Our toolkit will be open-source and available on github. We hope to have tools ready for community use by late 2018'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: https://t.co/NoPMvtxtWX
  text: Fill out our Migration Survey ›
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---
