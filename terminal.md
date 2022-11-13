Last login: Sun Nov 13 16:39:32 on ttys000
sergey@MacBook-Air-Sergey TEST % git init
Initialized empty Git repository in /Users/sergey/TEST/.git/
sergey@MacBook-Air-Sergey TEST % git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	README.md

nothing added to commit but untracked files present (use "git add" to track)
sergey@MacBook-Air-Sergey TEST % git add readmi.md
fatal: pathspec 'readmi.md' did not match any files
sergey@MacBook-Air-Sergey TEST % git add README.md
sergey@MacBook-Air-Sergey TEST % git status       
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   README.md

sergey@MacBook-Air-Sergey TEST % git commit -m "README.md"
[main (root-commit) c3c1d47] README.md
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
sergey@MacBook-Air-Sergey TEST % git commit -m "add README"   
On branch main
nothing to commit, working tree clean
sergey@MacBook-Air-Sergey TEST % git commit -m "add README"
On branch main
nothing to commit, working tree clean
sergey@MacBook-Air-Sergey TEST % git status                
On branch main
nothing to commit, working tree clean
sergey@MacBook-Air-Sergey TEST % git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
sergey@MacBook-Air-Sergey TEST % git add README.md
sergey@MacBook-Air-Sergey TEST % git commit -m "change README"
[main cbbe9a1] change README
 1 file changed, 3 insertions(+), 1 deletion(-)
sergey@MacBook-Air-Sergey TEST % git log --oneline
cbbe9a1 (HEAD -> main) change README
c3c1d47 README.md
sergey@MacBook-Air-Sergey TEST % git log          
commit cbbe9a1faceb4c56f5e659506763f1a80e8ac912 (HEAD -> main)
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:45:28 2022 +0200

    change README

commit c3c1d47cc7ac2a161d44ce24923bc5a2bd40e520
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:33:54 2022 +0200

    README.md
sergey@MacBook-Air-Sergey TEST % git status                   
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
sergey@MacBook-Air-Sergey TEST % git commit -m "README"       
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
sergey@MacBook-Air-Sergey TEST % git commit add README.md
error: pathspec 'add' did not match any file(s) known to git
sergey@MacBook-Air-Sergey TEST % git add README.md 
sergey@MacBook-Air-Sergey TEST % git commit -m "README"  
[main d84b803] README
 1 file changed, 3 insertions(+), 1 deletion(-)
sergey@MacBook-Air-Sergey TEST % git status              
On branch main
nothing to commit, working tree clean
sergey@MacBook-Air-Sergey TEST % git log                 
commit d84b803c92d7d1788794af33623b8439b3a9fa90 (HEAD -> main)
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:56:07 2022 +0200

    README

commit cbbe9a1faceb4c56f5e659506763f1a80e8ac912
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:45:28 2022 +0200

    change README

commit c3c1d47cc7ac2a161d44ce24923bc5a2bd40e520
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:33:54 2022 +0200

    README.md
sergey@MacBook-Air-Sergey TEST % git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	errors.md

nothing added to commit but untracked files present (use "git add" to track)
sergey@MacBook-Air-Sergey TEST % git add errors.md
sergey@MacBook-Air-Sergey TEST % git commit --m "ërror"   
[main f9e8d42] ërror
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 errors.md
sergey@MacBook-Air-Sergey TEST % git commit --amend --m "error"
[main aa86837] error
 Date: Sun Nov 13 17:59:56 2022 +0200
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 errors.md
sergey@MacBook-Air-Sergey TEST % git status                    
On branch main
nothing to commit, working tree clean
sergey@MacBook-Air-Sergey TEST % git log                       
commit aa86837ac4b6a950aa4d95d46ac33721d5a02ffe (HEAD -> main)
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:59:56 2022 +0200

    error

commit d84b803c92d7d1788794af33623b8439b3a9fa90
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:56:07 2022 +0200

    README

commit cbbe9a1faceb4c56f5e659506763f1a80e8ac912
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:45:28 2022 +0200

    change README

commit c3c1d47cc7ac2a161d44ce24923bc5a2bd40e520
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:33:54 2022 +0200

    README.md
sergey@MacBook-Air-Sergey TEST % git checkout c3c1d47cc7ac2a161d44ce24923bc5a2bd40e520
Note: switching to 'c3c1d47cc7ac2a161d44ce24923bc5a2bd40e520'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at c3c1d47 README.md
sergey@MacBook-Air-Sergey TEST % git log                                              
commit c3c1d47cc7ac2a161d44ce24923bc5a2bd40e520 (HEAD)
Author: Sergey Primaxx <primaxx66@icloud.com>
Date:   Sun Nov 13 17:33:54 2022 +0200

    README.md
sergey@MacBook-Air-Sergey TEST % git log --oneline --all
aa86837 (main) error
d84b803 README
cbbe9a1 change README
c3c1d47 (HEAD) README.md
sergey@MacBook-Air-Sergey TEST % git -                                                
unknown option: -
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]
sergey@MacBook-Air-Sergey TEST % git checkout -                                       
Previous HEAD position was c3c1d47 README.md
Switched to branch 'main'
sergey@MacBook-Air-Sergey TEST % git status                                           
On branch main
nothing to commit, working tree clean
sergey@MacBook-Air-Sergey TEST % 
