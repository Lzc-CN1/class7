# 深技大附中 · 2024级七班官网

> 青春正好，七班同行。

## 项目简介

这是深圳技术大学附属中学 2024 级七班的班级官方网站，记录我们高中三年的成长足迹。

网站由班级同学自主设计开发，托管于 GitHub Pages，通过自定义域名对外访问。

---

## 页面结构

| 板块 | 内容 |
|------|------|
| **Hero** | 班级集体照全屏背景，视差滚动效果 |
| **班级介绍** | 班级基本信息与数据展示 |
| **班主任寄语** | 杨文杰老师寄语 |
| **成员风采** | 全班 48 位同学姓名与职务 |
| **班级动态** | 高考倒计时与班级大事记 |
| **班级相册** | 横向轮播相册，支持大图预览 |
| **联系我们** | 班级联系方式与留言表单 |

---

## 技术栈

- 纯静态 HTML / CSS / JavaScript，无任何框架依赖
- 所有代码集中在单个 `index.html` 文件中
- 字体：[Noto Sans SC](https://fonts.google.com/noto/specimen/Noto+Sans+SC) + [ZCOOL QingKe HuangYou](https://fonts.google.com/specimen/ZCOOL+QingKe+HuangYou)（标题艺术字）
- 部署：GitHub Pages + 自定义域名

---

## 文件结构

```
├── index.html          # 主页面（含全部 HTML / CSS / JS）
├── README.md           # 项目说明
├── CNAME               # 自定义域名配置（部署时添加）
└── assets/
    └── images/
        ├── class-group-photo.jpg   # Hero 背景集体照
        ├── about-class.jpg         # 班级介绍配图
        └── mmexport177756287*.jpg  # 相册照片（共 8 张）
```

---

## 本地预览

不需要任何构建工具，直接用任意 HTTP 服务器启动即可。

**方式一：Python（推荐）**
```bash
python -m http.server 8080
# 浏览器访问 http://localhost:8080
```

**方式二：VS Code Live Server 插件**

安装 Live Server 插件后，右键 `index.html` → Open with Live Server

---

## 部署到 GitHub Pages

1. 新建 GitHub 仓库（设为 Public）
2. 推送代码：
   ```bash
   git init
   git add .
   git commit -m "初始版本"
   git remote add origin https://github.com/你的用户名/仓库名.git
   git push -u origin main
   ```
3. 进入仓库 Settings → Pages → Source 选择 `main` 分支 `/root`
4. 等待约 1 分钟后即可通过 `https://你的用户名.github.io/仓库名/` 访问

### 绑定自定义域名

1. 在项目根目录创建 `CNAME` 文件，写入你的域名：
   ```
   你的域名.com
   ```
2. 在域名 DNS 控制台添加 CNAME 记录：
   ```
   主机记录：@（或 www）
   记录值：你的用户名.github.io
   ```
3. 在 GitHub Pages 设置里填入域名，勾选 **Enforce HTTPS**

---

## 班级信息

- **学校**：深圳技术大学附属中学
- **年级**：2024 级
- **班级**：七班
- **班主任**：杨文杰老师
- **人数**：48 人
- **目标**：2027 年高考

---

## 更新记录

| 日期 | 更新内容 |
|------|----------|
| 2026-05 | 完成网站初版开发与上线 |

---

*© 2024-2026 深圳技术大学附属中学 2024 级七班*
