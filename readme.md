当图片数量过多时，便从分支br_template 创建一个新的空分支。

然后修改picgo，新图片都用这个分支。



```scala
# 使用 SSH 克隆指定分支
git clone git@github.com:mafulong/mdPic.git

# 切换到克隆的目录
cd mdPic

git checkout br_template

# 创建新分支并切换到该分支
NewName=v9
git checkout -b $NewName

# rename images 文件夹
mv images $NewName

# 推送新分支到远程仓库
git push --set-upstream origin $NewName
```

