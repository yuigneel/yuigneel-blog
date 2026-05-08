<div align="center">
  <img src="https://avatars.githubusercontent.com/u/202588416?s=400&u=baab8feb9dfc2e334858b649c91045a1be6f39f5&v=4" width="200" height="200" />


<h1><a href="https://yuigneel-blog.vercel.app/" target="_blank" rel="noopener noreferrer">yuigneel-blog</a></h1>

  <p>
    <a href="README.md">简体中文</a> | 
    <a href="README_EN.md">English</a>
  </p>
</div>

---

## 项目介绍

### 简介

- 本项目是一个由[AmisKwok](https://github.com/AmisKwok)开源的代码为基础改编，基于Next.js+React+TypeScript+TailwindCSS的开源博客项目。
- 目前项目仅用于目的**仅用于个人学习**，代码**仅供学习**，如有问题，**原作者和我均不背书**，想制作属于自己的博客**可以拷贝本仓库
  **，但**推荐**移步到[**源作者仓库**](https://github.com/AmisKwok/AmisHomepage)

### 功能特性

- 🎨 **现代化设计**
    - 全屏背景图 + 渐变遮罩
    - 动态背景（暗色：星空，亮色：落叶）

- ✍️ **SVG 绘画标题**
    - 手写风格标题
    - 动态计算 viewBox

- ⌨️ **打字机效果**
    - 动态打字机文字效果
    - 支持多文本循环

- 🎭 **故障效果**
    - 可配置的故障抖动动画
    - 支持自定义触发概率和间隔

- 🌈 **颜色渐变**
    - 动态彩色渐变效果（仅暗色主题）

- 👤 **头像动画**
    - 呼吸光圈效果
    - 悬停放大 + 多层光晕

- 🔗 **社交链接**
    - 背景图中心展示
    - 涟漪点击效果
    - 悬停光晕

- 📋 **关于我卡片**
    - 从 GitHub README 加载个人信息
    - 技能标签悬停效果

- 🌟 **精选项目**
    - 展示项目卡片
    - 支持边框流光、阴影扩散、图片遮罩动画

- 📊 **技能可视化**
    - 进度条展示技术栈
    - 数字动画效果

- 🌍 **多语言支持**
    - 支持中文/英文切换
    - 自动检测系统语言

- 🌓 **主题切换**
    - 支持亮色/暗色模式切换
    - 默认暗色主题
    - 模糊过渡动画
    - 主题适配所有组件

- 🕐 **时间组件**
    - 左上角显示本地时间和日期
    - 点击展开日历
    - 平滑宽度过渡动画

- 🖱️ **自定义鼠标指针**
    - 支持自定义鼠标指针样式
    - 可上传 .cur 文件

- 📱 **响应式布局**
    - 完美适配桌面端和移动端

- 🎬 **滚动动画**
    - 各卡片的淡入/滑入效果

- 🧭 **桌面端导航**
    - 右上角导航链接到精选项目、关于我、技能
    - 右侧侧边导航

- 📱 **移动端导航**
    - 移动端左下角简洁的圆形导航按钮

- ⚡ **性能优化**
    - Next.js Image 图片优化
    - 页面加载动画

- 🔝 **返回顶部**
    - 滚动时显示返回顶部按钮

- 🔧 **在线配置管理**
    - 可视化配置界面
    - 无需编辑代码
    - 自动同步到 GitHub

- 🎵 **全局音乐播放器**
    - 支持播放/暂停、上一首/下一首
    - 循环模式切换
    - 可展开/收起
    - 支持音乐列表管理

- 💬 **留言板**
    - 集成 Waline 评论系统
    - 支持访客留言

- 🔗 **友链页面**
    - 展示友情链接
    - 自动获取网站图标和名称

### 技术栈

- [Next.js 16](https://nextjs.org/) - React 框架
- [TypeScript](https://www.typescriptlang.org/) - 类型安全
- [Tailwind CSS](https://tailwindcss.com/) - 原子化 CSS
- [Font Awesome](https://fontawesome.com/) - 图标库

### 项目结构

```
.
├── config.json             # 📝 主配置文件（用户编辑）
├── config.example.json     # 📋 配置示例模板
├── app/
│   ├── admin/              # 管理后台页面
│   ├── api/                # API 路由
│   ├── guestbook/          # 留言板页面
│   ├── friends/            # 友链页面
│   ├── components/         # 组件（按功能分类）
│   │   ├── ui/             # UI 控件（开关、语言切换等）
│   │   ├── layout/         # 布局组件（导航等）
│   │   ├── content/        # 内容组件（项目、技能、关于等）
│   │   ├── media/          # 媒体组件（音乐播放器、头像等）
│   │   └── effects/        # 效果组件（背景、动画等）
│   ├── hooks/              # 自定义 Hooks
│   ├── stores/             # Zustand 状态管理
│   ├── scripts/            # 脚本文件
│   ├── site-config.ts      # 站点配置读取
│   ├── themeConfig.ts      # 主题配置
│   ├── globals.css         # 全局样式
│   ├── layout.tsx          # 根布局
│   ├── metadata.ts         # SEO 元数据
│   └── page.tsx            # 首页
├── types/                  # TypeScript 类型定义
│   ├── config.ts           # 配置相关类型
│   ├── theme.ts            # 主题相关类型
│   ├── store.ts            # Store 相关类型
│   └── api.ts              # API 相关类型
├── public/
│   ├── images/             # 图片资源
│   ├── music/              # 音乐文件
│   ├── markdown/           # Markdown 文件
│   └── robots.txt          # 爬虫规则
├── .env.example            # 环境变量示例
├── Dockerfile              # Docker 配置
├── docker-compose.yml      # Docker Compose 配置
└── package.json
```

### 更新进度

目前仅通过源作者的操作指南进行配置，然后用AI对性能进行了优化。

---

--- 

## 使用指南

### 构建指南

1. **配置config.json文件**

- 参考**根目录**下的**config.json.example和config.json**文件，对**config.json**进行修改。
- 将**i18n/messages/en.json**里面的名字（这里是：yuigneel）替换为你的名字（共三处）以及两行打印机的内容typeWriterText这一行

```html
{
"siteTitle": "yuigneel's Homepage",
"greetingMorning": "Good morning",
"greetingAfternoon": "Good afternoon",
"greetingEvening": "Good evening",
"typeWriterText": "Building a wonderful world with code",
"typeWriterText2": "Passionate about coding, pursuing excellence, never stopping",
"quickLinks": "Quick Links",
"footer": "© 2026 yuigneel's Personal Homepage. All Rights Reserved.",
"nav": {
"blog": "yuigneel's Blog",
"github": "GitHub",
"gitee": "Gitee"
}，
...
 ```

- 同理，**i18n/messages/zh.json**也是这样，只不过是中文（注意打印机两个文件的顺序不要搞反，其实反了也没事儿）。

2.**替换图片**

- 在**public/images**目录下有一下图片，请替换成你自己的图片，具体介绍如表：

|             图片名称             | 图片用途  |   推荐大小    |
|:----------------------------:|:-----:|:---------:|
|         `avatar.jpg`         |  头像   |  512x512  |
|         `index.jpg`          | 暗色背景图 | 1920x1080 |
|         `index4.jpg`         | 亮色背景图 | 1920x1080 |
|          `icon.png`          | 网站图标  |  512x512  |
| `index2.jpg` \~ `index9.jpg` | 项目展示图 | 1200x630  |

3.**其它配置**
其它配置如友链、音乐播放器、留言板、技能、项目描述（封面图片从`index2.jpg` \~ `index9.jpg`里面选，暂不支持**上传**
外）均可以通过稍后的配置网页来修改，无需编辑代码。

4.**运行项目**

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev
```

访问 <http://localhost:9998> 即可预览！

### 部署教程

#### Vercel 部署（推荐）

**适合人群：小白用户，免费托管**

1. **Fork 本项目**

- 点击右上角 `Fork` 按钮

2. **登录 Vercel**

- 访问 [vercel.com](https://vercel.com/)
- 使用 GitHub 登录

3. **配置环境变量（重要！）**
   在 Vercel 部署前，需要先配置以下环境变量：

- 进入 Vercel 控制台
- 选择你的项目 → **Settings** → **Environment Variables**
- 添加以下变量：

|         变量名          |       说明        |         示例         |
|:--------------------:|:---------------:|:------------------:|
|   `GITHUB_APP_ID`    |  GitHub App ID  |      `123456`      |
| `GITHUB_REPO_OWNER`  |      仓库所有者      |   `yourusername`   |
|  `GITHUB_REPO_NAME`  |      仓库名称       |   `AmisHomepage`   |
| `GITHUB_REPO_BRANCH` |      分支名称       |       `main`       |
|   `ENCRYPTION_KEY`   | 加密密钥（用于加密存储的私钥） | `随机生成的32字节十六进制字符串` |

- ⚠️ **注意**：`.env` 文件不会被上传到 GitHub，所以必须在 Vercel 控制台手动配置这些环境变量！

- 💡 **生成加密密钥**：可以使用以下命令生成安全的随机密钥：

    ```bash
        node -e "console.log(require('crypto').randomBytes(32).toString('hex'))"
    ```

4. **导入项目**

- 点击 `New Project`
- 选择你 Fork 的仓库
- 点击 `Deploy`

5. **绑定域名（可选）**
   在项目设置中添加自定义域名

### 在线配置管理（推荐）🔧

项目提供了可视化的配置管理界面，无需手动编辑 JSON 文件！

#### 访问配置页面

1. 部署完成后，访问 `https://your-domain.com/admin`
2. 上传你的 GitHub App PEM 私钥文件
3. 在线编辑所有配置项
4. 点击保存，自动提交到 GitHub

#### 支持的配置项

- ✅ 网站基本信息（名称、标题、URL）
- ✅ 个人资料（头像、姓名、简介）
- ✅ 背景大标题（中英文）
- ✅ TypeWriter 动态文字
- ✅ 打字机效果配置
    - 故障效果开关
    - 颜色渐变开关（仅暗色主题）
    - 故障触发概率（0-100%）
    - 故障触发间隔（500-5000ms）
- ✅ 页脚版权信息
- ✅ 社交链接（GitHub、Gitee、博客、邮箱）及显示/隐藏控制
- ✅ 技能列表（添加、删除、编辑）
- ✅ 项目展示（添加、删除、编辑）
- ✅ 网站组件控制
    - 时间组件（显示/隐藏）
    - 自定义鼠标指针（开启/关闭、上传 .cur 文件）
- ✅ 音乐列表管理（上传、删除、排序）
- ✅ 留言板设置（Waline 集成、启用/禁用）
- ✅ 友链管理（添加、删除、自动获取网站信息）

### GitHub App 配置步骤

1. 访问 GitHub → Settings → Developer settings → GitHub Apps
2. 点击 `New GitHub App`
3. 填写应用名称和描述
4. **权限设置**：

- Contents: **Read and Write**

5. 创建后，在应用详情页：

- 记录 `App ID`
- 生成并下载 `Private Key`（.pem 文件）

6. 将 App 安装到你的仓库
7. 在配置页面上传 PEM 文件即可使用

### 完整配置结构

```
config.json
├── site              # 网站基本信息
│   ├── name          # 网站名称
│   ├── title         # 网站标题
│   ├── url           # 网站地址
│   ├── ogImage       # 分享预览图
│   ├── author        # 作者名
│   ├── description   # 网站描述（中英文）
│   ├── keywords      # SEO 关键词
│   └── footer        # 页脚文字
├── profile           # 个人资料
│   ├── name          # 名字
│   ├── avatar        # 头像路径
│   ├── location      # 所在地
│   ├── focus         # 专业领域
│   ├── hobbies       # 爱好
│   ├── motto         # 座右铭
│   ├── typeWriterTexts # 打字机文字
│   └── currentFocus  # 当前关注事项
├── links             # 社交链接
├── projects          # 项目展示
│   ├── featured      # 精选项目列表
│   └── moreProjectsUrl # 更多项目链接
├── skills            # 技能列表
├── techStack         # 技术栈分类
│   ├── backend       # 后端技术
│   ├── mobile        # 移动端技术
│   └── frontend      # 前端技术
├── guestbook         # 留言板配置
│   ├── enabled       # 是否启用
│   └── walineUrl     # Waline 服务地址
├── friendLinks       # 友链配置
│   ├── enabled       # 是否启用
│   └── links         # 友链列表
├── typeWriterEffects # 打字机效果配置
│   ├── glitchEffect  # 故障效果开关
│   ├── colorGradient # 颜色渐变开关
│   ├── glitchProbability # 故障触发概率 (0-100%)
│   └── glitchInterval    # 故障触发间隔 (毫秒)
└── translations      # 多语言文本
```

### 图标使用说明

本项目使用 [Font Awesome](https://fontawesome.com/icons) 图标库，常用图标：

| 用途      | 图标代码                |
|---------|---------------------|
| 博客      | `fas fa-blog`       |
| GitHub  | `fab fa-github`     |
| 邮箱      | `fas fa-envelope`   |
| 数据库     | `fas fa-database`   |
| 服务器     | `fas fa-server`     |
| 手机      | `fas fa-mobile-alt` |
| 代码      | `fas fa-code`       |
| 音乐      | `fas fa-music`      |
| 首页      | `fas fa-home`       |
| Java    | `fab fa-java`       |
| React   | `fab fa-react`      |
| JS      | `fab fa-js`         |
| Android | `fab fa-android`    |

### 渐变色说明

项目卡片使用 Tailwind CSS 渐变色，常用组合：

| 渐变色代码                          | 效果   |
|--------------------------------|------|
| `from-blue-500 to-purple-600`  | 蓝紫渐变 |
| `from-pink-500 to-rose-600`    | 粉红渐变 |
| `from-emerald-500 to-teal-600` | 绿青渐变 |
| `from-orange-500 to-red-500`   | 橙红渐变 |
| `from-cyan-500 to-blue-600`    | 青蓝渐变 |

---

## 我的宠物

<p align="center"><img src="https://stone.professorlee.work/api/stone/yuigneel/yuigneel-blog" /></p>
<p align="center"><strong>石墩子</strong></p>

---  

## 特别鸣谢

<p align="center">
  <img src="https://img.shields.io/badge/💖-感谢-ff69b4?style=flat-square" alt="Heart" />
  <img src="https://img.shields.io/badge/🌟-支持-ffd700?style=flat-square" alt="Star" />
  <img src="https://img.shields.io/badge/🙏-感恩-4169e1?style=flat-square" alt="Pray" />
</p>  

|                                           贡献者头像                                           |                       贡献者昵称                       |         贡献内容         |
|:-----------------------------------------------------------------------------------------:|:-------------------------------------------------:|:--------------------:|
| <img src="https://avatars.githubusercontent.com/u/89632742?v=4" width="32" height="32" /> | [professor-lee](https://github.com/professor-lee) |   阅读文档里面的赛博宠物石墩子一枚   |
| <img src="https://avatars.githubusercontent.com/u/58239518?v=4" width="32" height="32" /> |      [AmisKwok](https://github.com/AmisKwok)      | 整个项目就是从该作者的项目基础上修改而来 |

<p align="center"><strong>特别鸣谢所有为本项目做出贡献和支持的开发者们！</strong></p>

---  

## LICENSE

### 许可证主旨

原则上，只要不违反以下原则，均可以使用：

- **保留署名** - 使用和修改代码时必须声明原作者
- **开源要求** - 无论本地部署还是作为API服务，都必须保持开源
- **商业用途** - 禁止用于商业用途
- **协议要求** - 修改后必须使用相同协议

### 许可证声明

- 本项目采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh)
  开源许可证。详细条款请参阅 [CC BY-NC-SA 4.0 官方文档](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode.zh-hans)。


- 本项目源码是由 [**AmisKwok**](https://github.com/AmisKwok)开源的代码基础上修改的，故项目遵循原作者要求选择的许可证发布，确保代码的开放性与可追溯性。


