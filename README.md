# CUC 媒体事实核查平台 - 微信小程序项目

一个基于微信小程序开发的媒体事实核查平台，支持音频、视频、图像等多种媒体类型的AI鉴伪检测。

<!-- PROJECT SHIELDS -->
<p align="left">
  <img src="https://img.shields.io/badge/微信小程序-原生开发-green.svg?style=flat-square" alt="微信小程序">
  <img src="https://img.shields.io/badge/JavaScript-ES6+-yellow.svg?style=flat-square" alt="JavaScript">
  <img src="https://img.shields.io/badge/WXML-模板语言-blue.svg?style=flat-square" alt="WXML">
  <img src="https://img.shields.io/badge/WXSS-样式语言-pink.svg?style=flat-square" alt="WXSS">
  <img src="https://img.shields.io/badge/AI鉴伪-深度学习-orange.svg?style=flat-square" alt="AI鉴伪">
  <a href="LICENSE.txt">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square" alt="License: MIT">
  </a>
</p>

## 📋 目录

- [项目概述](#项目概述)
- [版本历史与差异](#版本历史与差异)
- [功能特性](#功能特性)
- [技术架构](#技术架构)
- [安装与部署](#安装与部署)
- [使用说明](#使用说明)
- [项目结构](#项目结构)
- [开发指南](#开发指南)
- [版本控制](#版本控制)
- [贡献指南](#贡献指南)
- [许可证](#许可证)

## 🎯 项目概述

CUC媒体事实核查平台是一个基于微信小程序的AI鉴伪系统，旨在通过多种深度学习算法对音频、视频、图像等媒体内容进行真实性检测。该项目由中国传媒大学开发，集成了多种先进的AI鉴伪算法，为用户提供便捷的媒体内容核查服务。

### 核心功能
- **多模态鉴伪检测**：支持音频、视频、图像等多种媒体类型
- **多算法融合**：集成MVSS、MABC、OSN、W2V、传统算法等多种检测模型
- **实时分析**：提供快速的文件上传和检测结果展示
- **用户友好**：简洁直观的界面设计，支持移动端操作

## 📚 版本历史与差异

### 🚀 最新版本 (v2023.12.31)
**目录**: `鉴伪微信小程序1231/`

**主要特性**:
- ✅ 完整的子包架构设计
- ✅ 支持5种AI算法展示页面
- ✅ 综合鉴伪功能
- ✅ 详细的结果展示页面
- ✅ 优化的用户界面
- ✅ 支持下拉刷新

**页面结构**:
```
主包页面:
├── index/     # 首页 - 综合鉴伪入口
├── my/        # 个人中心
├── music/     # 综合鉴伪页面
├── show/      # 算法展示入口
├── result/    # 检测结果展示

子包页面:
├── package-music/
│   └── music/ # 音频鉴伪
├── package-show/
│   ├── MABC/  # MABC算法展示
│   ├── MVSS/  # MVSS算法展示
│   ├── OSN/   # OSN算法展示
│   ├── W2V/   # W2V算法展示
│   └── Tradition/ # 传统算法展示
└── package-result/
    └── result/ # 结果页面
```

### 🔄 历史版本对比

| 版本 | 目录 | 发布时间 | 主要特性 | 差异说明 |
|------|------|----------|----------|----------|
| **v2023.12.31** | `鉴伪微信小程序1231/` | 2023-12-31 | 完整功能版 | 最新稳定版本，功能最全 |
| **v2023.12.21** | `鉴伪微信小程序1221/` | 2023-12-21 | 功能完善版 | 与1231版本基本相同 |
| **v2023.12.17** | `鉴伪微信小程序1217/` | 2023-12-17 | 功能测试版 | 测试阶段版本 |
| **v2023.12.06** | `鉴伪微信小程序1206/` | 2023-12-06 | 界面优化版 | 优化了用户界面设计 |
| **v2023.12.03** | `鉴伪微信小程序1203/` | 2023-12-03 | 子包架构版 | 首次引入子包架构 |
| **v2023.12.03** | `鉴伪微信小程序1203（页面按钮）/` | 2023-12-03 | 按钮导航版 | 简化版本，使用按钮导航 |
| **v2023.11.19** | `鉴伪微信小程序初版1/` | 2023-11-19 | 初始版本 | 基础功能实现 |
| **展示版** | `鉴伪微信小程序展示版（无进度条）/` | - | 展示版本 | 用于演示，无进度条 |
| **美化版** | `鉴伪微信小程序 美化/` | - | 界面美化版 | 优化了视觉效果 |
| **爆改版** | `鉴伪微信小程序爆改版/` | - | 重构版本 | 大幅重构的版本 |

### 🔧 版本演进历程

#### 1. 初始版本 (v2023.11.19)
- **基础功能**: 仅支持音频、视频、图像三种媒体类型的简单鉴伪
- **页面结构**: 简单的卡片式导航
- **技术特点**: 基础的小程序开发，无子包设计

#### 2. 架构升级 (v2023.12.03)
- **重大改进**: 引入子包架构，优化代码组织
- **功能扩展**: 增加算法展示页面
- **用户体验**: 改进导航结构，提升加载性能

#### 3. 界面优化 (v2023.12.06)
- **视觉升级**: 重新设计用户界面
- **交互优化**: 改进用户操作流程
- **品牌统一**: 统一视觉风格和品牌元素

#### 4. 功能完善 (v2023.12.21 - v2023.12.31)
- **算法集成**: 完整集成5种AI鉴伪算法
- **结果展示**: 详细的多维度结果展示
- **性能优化**: 优化加载速度和用户体验

### 🆚 关键差异对比

#### 功能差异
| 功能模块 | 初版 | 1203版本 | 1231版本 |
|----------|------|----------|----------|
| 媒体类型支持 | 音频、视频、图像 | 音频、视频、图像 | 音频、视频、图像 |
| AI算法数量 | 基础算法 | 5种算法 | 5种算法 |
| 子包架构 | ❌ | ✅ | ✅ |
| 算法展示页面 | ❌ | ✅ | ✅ |
| 详细结果展示 | ❌ | ❌ | ✅ |
| 下拉刷新 | ❌ | ✅ | ✅ |

#### 技术架构差异
| 技术特性 | 初版 | 1203版本 | 1231版本 |
|----------|------|----------|----------|
| 页面数量 | 5个 | 10个 | 10个 |
| 子包数量 | 0个 | 3个 | 3个 |
| 代码组织 | 简单 | 模块化 | 高度模块化 |
| 性能优化 | 基础 | 优化 | 高度优化 |

## ✨ 功能特性

### 🎵 音频鉴伪
- **支持格式**: MP3, WAV, FLAC, M4A等主流音频格式
- **检测算法**: 
  - MVSS (Multi-View Stereo Synthesis)
  - MABC (Multi-Attribute Binary Classification)
  - OSN (One-Shot Network)
  - W2V (Wave2Vec)
  - 传统音频分析算法
- **检测维度**: 人声伪造、音频合成、音轨篡改等

### 🎬 视频鉴伪
- **支持格式**: MP4, AVI, MOV, WMV等主流视频格式
- **检测算法**: 综合多种视觉和音频分析算法
- **检测维度**: 人脸替换、视频合成、帧间不一致等

### 🖼️ 图像鉴伪
- **支持格式**: JPG, PNG, BMP, GIF等主流图像格式
- **检测算法**: 基于深度学习的图像真实性检测
- **检测维度**: 图像合成、篡改检测、AI生成图像识别等

### 📊 结果展示
- **综合评分**: 多算法融合的综合伪造概率
- **详细分析**: 各算法的独立检测结果
- **可视化图表**: 直观的结果展示图表
- **置信度评估**: 检测结果的可靠性评估

## 🏗️ 技术架构

### 前端技术栈
- **框架**: 微信小程序原生开发
- **语言**: JavaScript (ES6+)
- **模板**: WXML (WeiXin Markup Language)
- **样式**: WXSS (WeiXin Style Sheets)
- **状态管理**: 小程序原生数据绑定

### 后端集成
- **API接口**: RESTful API设计
- **算法服务**: 多种AI鉴伪算法集成
- **文件处理**: 支持大文件上传和处理
- **结果缓存**: 优化检测结果响应速度

### 架构设计
```
小程序架构:
├── 主包 (Main Package)
│   ├── 首页 (index)
│   ├── 个人中心 (my)
│   ├── 综合鉴伪 (music)
│   ├── 算法展示 (show)
│   └── 结果展示 (result)
├── 音频子包 (package-music)
│   └── 音频鉴伪页面
├── 展示子包 (package-show)
│   ├── MABC算法展示
│   ├── MVSS算法展示
│   ├── OSN算法展示
│   ├── W2V算法展示
│   └── 传统算法展示
└── 结果子包 (package-result)
    └── 详细结果页面
```

## 🚀 安装与部署

### 环境要求
- **微信开发者工具**: 最新稳定版本
- **Node.js**: 14.0+ (可选，用于构建工具)
- **微信小程序账号**: 已注册的小程序开发者账号

### 安装步骤

1. **克隆项目**
   ```bash
   git clone [项目地址]
   cd 鉴伪微信小程序1231/鉴伪微信小程序1231/
   ```

2. **导入项目**
   - 打开微信开发者工具
   - 选择"导入项目"
   - 选择项目目录
   - 填入小程序AppID

3. **配置项目**
   - 检查 `app.json` 配置
   - 确认API接口地址配置
   - 测试基础功能

4. **编译运行**
   - 点击"编译"按钮
   - 在模拟器中测试功能
   - 真机调试验证

### 部署配置

#### 小程序配置
```json
{
  "pages": [
    "pages/index/index",
    "pages/my/my",
    "pages/music/music",
    "pages/show/show",
    "pages/result/result"
  ],
  "subpackages": [
    {
      "root": "package-music",
      "pages": ["pages/music"]
    },
    {
      "root": "package-show", 
      "pages": [
        "pages/MABC",
        "pages/MVSS",
        "pages/OSN",
        "pages/W2V",
        "pages/Tradition"
      ]
    },
    {
      "root": "package-result",
      "pages": ["pages/result"]
    }
  ]
}
```

#### API配置
在 `utils/util.js` 中配置API接口地址：
```javascript
const baseUrl = 'https://your-api-domain.com/api';
```

## 📖 使用说明

### 用户操作流程

1. **进入首页**
   - 打开小程序，进入主页面
   - 查看平台介绍和功能说明

2. **选择鉴伪类型**
   - 点击"综合鉴伪"进行多模态检测
   - 或选择特定算法进行专项检测

3. **上传文件**
   - 选择要检测的媒体文件
   - 支持音频、视频、图像格式
   - 文件大小限制：100MB以内

4. **等待检测**
   - 系统自动分析文件内容
   - 显示检测进度
   - 多算法并行处理

5. **查看结果**
   - 获取综合检测结果
   - 查看各算法详细分析
   - 了解伪造概率和置信度

### 功能模块说明

#### 综合鉴伪
- **功能**: 一键检测多种媒体类型
- **算法**: 自动选择最适合的检测算法
- **结果**: 提供综合评分和详细分析

#### 算法展示
- **MVSS**: 多视角立体合成检测
- **MABC**: 多属性二分类检测
- **OSN**: 一次性网络检测
- **W2V**: 基于Wave2Vec的音频检测
- **传统算法**: 经典信号处理算法

#### 结果展示
- **综合结果**: 整体伪造概率评估
- **分项结果**: 各算法的独立检测结果
- **可视化**: 图表展示检测过程
- **置信度**: 结果可靠性评估

## 📁 项目结构

```
鉴伪微信小程序1231/
├── app.js                 # 小程序入口文件
├── app.json              # 小程序配置文件
├── app.wxss              # 全局样式文件
├── components/           # 自定义组件
│   └── navigation-bar/   # 导航栏组件
├── images/              # 图片资源
│   ├── icon1.png        # 首页图标
│   ├── icon1-active.png # 首页激活图标
│   ├── icon2.png        # 我的图标
│   └── icon2-active.png # 我的激活图标
├── miniprogram_npm/     # npm包依赖
├── package-music/       # 音频子包
│   └── pages/
│       └── music/       # 音频鉴伪页面
├── package-result/      # 结果子包
│   └── pages/
│       └── result/      # 结果展示页面
├── package-show/        # 展示子包
│   └── pages/
│       ├── MABC/        # MABC算法展示
│       ├── MVSS/        # MVSS算法展示
│       ├── OSN/         # OSN算法展示
│       ├── Tradition/   # 传统算法展示
│       └── W2V/         # W2V算法展示
├── pages/               # 主包页面
│   ├── index/           # 首页
│   ├── my/              # 个人中心
│   ├── music/           # 综合鉴伪
│   ├── show/            # 算法展示入口
│   └── result/          # 检测结果
├── store/               # 状态管理
│   └── index.js         # 全局状态
├── utils/               # 工具函数
│   └── util.js          # 通用工具函数
├── sitemap.json         # 站点地图
└── project.config.json  # 项目配置
```

## 🛠️ 开发指南

### 开发环境搭建

1. **安装微信开发者工具**
   - 下载并安装最新版本
   - 注册小程序开发者账号
   - 获取AppID

2. **项目初始化**
   ```bash
   # 创建新项目
   # 或导入现有项目
   ```

3. **依赖管理**
   ```bash
   # 安装npm包（如需要）
   npm install
   ```

### 代码规范

#### JavaScript规范
- 使用ES6+语法
- 遵循小程序开发规范
- 使用有意义的变量和函数名
- 添加必要的注释

#### WXML规范
- 使用语义化标签
- 保持结构清晰
- 合理使用组件

#### WXSS规范
- 使用BEM命名规范
- 保持样式模块化
- 避免样式冲突

### 调试技巧

1. **控制台调试**
   ```javascript
   console.log('调试信息');
   ```

2. **真机调试**
   - 使用微信开发者工具的真机调试功能
   - 测试各种设备和网络环境

3. **性能监控**
   - 监控页面加载时间
   - 优化大文件上传性能
   - 减少不必要的网络请求

### 常见问题

#### 文件上传问题
- **问题**: 文件上传失败
- **解决**: 检查文件格式和大小限制

#### 网络请求问题
- **问题**: API请求超时
- **解决**: 检查网络连接和API地址配置

#### 页面跳转问题
- **问题**: 子包页面跳转失败
- **解决**: 检查页面路径和子包配置

## 🔄 版本控制

### Git工作流
- **主分支**: `main` - 稳定版本
- **开发分支**: `develop` - 开发版本
- **功能分支**: `feature/*` - 新功能开发
- **修复分支**: `hotfix/*` - 紧急修复

### 版本命名规范
- **格式**: `vYYYY.MM.DD`
- **示例**: `v2023.12.31`
- **说明**: 年月日格式，便于版本管理

### 发布流程
1. 功能开发和测试
2. 代码审查和合并
3. 版本标签创建
4. 发布到微信小程序平台

## 🤝 贡献指南

### 贡献方式
1. **问题反馈**: 提交Issue报告问题
2. **功能建议**: 提出新功能建议
3. **代码贡献**: 提交Pull Request
4. **文档完善**: 改进项目文档

### 贡献流程
1. Fork项目到个人仓库
2. 创建功能分支
3. 开发新功能或修复问题
4. 提交Pull Request
5. 等待代码审查和合并

### 代码审查标准
- 代码质量和规范性
- 功能完整性和正确性
- 性能影响评估
- 向后兼容性

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE.txt](LICENSE.txt) 文件了解详情。

## 🙏 致谢

- **中国传媒大学**: 项目发起方和技术支持
- **微信小程序团队**: 提供优秀的开发平台
- **开源社区**: 提供各种开源工具和库
- **所有贡献者**: 为项目发展做出贡献的开发者

---

**项目维护者**: CUC开发团队  
**最后更新**: 2023年12月31日  
**项目状态**: 活跃维护中




