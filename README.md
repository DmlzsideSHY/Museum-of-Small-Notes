# 小纸条博物馆 / Note Museum

[中文](#) | [English](#)

---

## 中文内容

一个轻量级的个人记忆管理工具，用于收藏和管理高中生活中的碎片记忆——那些写满心事的纸条、随手涂鸦的便签，以及属于那个年代的“著作”。

在线体验：https://github.com/DmlzsideSHY/Museum of Small Notes.git

---

项目背景

高中三年，每个人都有太多值得留下的东西。

课堂上偷偷传过的纸条，走廊里塞给同桌的便签，深夜写在草稿纸上的心事，还有那些认真或随意写下的日记、诗、小说、计划——它们散落在书包里、抽屉中、旧课本的夹缝里，时间久了就再也找不到了。

小纸条博物馆就是为了把这些碎片收集起来而做的。

你可以把每一条“小纸条”上传保存——哪怕只是一张拍糊了的照片、一行歪歪扭扭的字。它能帮你把那些零散的东西归拢到一起，按时期和分类整理好，再也不会弄丢。

页面里的“高一”“高二”“高三”是默认的时期分类，方便你把记忆按时间线串起来。如果你不是高中生，或者有更合适的分类方式，也可以自由增删改。

这里没有算法推荐，没有社交压力，只是一个安静的、只属于你自己的回忆收藏夹。

---

功能特性

书架

- 添加/编辑/删除书籍
- 为书籍添加多页面（支持文字与配图）
- 内置阅读器，翻页浏览
- 下载书籍为 Markdown 文件

小纸条

- 上传图片（支持拖拽），添加备注
- 双层级分类：时期与分类（自由增删改）
- 两种展示模式：照片墙与铺排列表
- 筛选浏览：按时期和分类快速筛选
- 批量操作：勾选纸条，批量移动分类或生成分享图
- 导出与导入数据（JSON 格式备份）

---

快速开始

在线使用
直接访问部署好的 GitHub Pages 链接即可使用，无需安装任何东西。

本地运行
1. 下载 index.html 文件
2. 用浏览器打开即可使用
3. 所有数据存储在浏览器本地（IndexedDB），刷新页面不会丢失

---

技术栈

- 原生 HTML + CSS + JavaScript，纯前端，无框架依赖
- IndexedDB，数据持久化存储
- html2canvas，生成分享图

---

数据存储

所有数据存储在浏览器的 IndexedDB 数据库中，数据库名为 MemoryWorkshopDB，包含以下数据表：

- books：书籍数据（含页面）
- notes：小纸条数据
- settings：元数据（时期与分类列表、初始化标记）

数据完全在本地，不会上传到任何服务器。

---

数据导入与导出

- 导出：点击导出纸条按钮，下载 JSON 备份文件
- 导入：点击导入纸条按钮，上传 JSON 备份文件恢复数据
- 书籍导入：书架工具栏中有导入书籍按钮，支持导入书籍 JSON 数据

---

界面风格

- 暖色复古风格（土壤色系）
- 纯文字界面，无装饰性图标
- 响应式设计，适配手机和电脑

---

使用说明

书架模块

- 点击“添加书籍”创建新书
- 点击书籍封面进入阅读器
- 在书籍编辑界面可添加/编辑/删除页面
- 点击“下载”可将书籍导出为 Markdown 文件

小纸条模块

- 点击“添加纸条”上传图片并填写备注
- 使用“管理分类”创建时期和分类
- 点击纸条右上角圆点进行勾选
- 勾选后可批量“移动分类”或“生成分享图”
- 照片墙模式随机排列，铺排模式列表展示

数据备份

- 点击“导出纸条”下载 JSON 备份文件
- 点击“导入纸条”上传备份文件恢复数据
- 书架也有独立的“导入书籍”功能

---

更新日志

v1.0.0
- 初始版本发布
- 书架与小纸条双模块
- 照片墙与铺排双模式
- 批量分享图生成
- 数据导入与导出

---

致谢

本项目由未活猫使用 DeepSeek 生成。

特别感谢：

- html2canvas 截图工具
- 所有使用小纸条博物馆的朋友们

---

Made with ❤️
## English Content

A lightweight personal memory management tool for collecting and preserving fragmentary memories from high school life—those notes filled with thoughts, doodled sticky notes, and the "writings" that belong to that era.

Live Demo: https://github.com/DmlzsideSHY/Museum of Small Notes.git

---

Project Background

Everyone has too many things worth keeping from their three years of high school.

Notes secretly passed during class, sticky notes slipped to deskmates in the hallway, thoughts scribbled on scratch paper late at night, and diaries, poems, novels, plans written carefully or casually—they scatter in backpacks, drawers, between the pages of old textbooks, and over time, they disappear forever.

The Note Museum was created to collect these fragments.

You can save every "note"—even just a blurry photo, a line of crooked handwriting. It helps you gather those scattered pieces, organize them by period and category, and never lose them again.

The default period categories—"Grade 10," "Grade 11," "Grade 12"—help you string your memories along a timeline. If you're not a high school student, or if you have a better way to categorize, you are free to add, edit, or delete them.

There are no algorithms, no social pressure—just a quiet, personal memory collection that belongs only to you.

---

Features

Bookshelf

- Add / Edit / Delete books
- Add multiple pages to each book (supports text and images)
- Built-in reader for flip-through browsing
- Export books as Markdown files

Notes

- Upload images (drag-and-drop supported) and add remarks
- Two-level classification: Period + Category (freely add, edit, delete)
- Two display modes: Photo Wall and List
- Filter browsing: filter by period and category
- Batch operations: select notes, batch move categories, or generate shareable images
- Export and import data (JSON backup)

---

Quick Start

Online Usage
Directly visit the deployed GitHub Pages link—no installation required.

Local Usage
1. Download index.html
2. Open it in a browser
3. All data is stored locally in IndexedDB—data persists even after refreshing the page

---

Tech Stack

- Vanilla HTML + CSS + JavaScript, pure frontend, no framework dependencies
- IndexedDB for persistent data storage
- html2canvas for generating shareable images

---

Data Storage

All data is stored in the browser's IndexedDB database, named MemoryWorkshopDB, with the following tables:

- books: book data (including pages)
- notes: note data
- settings: metadata (period/category lists, initialization flag)

Data stays entirely on your device and is never uploaded to any server.

---

Data Import and Export

- Export: Click the "Export Notes" button to download a JSON backup file
- Import: Click the "Import Notes" button to upload a JSON backup file to restore data
- Book Import: Use the "Import Books" button in the Bookshelf toolbar to import book JSON data

---

UI Style

- Warm, vintage color palette (earth tones)
- Clean text-only interface, no decorative icons
- Responsive design, suitable for both desktop and mobile

---

User Guide

Bookshelf Module

- Click "Add Book" to create a new book
- Click a book cover to open the reader
- In the book editing interface, you can add / edit / delete pages
- Click "Download" to export the book as a Markdown file

Notes Module

- Click "Add Note" to upload an image and fill in a remark
- Use "Manage Categories" to create periods and categories
- Click the circle in the top-right corner of a note to select it
- After selecting, batch operations: "Move Category" or "Generate Shareable Image"
- Photo Wall mode arranges notes randomly; List mode displays them in a list

Data Backup

- Click "Export Notes" to download a JSON backup file
- Click "Import Notes" to upload a backup file and restore data
- Bookshelf also has an independent "Import Books" feature

---

Changelog

v1.0.0
- Initial release
- Bookshelf + Notes dual modules
- Photo Wall + List dual display modes
- Batch shareable image generation
- Data import and export

---

Acknowledgments

This project was generated by Weihuomao using DeepSeek.

Special thanks to:

- html2canvas screenshot tool
- Everyone who uses the Note Museum

---

Made with ❤️
