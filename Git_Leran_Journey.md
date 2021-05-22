Git_Leran_Journey

---

#### 基本命令快速查找:



创建目录: `mkdir`

移动到某目录: `cd`

显示当前目录: `pwd`

把这个目录变成Git可以管理的仓库：`git init`

如果没有看到`.git`目录，那是因为这个目录默认是隐藏的，用`ls -ah`命令

用记事本来写文件: `vi 文件名`,退出按esc后打入`:wq`

把文件**添加**到仓库: `git add 文件名`

把文件**提交**到仓库: `git commit -m "xxx"`

---

#### 一些特殊操作和注意点:



为什么Git添加文件需要`add`，`commit`一共两步呢？因为`commit`可以一次提交很多文件，所以你可以多次`add`不同的文件，比如：

`$ git add file1.txt`

`$ git add file2.txt file3.txt`

`$ git commit -m "add 3 files."`



---

#### 疑难解答:

Q：输入`git add readme.txt`，得到错误：`fatal: not a git repository (or any of the parent directories)`。

A：Git命令必须在Git仓库目录内执行（`git init`除外），在仓库目录外执行是没有意义的。



Q：输入`git add readme.txt`，得到错误`fatal: pathspec 'readme.txt' did not match any files`。

A：添加某个文件时，该文件必须在当前目录下存在，用`ls`或者`dir`命令查看当前目录的文件，看看文件是否存在，或者是否写错了文件名。



