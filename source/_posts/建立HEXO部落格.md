---
title: 建立HEXO部落格
date: 2024-05-28 10:00:00
tags:
 - HEXO
 - GitHub
categories: HEXSCHOOL
description: 建立 HEXO 部落格並將其部署到 GitHub Pages 是一個快速而有效的方法來建立個人部落格或網站。HEXO 是一個基於 Node.js 的靜態網站生成器，它可以幫助你快速建立並管理部落格內容，而 GitHub Pages 則是一個由 GitHub 提供的免費靜態網站主機服務，你可以將你的 HEXO 部落格部署到 GitHub Pages 上。
---


## 只要一到指令，瞬間建立一則部落格！

### 常用Hexo指令

    * hexo new ‘文章名稱’
    * hexo server
    * hexo generate - 用於public
    * hexo clean - 清除暫存
    * hexo deploy - 部屬
    
Hexo + GitHub Pages 官方部署說明 [連結](https://hexo.io/zh-tw/docs/github-pages#%E4%B8%80%E9%8D%B5%E9%83%A8%E5%B1%AC)

    1. 安裝 hexo-deployer-git.
        npm install hexo-deployer-git --save

    2. 清空 _config.yml 的現有資料，並新增以下組態:
        deploy:
            type: git
            repo: https://github.com/<username>/<project>
            # example, https://github.com/hexojs/hexojs.github.io
            branch: gh-pages

    3. 執行 hexo clean && hexo deploy
    4. 瀏覽 <GitHub 用戶名>.github.io 檢查你的網站能否運作。

### 等待Settings/Pages

網頁無法載入模板，請設定url 