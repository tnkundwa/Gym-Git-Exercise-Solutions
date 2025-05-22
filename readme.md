# Git exercises 1

## Exercise one
```bash
$ git init 
$ git branch -M main
$ git status
$ git status
$ git add .
$ git status
$ git push --set-upstream origin main
$ git pull origin main
$ git add .
$ git push --set-upstream origin main
$ git push --force --set-upstream origin main
$ git push
$ git status
$ git push
$ git push --set-upstream origin ft/bundle-2
$ git push
$ git branch -m "ft/bundle-2" "dev"
$ git branch
$ git status
$ git push
$ git push
$ git branch
$ bit status
$ git status
$ git push origin "dev"
$ git push
$ git branc
$ git checkout -b Test
$ git push origin test
$ git checkout dev
$ git delete -D test
$ git branch -D test
$ git push origin --delete test
$ git branch
$ git checkout main
```

##Exercise 2
```bash
$ git pull
$ git status
$ git add home.html
$ git stash
$ git stash list
$ git add about.html 
$ git stash
$ git status
$ git add team.html 
$ git stash
$ git stash list
$ git stash pop stash@{1}
$ git stash list
$ git stash pop stash@{0}
$  git status
$ git add .
$ git push
$ git merge ft/bundle-2
$ git push origin HEAD:ft/bundle-2
$ git stash pop
$ git stash list
$ git reset --hard
$ git stash list
```

#Bundle 2
## Exercise 1
```bash
$ git checkout -b "ft/bundle-3"
$ git branch
$ git add services.html 
$ git commit -m "Working on exercise 3"
$ git push
$ git push --set-upstream origin ft/bundle-3
```

##Exercise 2
```bash
$ git status
$ git status
$ git add .
$ git commit -m "Added some new services"
$ git push
$ git push --set-upstream origin ft/service-redesign
$ git status
$ git checkout main
$ git add .
$ git commit -m "Added other new services"
$ git push
$ git checkout ft/service-redesign 
$ git diff
$ git diff main
$ git merge main
$ git merge main
$ git merge main
$ git status
$ git add .
$ git commit -m "Combined both services"
$ git push
```

#Bundle 3
##Exercise 1
```bash
$ git checkout -b ft/team-page
$ git add team1.html 
$ git commit -m "Created a new html page"
$ git push
$ git push --set-upstream origin ft/team-page
$ git checkout main
$ git checkout -b ft/contact-page
$ git checkout ft/team-page
$ git log
$ git checkout ft/contact-page 
$ git cherry-pick d0ac4987d44efa72b60f45a3cb301fd5a018b60f
$ git add contact.html 
$ git status
$ git commit -m "Added a new contact html page"
$ git push
$ git push --set-upstream origin ft/contact-page
$ git checkout -b ft/faq-page
$ git add .
$ git commit -m "Added a new Faq page"
$ git push
$ git push --set-upstream origin ft/faq-page
$ git revert d0ac4987d44efa72b60f45a3cb301fd5a018b60f
$ git status
$ git add .
$ git commit -m "Just used the revert command"
$ git push
```
##Exercise 2
```bash
$ git checkout ft/faq-page
$ git checkout -b ft/home-page-redesign
$ git checkout main
$ git status
$ git add .
$ git push
$ git checkout ft/home-page-redesign
$ git rebase main
$ git add .
$ git commit -m "After rebasing I made some more changes"
$ git push
$ git push --set-upstream origin ft/home-page-redesign
```

#Bundle 4
##Exercise 1
```bash
$ git checkout main
$ git remote add git-copy https://github.com/tnkundwa/git-exercise-clone.git
$ git remote
$ git status
$ git add home.html 
$ git status
$ git commit -m "I just made some changes to the home html page"
$ git push
$ git push git-copy
```
##Exercise 2
```bash
$ git checkout -b ft/footer
$ git status
$ git add footer.html 
$ git commit -m "Added a new footer html page"
$ git add footer.html 
$ git commit -m "Added more content to the footer page"
$ git push
$ git push --set-upstream origin ft/footer
$ git checkout main
$ git checkout -b ft/squashing
$ git merge --squash ft/footer 
$ git status
$ git commit -m "footer changes squashing"
$ git status
$ git push
$ git add .
$ git push --set-upstream origin ft/squashing
$
```
#Bundle 5
##Exrcise 2
```bash
$ ls
$ cd ..

LONOVO@toussaintn23 MINGW64 ~
$ ls
$ cd Git\ Exercises/
$ ls
$ cd ..
$ git clone https://github.com/tnkundwa/git-cafe-exercise.git
$ ls
$ cd git-cafe-exercise/
$ ls
$ code .
$ git checkout main 
$ git status
$ git add .
$ git commit -m "Changed from place to restaurant"
$ git push
$
```