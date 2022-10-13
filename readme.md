# Git exercice
## Bundle 1
### exercice 1
```bash
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git init                        
Initialized empty Git repository in C:/Users/TheGym/Desktop/tutorial-projects/Gym-Git-Exercise-Solutions/.git/
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git branch -M main
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git commit -m "initial git project"
 1 file changed, 1 insertion(+)
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git remote add origin https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 245 bytes | 245.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
branch 'main' set up to track 'origin/main'.
Everything up-to-date
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git checkout -b dev
Switched to a new branch 'dev'
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push 
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use


To have this happen automatically for branches without a tracking

Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/NNesta/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/NNesta/Gym-Git-Exercise-Solutions/pull/new/test
remote:
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
 * [new branch]      test -> test
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git branch -D test
Deleted branch test (was 78b4987).
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push origin --delete test
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
 - [deleted]         test
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> 
```

## Bundle 2
### Exercice 1
```bash
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git checkout -b ft/bundle-2
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git add services.html
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git commit -m "adding service page "
[ft/bundle-2 8b6dd56] adding service page
 1 file changed, 12 insertions(+)
 create mode 100644 services.html
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use
    git push --set-upstream origin ft/bundle-2
To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 487 bytes | 243.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/NNesta/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```

## Exercice 2
```bash
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git pull
Already up to date.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git checkout -b ft/se
Switched to a new branch 'ft/service-redesign'
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git add services.html
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git commit -m "adding some changes on services.html"
[ft/service-redesign e0634be] adding some changes on services.html
 1 file changed, 3 insertions(+), 3 deletions(-)
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use
    git push --set-upstream origin ft/service-redesign
upstream, see 'push.autoSetupRemote' in 'git help config'.

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 398 bytes | 132.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push --set-upstream origin ft/service-redesign
git push --set-upstream origin ft/service-redesign
upstream, see 'push.autoSetupRemote' in 'git help config'.

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 398 bytes | 132.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git add -all
error: did you mean `--all` (with two dashes)?
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git add --all
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git commit -m "feat: add list of services"
[main 17f0774] feat: add list of services
 1 file changed, 7 insertions(+)
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 383 bytes | 191.00 KiB/s, done.
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
   5ddf525..17f0774  main -> main
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git diff
diff --cc services.html
index dfc08ec,187ab2e..0000000
--- a/services.html
+++ b/services.html
@@@ -7,8 -7,15 +7,21 @@@
      <title>Document</title>
  </head>
  <body>
++<<<<<<< HEAD
 +    <h1>New Service Page</h1>
 +    <p>Welcome to service page redesigned</p>
 +   <button>Login here again for the redesigned page</button>
++=======
+     <h1>Service Page</h1>
+     <p>Welcome to service page</p>
+    <ul>
+     <li>Servise 1</li>
+     <li>Servise 2</li>
+     <li>Servise 3</li>
+     <li>Servise 5</li>
+    </ul>
++>>>>>>> main
  </body>
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
   e0634be..a8b080f  ft/service-redesign -> ft/service-redesign
   PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git commit  
[ft/service-redesign d0a8849] feat: merging with main branch
 1 file changed, 100 insertions(+)
 PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.28 KiB | 653.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/NNesta/Gym-Git-Exercise-Solutions.git
   a8b080f..d0a8849  ft/service-redesign -> ft/service-redesign
PS C:\Users\TheGym\Desktop\tutorial-projects\Gym-Git-Exercise-Solutions> 
```

