# Changelog

All notable changes to this project will be documented in this file.

---

## [1.2.0] - 2026-03-20

### ✨ Features

- **图片分类支持 (Image Categorization)**
  - 新增基于子文件夹的自动分类系统。将图片放入 `public/images/<分类名>/` 即可自动识别分类，无需任何额外配置。
  - `/api/random` 接口新增 `category` 查询参数，支持按分类获取随机图片。
    - 示例：`/api/random?category=nature`（可与 `type` 参数组合使用）
  - 图库页面 (`/gallery`) 顶部新增分类筛选导航栏，支持一键切换分类。
  - 图片详情弹窗中新增"分类"信息展示字段。

### 🔧 Improvements

- 构建脚本 (`scripts/generate-images-metadata.js`) 现已在元数据中为每张图片附加 `category` 字段。
- 图库图片数量统计改为实时显示当前筛选下的图片数量。

---

## [1.1.0] - Initial Release

- 基于 EdgeOne Pages 构建的随机图片分发系统。
- 支持 PC / 移动端自动识别与分发。
- 瀑布流图库与 GSAP 动画。
- 构建时自动生成缩略图与元数据。
