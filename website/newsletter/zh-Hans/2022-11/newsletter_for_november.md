---
title: "Taichi 十一月社区月报"
date: "2022-12-01"
description:
  📌 十一月高光时刻\ Taichi 发布 v1.3.0 版本\官宣吉祥物赛博飞鼠\ Hackathon 圆满完赛
---

# Taichi 2022 年 11 月社区月报

## 📌十一月高光时刻

- Taichi 发布 v1.3.0 版本
- Taichi 官宣吉祥物，超萌表情包同步上线
- DEM 代码优化大赛结束，获奖名单揭晓
- 首届 Taichi Hackathon 圆满结束，10 支赛队获奖

##  ⚙️ 技术动态

**🔧 Taichi v1.3.0 发布！看看有哪些重要更新**

- Dynamic SNode 现支持各种基本数据类型以及 Matrix、Struct 等复杂数据类型。
- CUDA 后端目前也支持稀疏矩阵。
- Packed mode 现成为默认模式。
- 废弃了 Metal 后端的稀疏数据结构。

有关此版本的更多更新，请参阅完整的 [变更日志](https://github.com/taichi-dev/taichi/releases/tag/v1.3.0)

赶快升级体验新功能吧 👉 `pip install -U taichi==1.3.`

**📃 Taichi Cheatsheet 发布**

我们将 Taichi 的基础概念和常用 API 提炼出来浓缩在一页 A4 纸中，作为速查表方便大家浏览，Cheatsheet 也会持续更新哦。

![](https://user-images.githubusercontent.com/124654014/217705261-f2d6849d-442c-422e-9001-32772b1bd6d8.png)

视频详解请点击 [这里](https://www.bilibili.com/video/BV11Y411d7n2/?spm_id_from=333.999.0.0)

✔️ 本月合并 231 个 PR，解决 39 个 Issue。

## 🌟 社区精选作品

- [有限元求解器 FEMcy](https://github.com/mo-hanxuan/FEMcy)。

mo-hanxuan 完成了一个基于 Taichi 的有限元求解器 FEMcy。FEMcy 具有良好的可移植性并且是开源的，可以灵活地满足用户的需求。
  
![](https://user-images.githubusercontent.com/124654014/217705579-17d072e7-c5b1-42fb-a84d-b4e8c61d0607.gif)
  
- [三维离散元的 linear contact model](https://github.com/Yihao-Shi/TaichiDEM/tree/version-updated)

Yihao-shi 实现了三维离散元的 linear contact model。加入了库伦摩擦定律以及 rolling、twisting 的计算，使得球形颗粒能做出非球形颗粒的效果，并使用 Taichi 写了几个简单的四元数函数，完整地考虑了颗粒的旋转与方位。

![](https://user-images.githubusercontent.com/124654014/217714364-341564b5-b42a-41f8-95b4-9bef6506eb82.gif)

## 📢 社区活动

**[🔵 用 Taichi 实现 Instant NGP (NeRF) 的渲染器](https://forum.taichi-lang.cn/t/topic/3368)**

主讲人林尤添，是哈尔滨工业大学电子信息工程学院在读博士研究生，在这次分享中，向我们介绍了如何用 Taichi 实现 Instant NGP——Instant NGP 是加速 NeRF 训练和渲染的新方法 (SIGGRAPH 2022）。

视频详解请点击 [这里](https://www.bilibili.com/video/BV1xR4y117cU/?spm_id_from=333.999.0.0&vd_source=7e8cfbc83bcd0c8522627c6544d35724)

**[👨‍🏫 Git & GitHub 基础知识和实用技巧](https://forum.taichi-lang.cn/t/topic/3368)**

Taichi 编译器工程师 Ailing 和研究员包乾带来了详尽的实战操作演示，挑选出 Git 和 GitHub 工作中容易忽视的细节，进行突击式讲解。

视频详解请点击 [这里](https://www.bilibili.com/video/BV1xG4y1V7K1/?spm_id_from=333.999.0.0)

**[⌨️ DEM 代码优化挑战赛结束](https://mp.weixin.qq.com/s/07RRRp3knjqSwQaGDQKtLA)**

挑战赛共收到 9 个优秀投稿。经过大众评审投票和评委打分，最终诞生了一二三等奖和最佳人气奖。

![](https://user-images.githubusercontent.com/124654014/217713869-db5fcc67-f741-418a-bfd1-73afb7e7961c.gif)


**[🏆 首届 Taichi Hackathon 圆满结束](https://mp.weixin.qq.com/s/S02iUxsw1PJagwsdhWVKlQ)**

最终有 30 支队伍参与答辩，10 支赛队分获一二三等奖、最佳创意、最佳交互、最佳硬件、最佳潜力和极客奖。

![](https://user-images.githubusercontent.com/124654014/217713981-c95a17ae-773b-4772-b4a7-dfc5b3e251ea.gif)


## 🧑‍💻 如何成为 Taichi 贡献者

欢迎大家参与 Taichi 开发，这里有一些 issue 欢迎大家尝试解决：
- `taichi.lang.util.warning` doesn't respect stdlib `warnings` filters #4543
- Unexpect exit of ggui window after clicking Alt, Shift or Ctrl  #6513

更多 good first issue（非常容易上手） 和  welcome contribution （稍微带有挑战性）的 issue [请点击这里](https://github.com/taichi-dev/taichi/contribute)

**期待更多同学加入贡献者的队伍之中，特别送上几则小贴士：**

- **[Taichi 贡献者指南](https://docs.taichi-lang.org/docs/contributor_guide)**
 
   一文带大家读懂如何成为 Taichi 贡献者，解释了具体的行为规范，也包含了实用小技巧，便于大家快速上手。
- **[Taichi 编程语言的开发进度面板](https://github.com/orgs/taichi-dev/projects/1)**
 
   便于大家快速了解 Taichi 未处理/进展中/已处理/已完成开发的 issue。 
   
- **[加入 GitHub discussion](https://github.com/taichi-dev/taichi/discussions)**
 
   在这里你可以与海内外开发者一起讨论功能开发、Taichi roadmap 等话题，也欢迎提出你对 Taichi 的建议。
 
- **[Awesome Taichi](https://github.com/taichi-dev/awesome-taichi)**
 
   精选社区同学用 Taichi 做出的优质项目，可以从中找到感兴趣的例子尝试运行。 
