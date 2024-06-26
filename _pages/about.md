---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
Hi 👋 I'm a 3rd year PhD student at the LISN Lab, Université Paris-Saclay, working on Dialogue Systems and NLP.

<!-- **Thesis** : Towards More Natural Dialogues: Integrating Open-domain Dialogue Skills into Task-oriented Agents -->

My research focuses on the intersection between open-domain dialogue (a.k.a. chitchat) and task-oriented dialogue (TOD), which are typically regarded as two distinct modes. I aim to assess and integrate useful open-domain qualities into TOD systems, enhancing response appropriateness and system resilience to open-domain inputs.
<!-- Open-domain systems are designed to embody all the attributes of an ideal conversationalist, including empathy, engagement, knowledge, and politeness. In contrast, task agents are typically engineered to be efficient and effective tools.  -->


**My latest projects include**:
- Evaluation of the robustness of a Few-shot TOD Bot to inter-mode inputs (task requests that mix in chitchat or that are based on previous chitchat turns).  Casting dialogue state tracking as a function call generation task heavily improves JGA and end-to-end performance compared with an existing baseline prompting strategy, and stands out as more robust to inter-mode inputs. *Under Review*

- Dialogue state tracking for inter-mode inputs using TOD data only. Combining a TOD-only state tracker with 0-shot prompting for query reformulation leads to superior and comparable results on two benchmarks (respectively) compared with an LLM fine-tuned on inter-mode data. *Under Review* 

- Novel chitchat augmentation for MultiWOZ using in-context learning with Llama-2-70B. Provides a testbed for building more chitchat-resilient TOD systems and enables a system to respond with chitchat and TOD all in the same turn. *LREC-COLING 2024* [link](https://aclanthology.org/2024.lrec-main.284/)

- A unified approach to user emotion detection and TOD modeling, using a mixture of LoRA fine-tuning and CoT prompting on Llama-2-7B. Leads to improved task success rates and more empathetic responses. *IWSDS 2024* [link](https://arxiv.org/abs/2401.13789)

- Comparative study based on entropy of recent Task-Oriented Dialogue datasets enhanced with chitchat. *ASRU 2023* [link](https://ieeexplore.ieee.org/document/10389695)

[Papers on Arxiv](https://arxiv.org/search/?query=armand+stricker&searchtype=all&source=header)

<!-- - A novel automatic chitchat augmentation for MultiWOZ, in which a chatty user adds elements of backstory to their request. System responses are also automatically enhanced to provide support and understanding while still advancing the task. This provides a testbed for building more chitchat-resilient TOD systems. Baselines assessed are end-to-end and built on top of Llama-2, fine-tuned with LoRA.
- A unified approach to user emotion detection (ED) and TOD modeling.  ED is generally overlooked or treated as an independent, additional task in TOD systems. I assess the benefits of directly including user emotions into an end-to-end TOD pipeline. Tasks are learned with a unified language modeling objective and lead to mutual benefits. Experiments are based on GPT-2, Llama-2 and the EmoWOZ dataset.
- A zero-shot method for TOD grounded in previous chitchat exchanges. In this scenario, finding task-relevant entities in the previous chitchat is crucial and poses a unique coreference challenge. I explore the possibility of using a TOD-only model and zero-shot prompting for Query Reformulation to handle the challenge of inter-mode coreference, without the need for additional training data or fine-tuning. Experiments are based on GPT-3.5-turbo, LLama-2-7B and the FusedChat dataset. -->

<!-- 
**Topics of Interest**:
- Moving towards more user-focused TODs. This includes the development of more user-adaptive TOD systems, which can adapt to the user's conversational style, preferences, and emotions.
- Simulating more conversational and challenging TOD flows with LLMs to improve and evaluate system resilience. -->



<!-- This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
