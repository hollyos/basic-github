# Basic GitHub Project Setup

## Synopsis

Basic steps to follow when getting your team set up on GitHub work flow.

## Getting Started

### Local Setup

1. Fork repo

2. Clone down _your_ repo and `cd` to directory

3. Set up upstream branch and verify `upstream` was created

  ```
  git remote add upstream <main repo link (https or ssh)>
  git remote -v
  ```

### Work Flow

1. Work in feature branches. To create a branch use the -b modifier. [Documentation on branching & merging](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging).

  ```
  git checkout -b <yourBranch>
  ```

2. Add changes

  ```
  git add -A
  ```

3. Pull most recent changes from `upstream`

  ```
  git pull upstream <yourBranch>
  ```

4. Commit changes

  ```
  git commit -m "your commit message"
  ```

5. Switch branches to `master` then merge `<yourBranch>` to `master`

  ```
  git checkout master
  git merge <yourBranch>
  ```

6. Ensure you're up to date with `master`

  ```
  git pull upstream master
  ```

5. If there are changes commit your the changes from your pull

  ```
  git commit -m "your commit message"
  ```

7. Push changes to `origin` (your repo)

  ```
  git push origin master
  ```

8. Submit pull request to `upstream`. Utilize the GUI on GitHub in your repo.

9. Pull Requests should be reviewed and approved by at least 2 members to ensure quality. Utilize the comments to gain team approvals.

10. Once team members agree code is up to snuff the repo owner/admin can merge the pull request (utilize the GUI).

## Contributors

[Holly Springsteen](https://github.com/badwolf7)