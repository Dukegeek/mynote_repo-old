# git提交规范(弱约束)
## 提交格式
```
<type><scope>:<subject>
<body>
<footer>
```
## 格式叙述
1. type：
```
feat:新功能、新特性
fix:修复bug
perf: 更改代码，以提高性能（在不影响代码内部行为的前提下，对程序性能进行优化）
refactor: 代码重构（重构，在不影响代码内部行为、功能下的代码修改）
docs: 文档修改
style: 代码格式修改, 注意不是 css 修改（例如分号修改）
test: 测试用例新增、修改
build: 影响项目构建或依赖项修改
revert: 恢复上一次提交
ci: 持续集成相关文件修改
chore: 其他修改（不在上述类型中的修改）
release: 发布新版本
workflow: 工作流相关文件修改
```
2. scope
```
commit影响范围，如：route，component，utils，build
```
3. subject
```
commit概述：modify1->modify2
```
4. body
```
多行修改内容
```
5. footer
```
备注，常为BREAKING CHANGE，修复链接，关联的合并要求,reviewer
```
## 代码示例
```
(某一次提交：把笔记的TXT格式改为Markdown形式)git commit [File] -m '规范'
规范：
docs(globe)!:txt->md
把笔记的TXT格式改为Markdown形式
BREAKING CHANGE
```