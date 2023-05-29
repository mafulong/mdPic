当图片数量过多时，便从分支br_template 创建一个新的空分支。

然后修改picgo，新图片都用这个分支。



由于repo过大，下载仓库时使用以下命令。

```scala
git clone --single-branch --branch br_template https://github.com/mafulong/mdPic.git
git co -b v8
git push
```

