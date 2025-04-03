# Git-Notes

### print log

```
git log master > xxx.log
```

>此命令用于查看master分支的提交记录（commit history）

<br>

```
git log --name-only --pretty=format:"%h - %an, %ad : %s" --date=format:%Y/%m/%d HEAD > xxx.log
```

>--name-only 显示每个提交所修改的文件名。这些文件名会附加在日志信息后。<br><br>
>--pretty=format:"%h - %an, %ad : %s" 使用自定义格式显示提交记录，其中：<br>
>%h：显示提交的缩短哈希值（短 ID）。<br>
>%an：显示提交的作者姓名。<br>
>%ad：显示提交的日期。<br>
>%s：显示提交的简要信息（commit message）。<br><br>
>--date=format:%Y/%m/%d：指定日期格式为 年/月/日。<br><br>
>HEAD：表示当前分支的最新提交，及其之前的提交记录。<br>
