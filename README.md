# 暧昧实验室 · 情侣互动游戏平台

两个人隔着屏幕也能一起玩的小游戏合集。支持远程联机对战，手机浏览器打开就能进。

🔗 线上地址：<https://rentijielv.030611.xyz>

## 仓库内容

本仓库目前只包含 `README.md`、`package.json`、`vercel.json` 三个文件，用于 Vercel 侧的部署配置。整体架构如下：

| 部分 | 技术 | 部署位置 |
| --- | --- | --- |
| 前端 | 纯 HTML + CSS + JavaScript（无框架） | Vercel |
| 后端 | PHP + MySQL | 宝塔面板（自有服务器） |

## 部署

### 前端（Vercel）

1. Vercel 导入本仓库
2. 构建命令与输出目录按 `vercel.json` 中的配置执行
3. 绑定自定义域名 `rentijielv.030611.xyz`

### 后端（宝塔）

1. 把后端代码上传到站点根目录
2. 导入 `schema.sql` 到 MySQL
3. 配置伪静态与 PHP 版本

## API 配置

前端通过全局变量 `window.API_BASE_URL` 指定后端地址，改这一处即可切换环境。

## 说明

本项目为私人使用的小工具，未做多租户与权限隔离，不建议直接对外开放数据接口。

## License

私有项目，未经授权请勿转载或商用。
