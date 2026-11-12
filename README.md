# 黎健毓 · ALARA

我的个人网站，记录项目经历、技术实践和产品方向的探索。

**在线访问：** https://alara-li.github.io/

## 页面内容

- 个人介绍与当前探索方向
- 智能多肉生长装置、RoboMaster 步兵机器人、智能三子棋机械臂
- 技术能力、学习经历与 GitHub 联系入口

项目介绍基于已有经历；Linux 与开源标注为探索方向。页面插图为功能或主题示意，不代表项目实物照片。完整简历、个人电话和出生日期不包含在站点中。

## 技术与结构

纯 HTML、CSS、SVG，配合本地 WebP 配图与 WOFF2 字体，无构建依赖、跟踪脚本或后端服务。支持手机布局、键盘导航、原生项目详情展开以及减少动画偏好。

视觉采用黑白杂志排版：Instrument Serif 英文标题、Noto Serif SC 中文标题、大幅作品配图和充分留白。字体与许可证均保存在 `assets/`，页面不向外部字体服务发出请求。智能植物装置配图为项目已有的 AI 辅助概念设计图，保留原图标识，并非已交付样机的实物照片。

```text
index.html          页面内容
styles.css          样式与响应式布局
assets/             图标、概念配图、本地字体及许可证
DESIGN.md           设计规则与参考 skills
.nojekyll           让 GitHub Pages 直接发布静态文件
```

## 本地预览

在此目录执行：

```bash
python -m http.server 8080
```

打开 http://localhost:8080 。按 Ctrl+C 停止服务。

## GitHub Pages 部署

仓库名称：`alara-li.github.io`。

在仓库 **Settings → Pages → Build and deployment** 中：

1. Source 选择 **Deploy from a branch**。
2. Branch 选择 **main**，目录选择 **/(root)**。
3. 点击 **Save**，等待 GitHub Pages 构建完成。

后续提交到 `main` 即触发网站更新。

## 更新内容

直接修改 `index.html` 中对应段落。新增项目时，记录真实角色、已经完成的功能与验证结果，并保持探索中和已完成内容的区别。样式集中在 `styles.css`。
