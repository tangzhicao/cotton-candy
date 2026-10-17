# 棉花糖的秘密 (The Secret of Cotton Candy) 🍬

> 互动式科普课件 · 3D 物理模拟实验台 · 棉花糖机 3D 拼装工坊

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=three.js&logoColor=white)
![WebGL](https://img.shields.io/badge/WebGL-990000?style=flat-square&logo=webgl&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-blue?style=flat-square)

---

## 📖 项目简介

《棉花糖的秘密》是一套面向青少年与创客工程教育的**沉浸式可交互课件**。通过水彩糖果艺术风格与极简工业风的融合，结合 **Three.js** 3D 渲染引擎，带学生探索棉花糖背后的历史文化、高中物理向心力与离心现象，以及微型棉花糖机的实物机械结构与组装原理。

---

## 🧭 页面导览

| 页面 | 主题 | 核心亮点 |
| :--- | :--- | :--- |
| **`index.html`** | 课程总览封面 | 梦幻糖果水彩背景、动态 3D 棉花糖展示、课程章节总览 |
| **`page2.html`** | 历史溯源与演变史 | 1897 年世博会诞生、百年演变交互时间轴与珍贵档案 |
| **`page3.html`** | 机器档案全景图 | 经典机型图文对比与现代化自动棉花糖机器人展示 |
| **`page4.html`** | 棉花糖的化学与物理 | 蔗糖晶体熔化、相变、冷却凝固成丝全过程 |
| **`page5.html`** | 制作四大步骤解析 | 加热液化、高速离心、喷射拉丝、快速降温 |
| **`page6.html`** | 离心力理论推导篇 | 高中物理圆周运动公式推导：$F_n = m \cdot r \cdot \omega^2$ 与临界极限平衡 |
| **`page7.html`** | 3D 物理交互实验台 | 实时可调参数（质量 $m$、半径 $r$、摩擦因数 $\mu$、转速 $\omega$），动态验证飞出临界条件 |
| **`page8.html`** | 第二部分总标题过渡页 | 深空全息科幻风格、动态星空全息名片、工程与制造章节引言 |
| **`page9.html`** | 3D 拼装工坊（编辑器模式） | 工业级深灰参考网格、Outliner 零件库、真实比例 3D 模型实物吸附拼装与电机转速演示 |

---

## 🛠️ 技术实现

1. **纯前端免构建**：原生 HTML5 + CSS3 + 现代 JavaScript (ES6+)，无需 Node.js 构建打包，零依赖快速部署。
2. **Three.js 3D 引擎**：
   - 离心运动物理粒子系统；
   - 参数化空间曲线 `HelixSpringCurve` 真实生成微型锥度螺旋弹簧；
   - 细致还原实物尺寸（如电池盒实测 5cm×3cm×1cm、双凹槽、铜花铆扣、刀闸开关等）；
   - 自研阻尼控制器 `CleanOrbitControls`，支持旋转、缩放与平移。
3. **响应式与毛玻璃美学**：多层 `backdrop-filter: blur()` 毛玻璃卡片与柔和投影，兼顾大屏演示与桌面交互。

---

## 🚀 本地运行

直接双击打开任意 `.html` 文件即可在现代浏览器（Chrome、Edge、Safari、Firefox）中运行；推荐使用 VS Code 插件 `Live Server` 或 Python 本地服务预览：

```bash
python -m http.server 8000
```
然后访问 `http://localhost:8000`。
