optimus@optimus:~/Desktop/PLPBasicGitAssignment$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint:   git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint:   git branch -m <name>
Initialized empty Git repository in /home/optimus/Desktop/PLPBasicGitAssignment/.git/

optimus@optimus:~/Desktop/PLPBasicGitAssignment$ git config --global init.defaultBranch main
optimus@optimus:~/Desktop/PLPBasicGitAssignment$ git branch -m main
optimus@optimus:~/Desktop/PLPBasicGitAssignment$ git remote add origin https://github.com/Xylento/PLPBasicGitAssignment.git
optimus@optimus:~/Desktop/PLPBasicGitAssignment$ git add hello.txt
optimus@optimus:~/Desktop/PLPBasicGitAssignment$ git commit -m "Add hello.txt with a greeting"
[main (root-commit) f4389ab] Add hello.txt with a greeting
 1 file changed, 1 insertion(+)
 create mode 100644 hello.txt
 
optimus@optimus:~/Desktop/PLPBasicGitAssignment$ git push -u origin main
To https://github.com/Xylento/PLPBasicGitAssignment.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Xylento/PLPBasicGitAssignment.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

optimus@optimus:~/Desktop/PLPBasicGitAssignment$ git push --force origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 238 bytes | 238.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Xylento/PLPBasicGitAssignment.git
 + c22774e...f4389ab main -> main (forced update)


The following are the command i used and i was able to find the error and understand since am pushing to a repo that has a readme while locally i didn't have the readme
