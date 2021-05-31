# git命令
```
git add [File] 添加目录
git commit [File] [File]... -m '注释'
git status 显示XXX区状态
git reset --hard HEAD(^或^^或^^^或~回退数字)
git log (--pretty=oneline) 显示最近日志
git relog 获取版本好
git checkout (更新工作树中的文件以匹配索引或指定树中的版本。如果没有给出路径 - git checkout还会更新HEAD，将指定的分支设置为当前分支),不是太懂,这条命令会重写工作区。
rm [File] 可直接删除commit的文件，而后直接commit(永久删除)或从版本库中恢复被删文件
```