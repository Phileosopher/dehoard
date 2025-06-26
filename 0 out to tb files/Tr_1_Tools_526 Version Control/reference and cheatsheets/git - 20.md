
[Git Cheatsheet (Visualization) | Hacker News](https://news.ycombinator.com/item?id=2461700)
[index :: Git Cheatsheet :: NDP Software](https://www.ndpsoftware.com/git-cheatsheet.html)

[Git Cheat Sheet : git](https://old.reddit.com/r/git/comments/bwwqr3/git_cheat_sheet)

[MrKrishnaAgarwal/Git-CheatSheet: This repository lists mostly all git commands, some great resources and books for learning git.](https://github.com/MrKrishnaAgarwal/Git-CheatSheet)

[EshanTrivedi21/Git-CheatSheet: An opensource initiative to which over 37 individuals from all over the world collaborated in order to streamline the process of learning Git and GitHub.](https://github.com/EshanTrivedi21/Git-CheatSheet)

[Andrew Peterson](http://ndpsoftware.com/git-cheatsheet.html)
Interactive Git Cheatsheet with a weird UI

[MorganGeek](https://github.com/MorganGeek/bookmarks/blob/master/cheat/git.md)
My cheatsheet for Git

[Mark Lodato](https://marklodato.github.io/visual-git-guide/)
A Visual Git Reference

[agis/Git Style Guide](https://github.com/agis/git-style-guide)
[How to Get Your Change Into the Linux Kernel](https://kernel.org/doc/html/latest/process/submitting-patches.html)
inspiration for it
[git man pages](http://git-scm.com/doc)
inspiration for it

[Sven Hofmann](https://gist.github.com/hofmannsven/6814451)
Simply git cheatsheet

[GIT Guidelines](https://guides.github.com/introduction/flow/index.html)

[Git Cheat Sheet – Helpful Git Commands with Examples](https://www.freecodecamp.org/news/git-cheat-sheet-helpful-git-commands-with-examples/)

### Undo last commit while keeping changes

`git reset HEAD^`

### Get latest submodules changes ([src](https://stackoverflow.com/questions/5828324/update-git-submodule-to-latest-commit-on-origin))

`git submodule foreach git pull origin master`

### Most active hours from git history ([src](https://gist.github.com/bessarabov/674ea13c77fc8128f24b5e3f53b7f094#gistcomment-2973934))

```
git log --author="Morgan" \
        --format="%ad" \
        --date="format:%H" |\
        awk '{n=$1+0;if(H[n]++>max)max=H[n]}END{for(i=0;i<24;i++){printf"%02d -%5d ",i,H[i];for(n=0;n<H[i]/max*50;n++){printf "*"}print""}}'
```

### Using Git Diff Without a Repo ([src](https://www.jvt.me/posts/2020/10/29/git-diff-no-repo/))

The --no-index flag allows you to diff between files that aren't related to a Git repo:

#### does not work, returns status code 0
`git diff README.md ../other-repo/README.md`
#### works, returns status code 1 and the diff
`git diff --no-index README.md ../other-repo/README.md`
