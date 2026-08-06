---
layout: about
title: About
permalink: /
subtitle: Applied AI Scientist, PhD in NLP

profile:
  align: right
  image: prof_pic.jpg
  image_circular: true # crops the image to make it circular

selected_papers: true # includes a list of papers marked as "selected={true}"

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  # No limit: `limit` truncates the list before rendering rather than
  # paging it, so anything beyond it never reaches the page. Leaving it
  # unset renders every item, and scrollable keeps the box a fixed height.

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<style>
.news {
  height: 350px;
  overflow-y: auto;
  padding-right: 8px;
}

/* news.liquid puts an inline max-height on the inner .table-responsive
   whenever the feed is scrollable, which nests a second scrollbar inside
   this one. Inline styles beat selectors, hence !important. */
.news .table-responsive {
  max-height: none !important;
  overflow: visible;
}

/* Section headings ("news", "selected publications") are hardcoded
   lowercase in the theme's about layout, so capitalise them here
   rather than shadow the whole layout for two words. */
/* Section headings are plain text in the local about layout, which
   carries the capitalisation, so no text-transform or :has() workaround
   is needed -- only the spacing that keeps them off the section above. */
.section-heading {
  margin-top: 2.5rem;
}

/* Navbar social icons: larger than the gem's 1.7rem default */
#navbar .navbar-brand.social {
  font-size: 2.2rem;
}

#navbar .navbar-brand.social a {
  margin-right: 0.75rem;
}

/* Footer blends into the page background */
footer.fixed-bottom,
footer.sticky-bottom {
  background-color: var(--global-bg-color);
  border-top: none;
}

footer.fixed-bottom .container,
footer.sticky-bottom .container {
  color: var(--global-bg-color);
}
</style>

Hi, I'm Tarek, an Applied AI Scientist with a PhD in Natural Language Processing.

I am currently a Principal Data Scientist at [Presight](https://presight.ai/), part of [G42](https://www.g42.ai/), where I have spent more than seven years building and deploying AI systems across government, finance, public health, and behavioral analytics. My work spans client-facing delivery, product development, and R&D, often taking projects from an ambiguous initial requirement to a production system used in real operational settings.

More recently, I have focused on generative AI and agentic systems, including investment intelligence, law-enforcement decision support, analytical reporting, and multilingual speech technologies. My earlier work tackled applied NLP, computer vision, knowledge graphs, predictive modeling, and cloud-based big-data analytics.

Explore [selected projects](/projects/).

Alongside my industry role, I recently completed a PhD in Natural Language Processing at [MBZUAI](https://mbzuai.ac.ae/) with [Preslav Nakov](https://scholar.google.com/citations?user=DfXsKZ4AAAAJ&hl=en). My research spans multilingual NLP, psycholinguistics, cognitive computing, and computational social science, with publications at ACL, EMNLP, EACL, and NAACL.

Before MBZUAI, I completed an M.S. in Electrical Engineering at [KAUST](https://www.kaust.edu.sa/), then worked in [Jeff Shamma](https://scholar.google.com/citations?user=ixE1z7UAAAAJ&hl=en)’s group on autonomous multi-robot systems for exploration, coordination, and perception, culminating in first place at an international robotics competition in Spain.
