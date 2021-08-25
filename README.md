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

- ===想要在本地clone自己的私人项目的时候，为了私人项目的安全，就需要加上账号与密码进行验证==

[new way: token required](https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/)


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
