---
permalink: /
title: "Bio."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


<section id="aboutme">
My name is Fahao Chen. I received my Ph.D. degree from the Graduate School of Computer Science and Engineering, The University of Aizu in September 2024, supervised by Prof. Peng Li. My research interests include edge computing and distributed machine learning systems.
</section>

<section id="news">
  <h2>News</h2>
  <ul>
    <li><em>December 2024:</em> Two papers are accepted by <strong>IEEE INFOCOM 2025</strong>.</li>
    <li><em>October 2023:</em> One papers is accepted by <strong>ACM SIGMOD 2024</strong>.</li>
  </ul>
</section>


<section id="experience">
  <h2>Experience</h2>
  <ul>
    <li><em>2021 - 2024:</em> Ph.D. at <strong>The University of Aizu</strong>, supervised by Prof. Peng Li.</li>
    <li><em>2019 - 2021:</em> M.S. at <strong>The University of Aizu</strong>, supervised by Prof. Peng Li.</li>
    <li><em>2016 - 2020:</em> B.E. at <strong>China University of Geoscience (Wuhan)</strong>, supervised by Prof. Deze Zeng.</li>
  </ul>
</section>

<section id="publications">
  <h2>Selected Publications</h2>
  {% include base_path %}

  <!-- New style rendering if publication categories are defined -->
  {% if site.publication_category %}
    {% for category in site.publication_category  %}
      {% assign title_shown = false %}
      {% for post in site.publications reversed %}
        {% if post.category != category[0] %}
          {% continue %}
        {% endif %}
        {% unless title_shown %}
          <h3>{{ category[1].title }}</h3><hr />
          {% assign title_shown = true %}
        {% endunless %}
        {% include archive-single.html %}
      {% endfor %}
    {% endfor %}
  {% else %}
    {% for post in site.publications reversed %}
      {% include archive-single.html %}
    {% endfor %}
  {% endif %}
</section>


<section id="honors">
  <h2>Honors and Awards</h2>
  <ul>
    <li><em>August 2024:</em> Chinese Government Award for Outstanding Self-financed Students Abroad</li>
    <li><em>December 2023:</em> Best Paper Award from <strong>IEEE BDCloud</strong></li>
    <li><em>November 2023:</em> Best Paper Award from <strong>IEEE CyberSciTech</strong></li>
    <li><em>March 2023:</em> Research Fellowships for Young Scientists from <strong>Japan Society for the Promotion of Science (JSPS)</strong></li>
    </ul>
</section>


<!-- Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
2. Fork [this template](https://github.com/academicpages/academicpages.github.io) by clicking the "Use this template" button in the top right. 
3. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
4. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
5. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
6. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
