# 基于SpringBoot+Vue的实时热点新闻系统

![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) ![Vue3](https://img.shields.io/badge/-Vue3-grey?style=flat-square) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MyBatis](https://img.shields.io/badge/-MyBatis-000000?style=flat-square&logo=mybatis&logoColor=white) 

## 项目介绍

本系统是一款面向全网热点追踪与阅读互动的资讯门户平台（界面品牌：脉搏资讯），针对新闻热点分散、榜单与正文割裂、快讯难跟进、专题脉络不清等痛点，将今日要闻、实时热搜风云榜、7×24h 电报快讯、深度专题与跟帖互动整合到同一门户，支撑从发现焦点到阅读讨论的完整闭环。

系统采用 SpringBoot + Vue 前后端分离架构，区分普通读者与总编管理员：读者端完成频道筛选检索、热搜/快讯浏览、专题追踪、点赞收藏与评论；管理员在数据看板维护频道文章、快讯榜单、专题轮播与跟帖审核，并支持手动实时采集更新。适合作为毕设、课设与资讯聚合类学习参考。

## 主要功能模块

- **用户认证与双角色分流**：读者与管理员统一登录注册，JWT 鉴权；登录后按角色进入门户或总编后台，/admin 路由隔离
- **今日要闻门户**：焦点轮播、频道筛选、关键词检索、分页阅读与置顶热议标识
- **实时热搜风云榜**：多领域与爆/沸/热/新/升态势筛选，词条关联深度报道，支持手动实时获取
- **7×24h 电报快讯**：按领域与重要度筛选，红字重点预警，一键复制与关注互动
- **深度热点专题**：专题卡片、事件时间轴、关联报道聚合与追踪阅读
- **新闻详情与互动**：正文阅读、AI 速读摘要与舆情标签、推荐阅读、点赞收藏与跟帖评论（本人可删）
- **个人中心**：我的收藏、点赞、跟帖管理、头像资料与安全密码维护
- **总编数据看板**：关键运营指标与 ECharts 可视化，热搜 Top 监控
- **采编内容中台**：频道分类、热点文章审核编辑、快讯/热搜/专题/轮播维护
- **跟帖与用户治理**：评论精选与官方回复、用户启停重置、手动采集调度

## 技术架构

- **后端**：Spring Boot 2.7.18 + MyBatis-Plus + JWT + Lombok + Hutool
- **前端**：Vue 3 + TypeScript + Vue Router + Pinia + Element Plus + Vite + ECharts
- **数据库**：MySQL 8.0

<!-- screenshots-start -->
## 系统截图

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png" alt="登录页面" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E7%94%A8%E6%88%B7%E9%A6%96%E9%A1%B5.png" alt="用户首页" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E5%AE%9E%E6%97%B6%E7%83%AD%E6%90%9C%E6%A6%9C.png" alt="实时热搜榜" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E7%94%B5%E6%8A%A5%E5%BF%AB%E8%AE%AF.png" alt="电报快讯" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E6%96%B0%E9%97%BB%E8%AF%A6%E6%83%85.png" alt="新闻详情" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E7%AE%A1%E7%90%86%E5%91%98%E6%95%B0%E6%8D%AE%E7%9C%8B%E6%9D%BF.png" alt="管理员数据看板" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E5%90%8E%E5%8F%B0%E7%83%AD%E7%82%B9%E6%96%87%E7%AB%A0.png" alt="后台热点文章" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E8%87%AA%E5%8A%A8%E7%88%AC%E5%8F%96%E8%AE%BE%E7%BD%AE.png" alt="自动爬取设置" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E8%AE%BA%E6%96%87%E5%9B%BE1.png" alt="论文图1" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/%E8%AE%BA%E6%96%87%E5%9B%BE2.png" alt="论文图2" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/hotnews/UML%E5%9B%BE%E5%88%97%E8%A1%A8.png" alt="UML图列表" width="600" />

<!-- screenshots-end -->

---

## 接毕业设计和论文

### 作者微信：vvsgxmn  (支持修改、 部署调试、 支持代做毕设)

### 接网站建设、小程序

### 选题+开题报告+任务书+程序定制+安装调试+论文+答辩ppt 都可以做

### 购买地址：[https://www.vvxx.love](https://www.vvxx.love)（vv毕设网）

### 支持 **一键生成 UML 图**：上传项目压缩包即可自动产出功能模块图、用例图、流程图、E-R 图、时序图等全套毕设图表。

### 提供 **免费配套软件下载 + 安装说明 + 部署教程**

![vv毕设网 - 一键画图](https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/uml-draw.png)

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/image-20260825133349317.png" alt="image-20260825133349317" />

⚠️ Bug添加微信**免费修复**，免费修复。其他平台的私信一律不管（微信方便发送文件）
