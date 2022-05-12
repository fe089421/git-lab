1.  
git version 2.36.1

2. 
fredentsie@Freds-MacBook-Pro git-lab % git config --list
credential.helper=osxkeychain
user.name=fred entsie
user.email=fe089421@ohio.edu
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true

3.
pops up commands used in various situations


4.
fredentsie@Freds-MacBook-Pro git-lab % git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   answers.md

no changes added to commit (use "git add" and/or "git commit -a")
fredentsie@Freds-MacBook-Pro git-lab % 

5.
fredentsie@Freds-MacBook-Pro git-lab % git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   answers.md

no changes added to commit (use "git add" and/or "git commit -a")
fredentsie@Freds-MacBook-Pro git-lab % git add README.md
fredentsie@Freds-MacBook-Pro git-lab % git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   answers.md

fredentsie@Freds-MacBook-Pro git-lab % 


6.
fredentsie@Freds-MacBook-Pro git-lab % git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   answers.md

no changes added to commit (use "git add" and/or "git commit -a")
fredentsie@Freds-MacBook-Pro git-lab % git add README.md
fredentsie@Freds-MacBook-Pro git-lab % git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   answers.md

fredentsie@Freds-MacBook-Pro git-lab % git add answers.md
fredentsie@Freds-MacBook-Pro git-lab % git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        modified:   answers.md

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   answers.md

fredentsie@Freds-MacBook-Pro git-lab % 

7.
fredentsie@Freds-MacBook-Pro git-lab % git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   answers.md

no changes added to commit (use "git add" and/or "git commit -a")
fredentsie@Freds-MacBook-Pro git-lab % 

8.
redentsie@Freds-MacBook-Pro git-lab % git log
commit b3e93e6e0ecf8a407d0115b5ddb0a1571762cbb3 (HEAD -> main)
Author: fred entsie <fe089421@ohio.edu>
Date:   Thu May 12 08:28:34 2022 -0400

    Initial commit

commit 9c829df011cec140d15f2a81b820bc4d3724d18d
Author: fe089421@ohio.edu <fe089421@ohio.edu>
Date:   Thu May 12 08:08:38 2022 -0400

    first commit

commit c0f0cdeb5573477263141a1fff294333ccd9acaa
:...skipping...
commit b3e93e6e0ecf8a407d0115b5ddb0a1571762cbb3 (HEAD -> main)
Author: fred entsie <fe089421@ohio.edu>
Date:   Thu May 12 08:28:34 2022 -0400

    Initial commit

commit 9c829df011cec140d15f2a81b820bc4d3724d18d
Author: fe089421@ohio.edu <fe089421@ohio.edu>
Date:   Thu May 12 08:08:38 2022 -0400

    first commit

commit c0f0cdeb5573477263141a1fff294333ccd9acaa
Author: Fred Entsie <fe089421@ohio.edu>
Date:   Tue May 10 20:08:05 2022 -0400

    here

commit 79b1f8fe8cd8ac069be2ac8ef8b39d0a704686e0
Author: Fred Entsie <fe089421@ohio.edu>
:

9.

fredentsie@Freds-MacBook-Pro git-lab % git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   answers.md

no changes added to commit (use "git add" and/or "git commit -a")
fredentsie@Freds-MacBook-Pro git-lab % 

10.
No the changes did not reflect in my local copy

11.fredentsie@Freds-MacBook-Pro git-lab % git push
To https://github.com/fe089421/git-lab.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/fe089421/git-lab.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

12.The changes were made in my local copy

13.fredentsie@Freds-MacBook-Pro git-lab % ls -a
.               ..              .git            README.md       answers.md      git-lab-2
