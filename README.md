# skills to git and github

There are some skills using `git and github` in `Windows 8`.

## ssh keygen
* ��`bash.exe` 
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
* ��½`GitHub`����`Account settings`��`SSH Keys`ҳ�棺

��`Add SSH Key`����������Title����Key�ı�����ճ��`id_rsa.pub`�ļ�������

## add the remote repository

* in GitHub��`Create a new repo`

Repository name����`gitlearn`����������Ĭ�����ã������Create repository����ť

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