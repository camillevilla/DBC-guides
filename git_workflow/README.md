# Git Workflow Examples
(more to come)

- [git cheatsheet](#git-cheatsheet)
- [End of exercise / end of day PRs](#end-of-exercise--end-of-day-prs)
- [Pairing --> Solos](#pairing----solo)

## Git Cheatsheet

![Git workflow examples: clone, commit, add, and push](git_workflow_00.png)

## End of exercise / end of day PRs
- `git status`
- `git add FILENAME` add a
- ny changed files
- `git commit -m "my descriptive commit message"`
- `git push origin pair-camillevilla,bobross`
- Go to the GitHub repo for the exercise (e.g. sf-fiddlercrabs-2017/regex-drill)
- Click on the `Pull requests` tab

![Screenshot: Pull Request tab](PR_tab.png)

- Click on the green "New pull request" button
- Set the two branch for comparison. The base should be `master` and the compare branch should be your pair branch (e.g. `pair-camillevilla,bobross`)

![Screenshot: Pull Request button](compare_branches.png)

- Add comments, tag your advisor for a code review, etc.
- Click the green "Create pull request" button

## Pairing --> Solo
Example: At the end of core hours, you and your pair decide to go home for the evening and work on things separately.

- open your terminal and `git clone` the repo
- `git fetch origin` - this fetches information about all available branches on GitHub
- go to your open pull request on GitHub and copy the branch's name (e.g. `pair-camillevilla,bobross`)
- `git checkout -b pair-camillevilla,bobross origin/pair-camillevilla,bobross`
- `git log` and check your commit history
- `git checkout -b solo-camillevilla` - you now have your own branch that includes your past pair work
- `git push origin solo-camillevilla` and open a pull request
