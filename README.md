# GitCommandCheatTable
Git命令速查表

master: 默认开发分支   |    Head : 默认开发分支
orgin: 默认远程版本库  |    Head^ : Head的父提交

## 创建版本库
`$ git clone <url>`         克隆远程版本库
`$ git init`                初始化本地版本库

## 修改和提交
`$ git status`                      查看状态
`$ git diff`                        查看变更内容
`$ git add .`                       跟踪所有改动过的文件
`$ git add <file>`                  跟踪指定的文件
`$ git mv <old> <new>`              文件改名
`$ git rm <file>`                   删除文件
`$ git rm --cached <file>`          停止跟踪文件但不删除
`$ git commit -m "commit message"`  提交所有更新过的文件
`$ git commit --amend`              修改最后一次提交

## 查看提交历史
`$ git log`                         查看提交历史
`$ git long -p <file>`              查看指定文件的提交历史
`$ git blame <file>`                以列表方式查看指定文件的提交历史

## 撤销
`$ git reset --hard HEAD`           撤销工作目录中所有未提交文件的修改内容
`$ git checkout HEAD <file>`        撤销指定的未提交文件的修改内容
`$ git revert <commit>`             撤销指定的提交

## 分支与标签
`$ git branch`                      显示所有本地分支
`$ git checkout <branch/tag>`       切换到指定分支或标签
`$ git branch <new-branch>`         创建新分支
`$ git branch -d <branch>`          删除本地分支
`$ git tag`                         列出所有本地标签
`$ git tag <tagname>`               基于最新提交创建标签
`$ git tag -d <tagname>`            删除标签
