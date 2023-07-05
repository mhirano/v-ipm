## Project page template

### About

Project page template with Jekyll and GitHub Pages.  

You can create a simple project page like:  
https://mhirano.github.io/project-page-template-phantom/

This supports local test with Docker environment.

### Prerequisites

Visual Studio Code, Docker, Git, GitHub account

### How to launch a project page
1. Fork this repository with your project name ***project-name***  
  Your webpage will be https://YourGithubName.github.io/project-name/ (Not yet available, of cource)
1. Configure _config.yml for your project  
  Edit the following entries:  
    `title`, `baseurl`, `url`, `github_username`, `footer_text`, `admin_name`, (optional) `google_analytics` 
1. Edit `_include/home-hero.html`
1. Commit all and push to the GitHub
1. On GitHub's repo page, Click `Setting` -> `Pages`.
1. Below `Builld and deployment`, select `Deploy from a branch` for Source and `master`, `/(root)` beneath. Press `Save`.
1. Back to the repo's Code page, click the gear icon next to `About` in the right column. Toggle `Use your GitHub Pages website`. You'll see the webpage running after a few minutes.

### Test your page in your local environment
This codebase supports local test with Docker. Here is a very quick guide.
1. Open the project directory in Visual Studio Code.
1. On command palette, type `open folder in Container`  
  Build image from Dockerfile. No option added.
  Make sure you're inside the docker container. (You'll find root@RANDOM_NUMBERS when opening terminal inside the VSCode.)
1. On terminal, type `bundle install`
1. Then `bundle update`
1. Then `bundle exec jekyll serve --livereload`
1. If it's up and running, you can access to the project page via `http://127.0.0.1:4000/project-page-template-phantom/`

If you're ready to publish, rename the directory as you want (e.g. ***my-project***).  
create a GitHub repo named ***my-project*** and push all to it, then follow the above mentioned process (**How to launch a project page**) after *On GitHub's repo page, ...*.

### Sample
Masahiro Hirano, Yuji Yamakawa: **Falcon: A Wide-and-deep Onboard Active Vision System**, IROS2023.

https://mhirano.github.io/falcon

## Credit
Website base design: [Phantom for Jekyll](http://jamigibbs.github.io/phantom/)

## Contact
Masahiro Hirano, The University of Tokyo  
E-mail: mhirano_at_iis.u-tokyo.ac.jp