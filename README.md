# Git Fire

众所周知，火灾自救有以下步骤（大雾

![](/imgs/01.jpg)

担心遇到火灾时来不及上传代码而错失逃离良机？

草草上传却突然遭遇冲突需要合并？

别担心！使用 Git Fire 可以让你更加从容！

当同事还在一行一行地敲着 git 命令，又或是焦头烂额地处理冲突时，

你只需要 `git fire` ，就可以立刻逃离现场！

---

在 bash 执行以下命令

```bash
git config --global alias.fire "! f() { git checkout -b fire ; git add . ; git commit -m \"A fire has occurred\" ; git push origin fire:fire ; }; f"
```

或在你的 `.gitconfig` 文件中加入如下内容

```
[alias]
	fire = "! f() { git checkout -b fire ; git add . ; git commit -m \"A fire has occurred\" ; git push origin fire:fire ; }; f " 
```

之后，你就可以愉快地使用 `git fire` 来紧急上传代码啦！