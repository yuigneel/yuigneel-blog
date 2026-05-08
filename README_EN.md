<div align="center">
  <img src="https://avatars.githubusercontent.com/u/202588416?s=400&u=baab8feb9dfc2e334858b649c91045a1be6f39f5&v=4" width="200" height="200" />


<h1><a href="https://yuigneel-blog.vercel.app/" target="_blank" rel="noopener noreferrer">yuigneel-blog</a></h1>

  <p>
    <a href="README.md">简体中文</a> | 
    <a href="README_EN.md">English</a>
  </p>
</div>

---

## Project Introduction

### Overview

- This project is an open-source blog project based on Next.js+React+TypeScript+TailwindCSS, adapted from the open-source code by [AmisKwok](https://github.com/AmisKwok).
- Currently, this project is intended **for personal learning purposes only**. The code is **for learning purposes only**. If there are any issues, **neither the original author nor I endorse them**. If you want to create your own blog, you **can fork this repository**, but it is **recommended** to visit the [**original author's repository**](https://github.com/AmisKwok/AmisHomepage).

### Features

- 🎨 **Modern Design**
    - Full-screen background image + gradient overlay
    - Dynamic backgrounds (dark mode: starry sky, light mode: falling leaves)

- ✍️ **SVG Drawing Title**
    - Handwritten style title
    - Dynamically calculated viewBox

- ⌨️ **Typewriter Effect**
    - Dynamic typewriter text effect
    - Supports multiple text loops

- 🎭 **Glitch Effect**
    - Configurable glitch shake animation
    - Supports custom trigger probability and interval

- 🌈 **Color Gradient**
    - Dynamic colorful gradient effect (dark theme only)

- 👤 **Avatar Animation**
    - Breathing halo effect
    - Hover zoom + multi-layer glow

- 🔗 **Social Links**
    - Displayed at the center of the background image
    - Ripple click effect
    - Hover glow

- 📋 **About Me Card**
    - Loads personal information from GitHub README
    - Skill tag hover effects

- 🌟 **Featured Projects**
    - Displays project cards
    - Supports border flowing light, shadow diffusion, and image mask animations

- 📊 **Skill Visualization**
    - Progress bars to showcase tech stack
    - Number animation effects

- 🌍 **Multi-language Support**
    - Supports Chinese/English switching
    - Automatically detects system language

- 🌓 **Theme Switching**
    - Supports light/dark mode switching
    - Default dark theme
    - Blur transition animation
    - Theme adapts to all components

- 🕐 **Time Component**
    - Displays local time and date in the top-left corner
    - Click to expand calendar
    - Smooth width transition animation

- 🖱️ **Custom Cursor**
    - Supports custom cursor styles
    - Can upload .cur files

- 📱 **Responsive Layout**
    - Perfectly adapts to desktop and mobile devices

- 🎬 **Scroll Animations**
    - Fade-in/slide-in effects for various cards

- 🧭 **Desktop Navigation**
    - Top-right navigation links to featured projects, about me, and skills
    - Right-side sidebar navigation

- 📱 **Mobile Navigation**
    - Simple circular navigation button in the bottom-left corner on mobile

- ⚡ **Performance Optimization**
    - Next.js Image optimization
    - Page loading animation

- 🔝 **Back to Top**
    - Shows back-to-top button when scrolling

- 🔧 **Online Configuration Management**
    - Visual configuration interface
    - No need to edit code
    - Automatic synchronization to GitHub

- 🎵 **Global Music Player**
    - Supports play/pause, previous/next track
    - Loop mode switching
    - Expandable/collapsible
    - Supports music list management

- 💬 **Guestbook**
    - Integrated Waline comment system
    - Supports visitor comments

- 🔗 **Friend Links Page**
    - Displays friend links
    - Automatically fetches website icons and names

### Tech Stack

- [Next.js 16](https://nextjs.org/) - React framework
- [TypeScript](https://www.typescriptlang.org/) - Type safety
- [Tailwind CSS](https://tailwindcss.com/) - Atomic CSS
- [Font Awesome](https://fontawesome.com/) - Icon library

### Project Structure

```
.
├── config.json             # 📝 Main configuration file (user editable)
├── config.example.json     # 📋 Configuration example template
├── app/
│   ├── admin/              # Admin backend page
│   ├── api/                # API routes
│   ├── guestbook/          # Guestbook page
│   ├── friends/            # Friend links page
│   ├── components/         # Components (organized by function)
│   │   ├── ui/             # UI controls (toggles, language switcher, etc.)
│   │   ├── layout/         # Layout components (navigation, etc.)
│   │   ├── content/        # Content components (projects, skills, about, etc.)
│   │   ├── media/          # Media components (music player, avatar, etc.)
│   │   └── effects/        # Effect components (backgrounds, animations, etc.)
│   ├── hooks/              # Custom Hooks
│   ├── stores/             # Zustand state management
│   ├── scripts/            # Script files
│   ├── site-config.ts      # Site configuration reader
│   ├── themeConfig.ts      # Theme configuration
│   ├── globals.css         # Global styles
│   ├── layout.tsx          # Root layout
│   ├── metadata.ts         # SEO metadata
│   └── page.tsx            # Homepage
├── types/                  # TypeScript type definitions
│   ├── config.ts           # Configuration-related types
│   ├── theme.ts            # Theme-related types
│   ├── store.ts            # Store-related types
│   └── api.ts              # API-related types
├── public/
│   ├── images/             # Image resources
│   ├── music/              # Music files
│   ├── markdown/           # Markdown files
│   └── robots.txt          # Crawler rules
├── .env.example            # Environment variable example
├── Dockerfile              # Docker configuration
├── docker-compose.yml      # Docker Compose configuration
└── package.json
```

### Update Progress

Currently configured only through the original author's operation guide, with AI-based performance optimizations applied.

---

--- 

## Usage Guide

### Build Guide

1. **Configure the config.json file**

- Refer to the **config.json.example** and **config.json** files in the **root directory** to modify **config.json**.
- Replace the name (here: yuigneel) in **i18n/messages/en.json** with your name (three places in total) and the two lines of typewriter content in the typeWriterText line:

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
},
...
 ```

- Similarly, do the same for **i18n/messages/zh.json**, but in Chinese (note that the order of the two typewriter files should not be reversed, although it doesn't really matter if it is).

2. **Replace Images**

- In the **public/images** directory, there are the following images. Please replace them with your own images. Details are shown in the table below:

|             Image Name             | Image Purpose  |   Recommended Size    |
|:----------------------------:|:-----:|:---------:|
|         `avatar.jpg`         |  Avatar   |  512x512  |
|         `index.jpg`          | Dark mode background | 1920x1080 |
|         `index4.jpg`         | Light mode background | 1920x1080 |
|          `icon.png`          | Website icon  |  512x512  |
| `index2.jpg`、`index3.jpg`、`index5.jpg` \~ `index9.jpg` | Project display images | 1200x630  |

3. **Other Configurations**
Other configurations such as friend links, music player, guestbook, skills, project descriptions (cover images selected from `index2.jpg` \~ `index9.jpg`, currently does not support **uploading**) can all be modified through the configuration webpage later, without editing code.

4. **Run the Project**

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

Visit <http://localhost:9998> to preview!

### Deployment Tutorial

#### Vercel Deployment (Recommended)

**Suitable for: Beginners, free hosting**

1. **Fork This Project**

- Click the `Fork` button in the top-right corner

2. **Log in to Vercel**

- Visit [vercel.com](https://vercel.com/)
- Log in using GitHub

3. **Configure Environment Variables (Important!)**
   Before deploying to Vercel, you need to configure the following environment variables:

- Enter the Vercel console
- Select your project → **Settings** → **Environment Variables**
- Add the following variables:

|         Variable Name          |       Description        |         Example         |
|:--------------------:|:---------------:|:------------------:|
|   `GITHUB_APP_ID`    |  GitHub App ID  |      `123456`      |
| `GITHUB_REPO_OWNER`  |      Repository Owner      |   `yourusername`   |
|  `GITHUB_REPO_NAME`  |      Repository Name       |   `AmisHomepage`   |
| `GITHUB_REPO_BRANCH` |      Branch Name       |       `main`       |
|   `ENCRYPTION_KEY`   | Encryption key (used to encrypt stored private keys) | `Randomly generated 32-byte hexadecimal string` |

- ⚠️ **Note**: The `.env` file will not be uploaded to GitHub, so you must manually configure these environment variables in the Vercel console!

- 💡 **Generate encryption key**: You can use the following command to generate a secure random key:

    ```bash
        node -e "console.log(require('crypto').randomBytes(32).toString('hex'))"
    ```

4. **Import Project**

- Click `New Project`
- Select your forked repository
- Click `Deploy`

5. **Bind Domain (Optional)**
   Add a custom domain in the project settings

### Online Configuration Management (Recommended) 🔧

The project provides a visual configuration management interface, eliminating the need to manually edit JSON files!

#### Access Configuration Page

1. After deployment, visit `https://your-domain.com/admin`
2. Upload your GitHub App PEM private key file
3. Edit all configuration items online
4. Click save to automatically submit to GitHub

#### Supported Configuration Items

- ✅ Basic website information (name, title, URL)
- ✅ Personal profile (avatar, name, bio)
- ✅ Background main title (Chinese and English)
- ✅ TypeWriter dynamic text
- ✅ Typewriter effect configuration
    - Glitch effect toggle
    - Color gradient toggle (dark theme only)
    - Glitch trigger probability (0-100%)
    - Glitch trigger interval (500-5000ms)
- ✅ Footer copyright information
- ✅ Social links (GitHub, Gitee, blog, email) and show/hide control
- ✅ Skill list (add, delete, edit)
- ✅ Project display (add, delete, edit)
- ✅ Website component control
    - Time component (show/hide)
    - Custom cursor (enable/disable, upload .cur file)
- ✅ Music list management (upload, delete, sort)
- ✅ Guestbook settings (Waline integration, enable/disable)
- ✅ Friend link management (add, delete, auto-fetch website information)

### GitHub App Configuration Steps

1. Visit GitHub → Settings → Developer settings → GitHub Apps
2. Click `New GitHub App`
3. Fill in the application name and description
4. **Permission Settings**:

- Contents: **Read and Write**

5. After creation, on the application details page:

- Record the `App ID`
- Generate and download the `Private Key` (.pem file)

6. Install the App to your repository
7. Upload the PEM file on the configuration page to use

### Complete Configuration Structure

```
config.json
├── site              # Basic website information
│   ├── name          # Website name
│   ├── title         # Website title
│   ├── url           # Website URL
│   ├── ogImage       # Share preview image
│   ├── author        # Author name
│   ├── description   # Website description (Chinese and English)
│   ├── keywords      # SEO keywords
│   └── footer        # Footer text
├── profile           # Personal profile
│   ├── name          # Name
│   ├── avatar        # Avatar path
│   ├── location      # Location
│   ├── focus         # Professional field
│   ├── hobbies       # Hobbies
│   ├── motto         # Motto
│   ├── typeWriterTexts # Typewriter text
│   └── currentFocus  # Current focus
├── links             # Social links
├── projects          # Project display
│   ├── featured      # Featured project list
│   └── moreProjectsUrl # More projects link
├── skills            # Skill list
├── techStack         # Tech stack categories
│   ├── backend       # Backend technologies
│   ├── mobile        # Mobile technologies
│   └── frontend      # Frontend technologies
├── guestbook         # Guestbook configuration
│   ├── enabled       # Whether enabled
│   └── walineUrl     # Waline service URL
├── friendLinks       # Friend link configuration
│   ├── enabled       # Whether enabled
│   └── links         # Friend link list
├── typeWriterEffects # Typewriter effect configuration
│   ├── glitchEffect  # Glitch effect toggle
│   ├── colorGradient # Color gradient toggle
│   ├── glitchProbability # Glitch trigger probability (0-100%)
│   └── glitchInterval    # Glitch trigger interval (milliseconds)
└── translations      # Multi-language text
```

### Icon Usage Instructions

This project uses the [Font Awesome](https://fontawesome.com/icons) icon library. Common icons:

| Purpose      | Icon Code                |
|---------|---------------------|
| Blog      | `fas fa-blog`       |
| GitHub  | `fab fa-github`     |
| Email      | `fas fa-envelope`   |
| Database     | `fas fa-database`   |
| Server     | `fas fa-server`     |
| Mobile      | `fas fa-mobile-alt` |
| Code      | `fas fa-code`       |
| Music      | `fas fa-music`      |
| Home      | `fas fa-home`       |
| Java    | `fab fa-java`       |
| React   | `fab fa-react`      |
| JS      | `fab fa-js`         |
| Android | `fab fa-android`    |

### Gradient Color Instructions

Project cards use Tailwind CSS gradients. Common combinations:

| Gradient Code                          | Effect   |
|--------------------------------|------|
| `from-blue-500 to-purple-600`  | Blue-purple gradient |
| `from-pink-500 to-rose-600`    | Pink-red gradient |
| `from-emerald-500 to-teal-600` | Green-cyan gradient |
| `from-orange-500 to-red-500`   | Orange-red gradient |
| `from-cyan-500 to-blue-600`    | Cyan-blue gradient |

---

## My Pet

<p align="center"><img src="https://stone.professorlee.work/api/stone/yuigneel/yuigneel-blog" /></p>
<p align="center"><strong>Stone Pedestal</strong></p>

---  

## Special Thanks

<p align="center">
  <img src="https://img.shields.io/badge/💖-Thanks-ff69b4?style=flat-square" alt="Heart" />
  <img src="https://img.shields.io/badge/🌟-Support-ffd700?style=flat-square" alt="Star" />
  <img src="https://img.shields.io/badge/🙏-Gratitude-4169e1?style=flat-square" alt="Pray" />
</p>  

|                                           Contributor Avatar                                           |                       Contributor Name                       |         Contribution Content         |
|:-----------------------------------------------------------------------------------------:|:-------------------------------------------------:|:--------------------:|
| <img src="https://avatars.githubusercontent.com/u/89632742?v=4" width="32" height="32" /> | [professor-lee](https://github.com/professor-lee) |   Cyber pet stone pedestal mentioned in the documentation   |
| <img src="https://avatars.githubusercontent.com/u/58239518?v=4" width="32" height="32" /> |      [AmisKwok](https://github.com/AmisKwok)      | The entire project was modified based on this author's project |

<p align="center"><strong>Special thanks to all developers who have contributed to and supported this project!</strong></p>

---  

## LICENSE

### License Principles

In principle, you may use this project as long as you do not violate the following principles:

- **Attribution Required** - You must credit the original author when using or modifying the code
- **Open Source Requirement** - Must remain open source whether deployed locally or as an API service
- **Commercial Use** - Prohibited for commercial purposes
- **License Requirement** - Modifications must use the same license

### License Statement

- This project is licensed under the [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.en)
  open source license. For detailed terms, please refer to the [CC BY-NC-SA 4.0 Official Documentation](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).


- The source code of this project was modified based on the open-source code by [**AmisKwok**](https://github.com/AmisKwok). Therefore, the project follows the license chosen by the original author to ensure the openness and traceability of the code.

