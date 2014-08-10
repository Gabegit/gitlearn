# skills to git and github

There are some skills using `git and github` in `Windows 8`.

## ssh keygen
* 打开`bash.exe` 
```
ssh-keygen -t rsa -C "email@yourgithub.com"
input id_rsa
enter
```
* copy the `id_rsa and id_rsa.pub` to `.ssh` in /c/Users/.ssh/

```
id_rsa
id_rsa.pub
known_hosts
```
* 登陆`GitHub`，打开`Account settings`，`SSH Keys`页面：

点`Add SSH Key`，填上任意Title，在Key文本框里粘贴`id_rsa.pub`文件的内容

## add the remote repository

* in GitHub，`Create a new repo`

Repository name填入`gitlearn`，其他保持默认设置，点击“Create repository”按钮

* Push an existing repository from the local computer command line

fisrt time

```
git remote add origin git@github.com:Gabegit/gitlearn.git
git push -u origin master
```

* Create a new repository on the command line

```
touch README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:Gabegit/gitlearn.git
git push -u origin master
```
* push changed local repository to remote one 

```
$ git push origin master
```