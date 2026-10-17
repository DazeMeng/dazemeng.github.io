# 归去

> 归去，也无风雨也无晴。

基于 Firefly (Astro) 主题的个人博客。

访问地址：https://dazemeng.github.io

## 本地开发

需要 Node.js >= 22.23.0。

```bash
npm install --legacy-peer-deps --ignore-scripts
npm run dev
```

> 注：项目 packageManager 为 pnpm@11.22.0，云端构建走 pnpm；本机（Windows 非管理员）pnpm isolated 模式符号链接失效，才用上面的 npm 替代装法。

## 部署

GitHub Pages（本仓库即用户页 dazemeng.github.io，master 推送自动构建部署）。
部署 workflow 在 `.github/workflows/deploy.yml`——**该目录无法经 API 写入**（token 无 workflow scope），由 GitHub 网页端维护；本地推送脚本用 base_tree 增量模式保留它。
