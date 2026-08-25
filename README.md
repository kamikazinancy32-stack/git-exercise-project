# Git Exercise Solutions

## Bundle 1 Exercise 1
- git init
- git branch -M main
- git add .
- git commit -m "Initial project setup"
- git remote add origin https://github.com/kamikazinancy32-stack/git-exercise-project.git
- git push -u origin main
- git checkout -b dev
- git checkout -b test
- git checkout dev
- git branch -d test

## Bundle 1 Exercise 2
- git checkout dev
- git stash
- git stash pop
- git add home.html about.html
- git commit -m "Add home page and update about page"
- git push origin dev

## Bundle 2 Exercise 1
- git checkout -b ft/bundle-2
- git add services.html
- git commit -m "Add Services page"
- git commit -m "Rename service page"
- git push origin ft/bundle-2
- git checkout main
- git merge ft/bundle-2
- git push origin main

## Bundle 2 Exercise 2
- git checkout main
- git pull
- git checkout ft/service-redesign
- git merge main
- git add services.html
- git commit -m "Add services page content on service redesign"
- git push origin ft/service-redesign
- git checkout main
- git add services.html
- git commit -m "Update services heading on main branch"
- git push origin main
- git checkout ft/service-redesign
- git merge main
- git add services.html
- git commit -m "Resolve merge conflict between main and service redesign"
- git push origin ft/service-redesign

## Bundle 3 Exercise 1
- git checkout main
- git checkout -b ft/team-page
- git add team.html
- git commit -m "Add team page"
- git push origin ft/team-page
- git checkout main
- git checkout -b ft/contact-page
- git log --oneline ft/team-page
- git cherry-pick ec63a30
- git add contact.html
- git commit -m "Add contact page"
- git push origin ft/contact-page
- git checkout -b ft/faq-page
- git add faq.html
- git commit -m "Add FAQ Page"
- git push origin ft/faq-page
- git revert ec63a30
- git push origin ft/faq-page

## Bundle 3 Exercise 2
- git checkout ft/faq-page
- git checkout -b ft/home-page-redesign
- git checkout main
- git add index.html
- git commit -m "Update home page on main"
- git push origin main
- git checkout ft/home-page-redesign
- git rebase main
- git add index.html
- git commit -m "Redesign home page"
- git push origin ft/home-page-redesign

## Bundle 4 Exercise 1
- git checkout main
- git remote add git-copy https://github.com/kamikazinancy32-stack/git-exercise-project-copy.git
- git remote -v
- git add index.html
- git commit -m "Update home page for dual push"
- git push origin main
- git push git-copy main

## Bundle 4 Exercise 2
- git checkout -b ft/footer
- git add index.html
- git commit -m "Add footer section"
- git add index.html
- git commit -m "Add footer with contact info"
- git push origin ft/footer
- git checkout main
- git checkout -b ft/squashing
- git merge --squash ft/footer
- git commit -m "footer changes squashing"
- git push origin ft/squashing

## Bundle 5 Exercise 1
- Enabled GitHub Pages on repository settings
- Site URL: https://kamikazinancy32-stack.github.io/git-exercise-project/

## Bundle 5 Exercise 2
- Forked https://github.com/octangroup/git-cafe-exercise
- git clone https://github.com/kamikazinancy32-stack/git-cafe-exercise.git
- cd git-cafe-exercise
- git add index.html
- git commit -m "change welcome message to restaurant"
- git push origin main
- Created Pull Request to original repository