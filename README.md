# README
```wiki
@author Zeng Qi
@date 2022.12.1
```

[![zq-homepage](https://img.shields.io/badge/Zeng%20Qi's-Homepage-%234994c4?style=flat-square)](https://firstheart01.github.io/zq-homepage)
![LICENSE](https://img.shields.io/github/license/firstheart01/zq-homepage?style=flat-square)

非常感谢 [vuepress-theme-hope](https://vuepress-theme-hope.github.io/v2/) 所构建的主题以及 [rpg-homepage-template](https://ruopenggao.com) 编写的的模板。


## 写在前面 

本仓库主要使用了 [rpg-homepage-template](https://ruopenggao.com) 的模板，该仓库下已经有很完整的配置、指令和部署说明，可以照着该仓库下进行开发配置。

本人在服务器部署时，采用了Github Page，在配置过程中出现了一些问题进行记录。 

## 部署在 GitHub

vuepress-theme-hope 提供了非常简单的部署到 GitHub 的方法，可以先简单参考一下文档中 [部署项目](https://vuepress-theme-hope.github.io/v2/zh/cookbook/tutorial/deploy.html) 一章。

由于我的仓库名称不是\<Username\>.github.io的形式，因此在部署的网址是：\<Username\>.github.io.\<repo\>，所以需要在config.ts和theme.ts当中修改hostname，同时config.ts中的base也需要进行修改。

由于最开始我创建了工作流，使用了Github Actions进行部署，因此我在工作流中创建了一个分支，用于储存 vuepress build docs 产生的文件，但是不知道为什么使用工作流没有部署好，虽然提示部署成功，可域名还是无法访问，



值得注意的是，本仓库在使用 vuepress-theme-hope 建立之初，并没有创建 GitHub 工作流，因此需要根据教程进行创建；又或是可以选择 [直接创建 vuepress-theme-hope 的运行环境](https://vuepress-theme-hope.github.io/v2/zh/cookbook/tutorial/env.html)，在创建过程中选择创建 GitHub 工作流，并且将本仓库中的文件替换到创建好的运行环境中即可。