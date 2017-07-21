# 文档系统说明

## 目的
将零散的文档通过Html页面的形式有效**组织**和**链接**在一起。
## 使用MarkDown
>强烈推荐使用MarkDown进行文档的编写，这将方便显示在此页面上。

## Word转markdown
>使用[Word to Markdown Converter](https://word-to-markdown.herokuapp.com/) 工具将已有的word转换成md文件，再在此基础上进行修改。

## 如何管理文档
>1. 暂时使用SMB也即是局域网共享管理文档的存放。
SMB路径
>```text
>.
>├── docs
>|   └── README.md 主页
>|   └── designerdoc 设计文档
>|       └──A.md
>|       └──B.md
>|   └── usermanual 用户手册
>|        └──usermanual.md
>|   └── changelog  更新说明
>|       └──changelog.md sdk更新说明
>|       └──desktopchangelog.md  desktop更新说明
>```
>2. 当想纳入不在此路径上文档时，通过mklink建立基于文件系统的符号链接**备注：局域网的文件可能无法通过硬链接进行使用**  


## 添加SDK文档
使用第三方工具生成的页面，使用超链接的形式链接到此文档中。

## 部署文档系统
>使用Nodejs  
>文档的实时修改会自动刷新页面

```bash
npm i docsify-cli -g
docsify serve docs
```
>使用Python  
>需要手动刷新页面
```bash
cd docs && python -m SimpleHTTPServer 3000
```

## 外网使用






