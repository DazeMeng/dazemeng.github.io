# 归去

> 归去，也无风雨也无晴。

基于 Firefly (Astro) 主题的个人博客。

访问地址：https://blog.l8865004.workers.dev

## 本地开发

需要 Node.js >= 22.23.0。

```bash
npm install --legacy-peer-deps --ignore-scripts
npm run dev
```

> 注：项目 packageManager 为 pnpm@11.22.0，云托管构建走 pnpm；本机（Windows 非管理员）pnpm isolated 模式符号链接失效，才用上面的 npm 替代装法。

## 部署

Cloudflare Workers 静态托管（wrangler.jsonc 指定 assets.directory=./dist）。
构建环境变量 NODE_VERSION=22.23.3；推送到 master 自动触发重新构建。
