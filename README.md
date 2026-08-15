# Lingsong Xiong / 熊凌崧 — Academic Website

基于 [Academic Pages](https://github.com/academicpages/academicpages.github.io) 模板的中英双语学术主页。
Based on the [Academic Pages](https://github.com/academicpages/academicpages.github.io) template, with a custom English/Chinese bilingual setup.

**当前状态：英文版已按 CV 填充完成（主页、简历、论文、报告、教学）；中文版内容已全部就绪，但暂不上线——`_config.yml` 中 `zh_enabled: false`，/zh/ 页面不构建、导航不显示"中文"按钮。重新上线方法见该配置项的注释。**

---

## 一、双语机制（先读这一节）

全站约定：**英文页面在根路径 `/`，中文页面在 `/zh/`**，一一对应：

| 页面 | 英文 | 中文 |
|---|---|---|
| 主页 | `/` | `/zh/` |
| 发表论文 | `/publications/` | `/zh/publications/` |
| 学术报告 | `/talks/` | `/zh/talks/` |
| 教学 | `/teaching/` | `/zh/teaching/` |
| 博客 | `/year-archive/` | `/zh/year-archive/` |
| 简历 | `/cv/` | `/zh/cv/` |

- 每个页面 front matter 里有 `lang: en` 或 `lang: zh`（英文页面由 `_config.yml` 默认提供，中文页面需显式写 `lang: zh`）。
- 顶部导航栏右侧的 **中文 / EN** 按钮按“加减 `/zh` 前缀”自动计算对应页面地址，实现语言切换。某页与镜像页地址不对应时，可在该页 front matter 用 `lang-alt: /path/` 手动指定。
- 顶部导航菜单按页面语言加载：英文 `_data/navigation.yml`，中文 `_data/navigation-zh.yml`。
- 列表页（论文/报告/教学/博客）按 `lang` 过滤：**英文列表只显示非 `zh` 条目，中文列表只显示 `lang: zh` 条目**，因此同一篇论文不会在两个语言下重复出现。

### 如何让一条内容“双语化”

以一篇论文为例：

1. 英文条目：`_publications/2026-01-01-my-paper.md`（`permalink: /publication/my-paper`，无 `lang` 字段 → 默认英文）。
2. 中文条目：复制该文件，`permalink` 改为 `/zh/publication/my-paper`，front matter 加一行 `lang: zh`，标题/摘要/正文译成中文。
3. 完成——两个语言的列表页和详情页各自显示对应版本，切换按钮直接互通。

报告（`_talks`）、教学（`_teaching`）、博文（`_posts`）同理。中文页面文件统一放在 `_pages/zh/` 目录。

## 二、日常编辑指南

| 要改什么 | 改哪个文件 |
|---|---|
| 姓名、邮箱、头像、社交链接、网站标题 | `_config.yml` |
| 英文主页 | `_pages/about.md` |
| 中文主页 | `_pages/zh/about.md` |
| 英文/中文简历 | `_pages/cv.md` / `_pages/zh/cv.md` |
| 论文列表 | `_publications/` 下每篇一个文件 |
| 报告列表 | `_talks/` 下每场一个文件 |
| 课程列表 | `_teaching/` 下每门一个文件 |
| 博文 | `_posts/` 下每篇一个文件（文件名 `YYYY-MM-DD-标题.md`） |
| 导航菜单 | `_data/navigation.yml` / `_data/navigation-zh.yml` |
| 头像图片 | `images/profile.png` |
| PDF 等附件 | 放入 `files/`，链接写 `/files/xxx.pdf` |

## 三、本地预览

本机（macOS 系统 Ruby 2.6）已装好全部依赖，直接运行：

```bash
PATH="$HOME/.gem/ruby/2.6.0/bin:$PATH" JEKYLL_NO_BUNDLER_REQUIRE=1 jekyll serve
# 打开 http://localhost:4000，改文件会自动刷新
```

说明：

- 本机系统 Ruby 太老，`bundle install` 会因新版 gem 的平台兼容问题失败，所以本机用
  `gem install --user-install` 直装（已完成），并加 `JEKYLL_NO_BUNDLER_REQUIRE=1`
  绕过 Gemfile；这只影响本机预览，**线上 GitHub Actions 构建走仓库根目录的 `Gemfile`，不受影响**。
- 在装有 Ruby 3.x 的机器上可以直接 `bundle install && bundle exec jekyll serve`。
- 也可以参考模板自带的 `.devcontainer` 或 Docker 配置。

## 四、发布上线

1. 在 GitHub 新建仓库，名字用 `你的用户名.github.io`（CV 中 GitHub 用户名为 xionglingsong，对应 `xionglingsong.github.io`），即可得到 `https://用户名.github.io` 的免费网址。
2. 把本目录推上去（本目录已是初始化好的空 git 仓库）：

   ```bash
   git add .
   git commit -m "Initial academic website"
   git remote add origin git@github.com:你的用户名/你的用户名.github.io.git
   git push -u origin main
   ```

3. 仓库 Settings → Pages 确认由 GitHub Actions / gh-pages 分支构建（模板自带工作流）。
4. 如果 GitHub 用户名不是 xionglingsong，记得把 `_config.yml` 里的 `url` 和 `repository` 改成实际地址。

## 五、致谢

- 模板：[Academic Pages](https://github.com/academicpages/academicpages.github.io)（fork 自 [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)）
- 双语方案为本仓库自行添加：语言切换按钮（`_includes/lang-switch.html`）、双语导航（`_includes/masthead.html`）、语言过滤列表页。
