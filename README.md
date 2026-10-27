# Cyberl Blog 友情链接

本仓库收集并维护 [Cyberl Blog](https://kagaranakaki.top/) 的友情链接。审核通过的站点会显示在博客的[伙伴页面](https://kagaranakaki.top/friends/)。

## 如何申请

首选方式是使用 [GitHub 友链申请表](https://github.com/Cyberl-ty02/friends/issues/new?template=friend.yml)：

1. 登录 GitHub。
2. 打开申请表并填写网站资料。
3. 提交 Issue，等待人工审核。
4. 如资料不完整，根据 Issue 中的反馈补充信息。

使用 Issue Form 需要 GitHub 账号。不熟悉 Git 的访客无需 Fork 仓库、编辑 YAML 或上传图片。提交申请不代表自动通过，也不承诺固定审核时间。

## 申请资料与审核

申请时请提供：

- 站点名称和简短介绍；
- 完整的 HTTPS 站点地址；
- 可公开使用的头像或站点图片 URL；
- 对方的友链页面地址及互链情况；
- RSS/Atom Feed（选填）。

维护者会人工核对站点和链接是否真实有效、是否已有重复记录、图片是否可以公开使用，以及资料是否适合公开展示。外部 URL 的可访问性、安全性、内容和图片权利不能由表单自动证明；未经审核的资料不会自动合并或写入博客。

请勿公开提交真实姓名、电话、邮箱、私人社交账号、登录凭据、数据库信息或网站后台信息。

## 数据存储格式

`linklist.yml` 保存审核后的正式数据，并继续使用 Kratos-Rebirth 原生格式：

```yaml
friends:
  - title: "站点名称"
    description: "站点简介"
    image: "/images/friends/example.webp"
    link: "https://example.com/"
```

Issue Form 收集的是申请资料，不是可直接合并的 YAML。RSS 和对方友链页面仅供审核参考，不强制加入主题的数据模型；申请中的图片 URL 也是候选输入，不代表博客会直接热链该图片。

## 图片与同步

- 本仓库是友链审核与维护的权威来源。
- 博客仓库保留已审核 YAML 和图片的发布快照，构建时不会动态读取本仓库的 `main`。
- 维护者会人工审核图片，在需要时转换并保存为本地 WebP，再分别同步审核后的数据和必要图片。
- 不自动热链任意外部图片，也不自动接收或执行申请者提供的代码。

## 使用 Pull Request 申请

熟悉 Git 的申请者仍可 Fork 本仓库并提交 Pull Request，但必须遵循相同的人工审核、数据格式和图片规则，不能绕过审核流程。

本仓库最初的友链维护方式参考了 [Candinya](https://github.com/Candinya) 及 [Kratos : Rebirth 实例列表](https://awesome.krt.moe/show-my-site/)，在此致谢。
