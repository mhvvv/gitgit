```bash
git ls-files  # 查看暂存区文件
```

```bash
git status

git status -s

# 第一列表示暂存区状态，第二列表示工作区抓那个太
U:  untrack   #  未跟踪的新文件
A:  add       #  新添加到Git暂存的文件(之前版本未记录此文件)
M:  modified  #  工作区内容产生变化的文件
```

```bash
git restore _file      # 放弃工作区内容，使用暂存区版本覆盖

git rm --cached _file  # 从暂存区移除文件
```

```bash
git log

git log --oneline
```

```bash
# git 回退版本  (从版本库回退)
                             #  工作区   暂存区       版本库
git reset --soft _version    #  保留     覆盖    <-  _version
git reset --hard             #  覆盖     覆盖
git reset (--mixed)          #  保留     覆盖
```

```bash
git branch _name       # 创建分支
git checkout _name     # 切换分支
git checkout -b _name  # both
```

