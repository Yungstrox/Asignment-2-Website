Hosting a Resume Website Using Markdown, Jekyll, and GitHub Pages
Purpose

This README explains the technical process used to create and host a resume as a static website using Markdown, Jekyll, and GitHub Pages. The goal is to document the steps required to format a resume using lightweight markup and publish it online through a static site generator and version-controlled repository.

The intended audience for this document is students or developers who want to publish a resume website using modern technical writing tools. The instructions follow the recommendations in Andrew Etter’s Modern Technical Writing, which promotes simple tools such as Markdown, distributed version control, static site generators, and forges like GitHub for producing and maintaining documentation.

Prerequisites

Before following these instructions, the reader should have the following:

A GitHub account

Git installed on their computer

Basic knowledge of Markdown syntax

A resume written in Markdown format

A web browser

Access to a command line (Git Bash or terminal)

Software used in this project:

Static site generator: Jekyll

Forge: GitHub

Hosting platform: GitHub Pages

Instructions
Step 1: Write the resume using Markdown

Begin by writing the resume in Markdown format instead of HTML or Word. Markdown is a lightweight markup language that allows writers to focus on content rather than formatting.

For example:

# Saif Ahmed
Computer Science Major (Mathematics Minor)

## Contact Information
Phone: 813-304-7047
Email: Seeso.saif@gmail.com

Andrew Etter recommends using lightweight markup because it keeps documents simple and easy to maintain. Markdown files are plain text, meaning they can be edited with any text editor and tracked easily using version control.

Step 2: Create a GitHub repository

Next, create a repository on GitHub to store the website source files.

Log in to GitHub.

Click New Repository.

Name the repository.

Set it to Public.

Create the repository.

Using GitHub follows Etter’s recommendation to store documentation in a distributed version control system. Git allows changes to be tracked, shared, and reviewed efficiently.

Step 3: Organize the project structure

The repository must contain the source files used to generate the website. In this project the structure looks like this:

Assignment-2-Website
│
├── docs
│   ├── _config.yml
│   ├── index.md
│   └── resume
│       └── index.md
│
└── README.md

The docs folder contains the website source files. GitHub Pages is configured to publish the site from this folder.

Organizing files in a structured directory improves maintainability, which aligns with Etter’s focus on clear and maintainable documentation systems.

Step 4: Configure the Jekyll static site generator

A configuration file called _config.yml is used to configure Jekyll.

Example:

title: Assignment 2 Website
theme: minima
markdown: kramdown

This file tells GitHub Pages to generate the site using the Minima theme and the Kramdown Markdown processor.

Static site generators convert Markdown into HTML automatically. Etter encourages using static site generators because they separate content from design and simplify publishing.

Step 5: Create the website home page

The homepage is created using index.md.

Example front matter:

---
layout: default
title: Home
---

The homepage includes a short description and a link to the resume page.

# Assignment 2 Website

Welcome to my resume website.

[View my resume](resume/)

Front matter is required by Jekyll so it knows how to render the page.

Step 6: Add the resume page

The resume itself is stored as a Markdown page inside a folder.

docs/resume/index.md

The page includes front matter:

---
layout: default
title: Resume
---

Then the Markdown resume content follows. When Jekyll builds the site, this Markdown file becomes a formatted webpage.

This method demonstrates Etter’s principle of keeping documentation simple and portable, since the same Markdown file can be reused in other systems.

Step 7: Enable GitHub Pages hosting

To publish the website:

Open the repository settings.

Go to Pages.

Select Deploy from branch.

Choose the main branch.

Set the folder to /docs.

GitHub automatically builds the website using Jekyll and publishes it online.

Once deployed, the website becomes accessible through a GitHub Pages URL.

This step illustrates Etter’s principle of automated publishing systems, which reduce manual work and errors.

Step 8: Verify the website

After deployment:

Open the GitHub Pages URL.

Confirm the homepage loads correctly.

Click the resume link to ensure the page renders properly.

If the resume changes later, simply update the Markdown file and push the changes to GitHub. GitHub Pages will rebuild the site automatically.

This workflow demonstrates the advantage of combining version control with static site generators.

Further Resources

The following resources provide additional information about the technologies used in this project:

Markdown Guide
https://www.markdownguide.org/

GitHub Pages Documentation
https://docs.github.com/en/pages

Jekyll Official Documentation
https://jekyllrb.com/docs/

Modern Technical Writing by Andrew Etter
https://www.oreilly.com/library/view/modern-technical-writing/9781492049382/

Git Tutorial
https://git-scm.com/docs

FAQ
Why use Markdown instead of writing HTML directly?

Markdown is easier to read and write than raw HTML. It allows writers to focus on content rather than formatting. According to Andrew Etter, lightweight markup languages make documentation easier to maintain and collaborate on because they are simple plain-text files.

Why doesn’t my website update when I change my Markdown file?

GitHub Pages only updates when changes are committed and pushed to the repository. After pushing updates, GitHub must rebuild the site, which may take a few minutes. Clearing the browser cache or refreshing the page usually resolves this issue.

Why use a static site generator instead of writing a normal website?

Static site generators automatically convert Markdown files into formatted HTML pages. This approach allows content to remain simple while the generator handles layout and design. It also improves security and performance because static websites do not rely on server-side processing.

Credits

Author
Saif Ahmed

Peer Review Contributors
Classmates participating in the in-class peer editing session.

Third-Party Software

Jekyll Static Site Generator
https://jekyllrb.com/

Minima Theme
https://github.com/jekyll/minima

GitHub Pages Hosting
https://pages.github.com/