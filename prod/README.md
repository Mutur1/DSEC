# DSEC Cybersecurity Website

- Welcome to DSEC, your trusted partner in safeguarding digital assets. This repository hosts the source code for our static website, built with HTML, CSS & JavaScript, and deployed via a CI/CD pipeline to GitHub Pages. 
- Our mission is to provide top-tier cybersecurity solutions—explore our services and see how we can protect your business from evolving threats.
Table of Contents

### Project Overview
    Features
    Folder Structure
    Getting Started
        Prerequisites
        Local Development
    CI/CD Pipeline
    Deployment
    Contributing
    License
    Contact

### Project Overview

DSEC is a static website designed to promote our cybersecurity services, including penetration testing, threat intelligence, and incident response. Built with simplicity and performance in mind, this site uses vanilla HTML, CSS, and JavaScript, with assets like images and icons stored in the assets/ folder. The site is automatically deployed to GitHub Pages using GitHub Actions, ensuring seamless updates from development to production.

Live URLs:

    Development: https://Mutur1.github.io/DSEC/dev/
    Production: https://Mutur1.github.io/DSEC/prod/

#### Features

    - Responsive Design: Adapts to desktops, tablets, and mobile devices.
    - Service Highlights: Showcases cybersecurity offerings with clear calls-to-action.
    - Fast & Secure: Lightweight static site with no server-side dependencies.
    - Automated Deployment: CI/CD pipeline deploys changes to dev and prod environments.

### Folder Structure
```shell
DSEC/
├── .github/
│   └── workflows/
│       └── deploy.yml       # GitHub Actions workflow for CI/CD
├── assets/                  # Images, icons, and other static resources
│   └── (e.g., logo.png)
├── index.html               # Main HTML file
├── styles.css               # CSS styling for the site
└── README.md                

```
    - .github/workflows/deploy.yml: Defines the deployment pipeline to GitHub Pages.
    - assets/: Holds all static assets (add your images here).
    - index.html: The entry point of the website.
    - styles.css: Custom styles for layout and design.

## Getting Started

#### Prerequisites

    Git: To clone and manage the repository.
    Web Browser: For local testing (e.g., Chrome, Firefox).
    Text Editor: Like VS Code or Sublime Text for editing files.
    GitHub Account: For deployment and hosting.

No additional tools (e.g., Node.js) are required since this is a pure static site.

### Local Development

    Clone the Repository:
  
  ```bash
git clone https://github.com/Mutur1/DSEC.git
``` 

```bash
cd DSEC
```

Open Locally:

    Double-click index.html to view it in your browser, or
    Use a local server for better testing:

      ```bash
        npm install http-server
      ```

  - Then visit [http://127.0.0.1:8081](http://127.0.0.1:8081)
    Make Changes:
    Edit index.html for content.
    Update styles.css for design.
    Add images or assets to the assets/ folder.
    Test:
        Refresh your browser to see updates.
        Test responsiveness using browser dev tools (e.g., mobile view).

### CI/CD Pipeline

We use GitHub Actions to automate deployment:

    Trigger: Pushes to dev or prod branches (typically via merged pull requests).
    Workflow: Defined in .github/workflows/deploy.yml.
    Process:
        Checks out the code.
        Deploys files to the gh-pages branch using peaceiris/actions-gh-pages.
        Files go to gh-pages/dev/ for dev and gh-pages/prod/ for prod (or root for prod if configured).

To modify the pipeline, edit deploy.yml and commit changes.
Deployment

The site is hosted on GitHub Pages:

    Source Branch: gh-pages.
    URLs:
        dev: https://Mutur1.github.io/DSEC/dev/
        prod: https://Mutur1.github.io/DSEC/ (or /prod/).

`To deploy updates:`

    Create a feature branch (e.g., feature/new-service):
    bash

git checkout -b feature/new-service

Commit and push changes:
```bash

    git add .
    git commit -m "Add new service section"
    git push origin feature/new-service
    Open a pull request to dev or prod on GitHub.
    Merge the PR—GitHub Actions will deploy automatically.
```

Check the Actions tab for deployment status.
Contributing

We welcome contributions to improve DSEC’s website! To contribute:

    Fork the repository.
    Create a feature branch (git checkout -b feature/your-idea).
    Commit your changes (git commit -m "Describe your change").
    Push to your fork (git push origin feature/your-idea).
    Open a pull request to the dev branch.

Please ensure your code follows basic HTML/CSS best practices and includes a descriptive PR message.
License

This project is licensed under the MIT License. See LICENSE for details (add a LICENSE file if you want to formalize this).
Contact

For inquiries about our cybersecurity services or this project:

    Email: muturi@gmail.com
    GitHub Issues: Open an issue on this repository.
    Website: Visit us at https://Mutur1.github.io/DSEC/

Stay secure with DSEC—because your defenses should be as strong as your ambitions.

### Reasources

[CSS Grid Layout properties](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-rows)

```css
@media(max-width: 480px){
  .vision-mission-values{
    margin: 0.5rem;
  }
  .text{
    font-size:16px ;
  }
  ```