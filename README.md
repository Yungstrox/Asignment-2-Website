# Hosting a Resume Website Using Markdown, Jekyll, and GitHub Pages

## Purpose

This README explains how a resume was created and published as a static website using modern technical documentation tools. The project demonstrates how Markdown, Git, Jekyll, and GitHub Pages can be used together to produce structured and maintainable documentation.

The primary goal of this assignment is to host a resume online using a static site generator while documenting the process in a clear and organized way. The intended audience for this README is a student or technical writer who wants to understand how to create a simple static documentation site using modern technical writing practices.

The approach used in this project follows the recommendations from Andrew Etter’s *Modern Technical Writing*. Etter encourages writers to use lightweight markup languages, distributed version control systems, static site generators, and forges to create documentation that is easy to maintain and publish.

By combining Markdown with Git and Jekyll, this project demonstrates how technical documentation can be written in plain text, tracked with version control, and automatically converted into a professional website.

---

## Prerequisites

Before following these instructions, the reader should have the following resources available.

### Accounts

- A GitHub account
- Internet access

### Software

- Git installed on the computer
- A text editor such as Visual Studio Code, Notepad++, or another Markdown-compatible editor
- A web browser

### Knowledge

- Basic familiarity with Markdown syntax
- Basic command line usage
- Basic Git commands such as cloning and pushing

### Tools Used in This Project

| Tool | Purpose |
|-----|------|
| Markdown | Writing the resume content |
| Git | Version control |
| GitHub | Hosting the source repository |
| Jekyll | Static site generator |
| GitHub Pages | Hosting the generated website |

These tools align with Etter’s principle of using simple, text-based systems that allow documentation to be easily maintained and automatically published.

---

## Instructions

The following steps explain how to create and publish a resume website using a static site generator.

### Step 1: Write the Resume Using Markdown

Create the resume using Markdown instead of HTML or word processing software.

Example structure:
Name
Education
Work Experience
Skills
### Step 2: Create a GitHub Repository

Create a repository on GitHub to store the project files.

1. Log into GitHub.
2. Click **New Repository**.
3. Enter a repository name.
4. Set the repository to **Public**.
5. Create the repository.

Using a Git repository follows Etter’s recommendation of using distributed version control systems to manage documentation. Git allows changes to be tracked, reviewed, and reverted if necessary.

---

### Step 3: Organize the Project Structure

Organize the project files using a clear directory structure.

Example structure:Assignment-2-Website
│
├── README.md
│
└── docs
├── _config.yml
├── index.md
└── resume
└── index.md


The `docs` directory contains the files used to generate the website. GitHub Pages can publish a site directly from this folder.

Maintaining a structured directory layout improves clarity and maintainability, which are key principles in technical documentation.

---

### Step 4: Configure the Static Site Generator

Create a configuration file called `_config.yml` inside the `docs` directory.

Example configuration:
title: Assignment 2 Website
theme: minima
markdown: kramdown

This configuration tells Jekyll which theme to use and which Markdown processor should convert Markdown into HTML.

Static site generators automate the process of converting documentation into websites. Etter recommends this approach because it separates content creation from design and simplifies publishing workflows.

---

### Step 5: Create the Homepage

Create a file named `index.md` inside the `docs` directory.

Add Jekyll front matter to the file:
layout: default
title: Home

Then add content for the homepage.

Example:Assignment 2 Website

Welcome to my resume website.

![]View my resume()


The homepage provides an overview of the site and links to the resume page.

---

### Step 6: Add the Resume Page

Create a folder named `resume` inside the `docs` directory and add a Markdown file called `index.md`.

Example path:docs/resume/index.md


Include Jekyll front matter at the top of the file:
layout: default
title: Resume
Below the front matter, add the Markdown resume content.

Using Markdown for the resume ensures the document remains portable and easy to update.

---

### Step 7: Enable GitHub Pages

Publish the website using GitHub Pages.

1. Open the repository settings.
2. Navigate to the **Pages** section.
3. Select **Deploy from branch**.
4. Choose the **main branch**.
5. Set the folder to `/docs`.

GitHub Pages will automatically build the website using Jekyll.

Automated publishing is a key concept discussed in *Modern Technical Writing* because it reduces manual effort and minimizes publishing errors.

---

### Step 8: Verify the Website

After enabling GitHub Pages, open the generated website URL.

Verify that:

- The homepage loads correctly
- The resume page is accessible
- The formatting appears correctly

If changes are made to the Markdown files, simply commit and push the updates to GitHub. GitHub Pages will automatically rebuild the site.

This workflow demonstrates how version control and automated publishing can simplify documentation management.

---

## Further Resources

The following resources provide additional information about the technologies used in this project.

### Markdown Guide
https://www.markdownguide.org/

### GitHub Pages Documentation
https://docs.github.com/en/pages

### Jekyll Documentation
https://jekyllrb.com/docs/

### Modern Technical Writing – Andrew Etter
https://www.oreilly.com/library/view/modern-technical-writing/9781492049382/

### Git Documentation
https://git-scm.com/docs

These resources provide additional background information on Markdown, static site generators, and version control systems.

---

## FAQ

### Why use Markdown instead of HTML?

Markdown is simpler to read and write than raw HTML. Because Markdown is plain text, it allows writers to focus on content rather than formatting. Andrew Etter recommends lightweight markup languages because they make documentation easier to maintain and integrate with version control systems.

---

### Why use a static site generator?

Static site generators automatically convert Markdown files into HTML pages. This allows writers to maintain documentation in plain text while generating professional-looking websites automatically. Static sites are also faster and more secure because they do not rely on server-side processing.

---

### Why doesn’t my website update immediately?

GitHub Pages rebuilds the website after changes are pushed to the repository. This process may take a few minutes. Refreshing the browser or clearing the cache will usually display the updated version.

---

### Why use Git for documentation?

Git tracks every change made to the documentation. This allows authors to review edits, revert mistakes, and collaborate with others. Version control systems make documentation easier to manage over time.

---

## Credits

### Author

Saif Ahmed

### Peer Review Contributors

Mohammad Kmr  
Ahmed Abdelgalil  

### Third-Party Software

Jekyll Static Site Generator  
https://jekyllrb.com/

Minima Theme  
https://github.com/jekyll/minima

GitHub Pages Hosting  
https://pages.github.com/

### Additional Tools

Git Version Control  
https://git-scm.com/

Markdown Documentation  
https://www.markdownguide.org/
