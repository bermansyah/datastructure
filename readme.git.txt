git --version

C:\Users\BRI>git --version
git version 2.17.0.windows.1

git config --global user.name bdy
 
git config --global user.email bermansyah@gmail.com

git config --list

C:\Users\BRI>git config --list
core.symlinks=false
core.autocrlf=true
core.fscache=true
color.diff=auto
color.status=auto
color.branch=auto
color.interactive=true
help.format=html
rebase.autosquash=true
http.sslcainfo=C:/development/Git/mingw64/ssl/certs/ca-bundle.crt
http.sslbackend=openssl
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
credential.helper=manager
user.name=bdy
user.email=bermansyah@gmail.com

===

cd \project.git\web

git init
D:\project.git\web>git init
Initialized empty Git repository in D:/project.git/web/.git/

git status
D:\project.git\web>git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        index.html

nothing added to commit but untracked files present (use "git add" to track)

git add .

git commit -m "first commit"
D:\project.git\web>git commit -m "first commit"
[master (root-commit) 2e9a693] first commit
 1 file changed, 8 insertions(+)
 create mode 100644 index.html

git log --oneline
D:\project.git\web>git log --oneline
2e9a693 (HEAD -> master) first commit

git add .

git commit -m "second commit"
D:\project.git\web>git commit -m "second commit"
[master 0102519] second commit
 2 files changed, 10 insertions(+)
 create mode 100644 templates/template.html

git checkout 0102519 index.html

git checkout -- index.html

===

https://github.com/login
user: bermansyah@gmail.com
pass: Bdy@103004

git remote add origin https://github.com/bermansyah/web

git push -u origin master --force
D:\project.git\web>git push -u origin master --force
Counting objects: 7, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (5/5), done.
Writing objects: 100% (7/7), 613 bytes | 153.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/bermansyah/web
 + 526dc8e...0102519 master -> master (forced update)
Branch 'master' set up to track remote branch 'master' from 'origin'.

cd \project.git\clone
git clone https://github.com/bermansyah/web
D:\project.git\clone>git clone https://github.com/bermansyah/web
Cloning into 'web'...
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 7 (delta 1), reused 7 (delta 1), pack-reused 0
Unpacking objects: 100% (7/7), done.


