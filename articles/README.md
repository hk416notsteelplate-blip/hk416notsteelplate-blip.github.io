# Markdown 文章上传说明

## 文件夹

- `intro/`：介绍板块
- `01/` 到 `04/`：对应编号栏目
- 每个文件夹的 `intro.md` 是进入板块时默认展示的介绍
- `example.md` 是文字和图片示例，可以复制后修改

## 上传文章

进入对应文件夹，选择 **Add file → Upload files**，上传 .md 文件并提交。文件名建议使用英文字母、数字和连字符，例如 `my-first-post.md`。不要覆盖 `intro.md`，除非你要修改默认介绍。

每个 Markdown 文件开头保留下面的设置块：

```yaml
---
title: "文章标题"
subtitle: "可选小标题"
order: 20
layout: null
---
```

然后空一行，开始写 Markdown 正文。小标题可以删除。数字较小的 order 会排在前面，intro.md 始终排在最前面。

上传时间默认调用 GitHub 的文件首次提交时间；API 暂时不可用时会显示提示。也可以在设置块中加 `uploaded_at: "2026-10-12T19:00:00+08:00"`，使用自己的时间。

## 图片

可以将图片放在 `assets/`，从文章里写 `![说明](../../assets/photo.jpg)`。也可以在文章文件夹新建 images 文件夹，写 `![说明](images/photo.jpg)`。外部完整 HTTPS 图片链接同样支持。

## 评论授权

使用 Utterances 将评论保存为本仓库的 GitHub Issues。仓库所有者需要打开 https://github.com/apps/utterances ，点击 Install，为本仓库授权；同时保持仓库 Issues 功能开启。随后读者可使用 GitHub 账号评论。评论标识使用文章源文件路径，不受标题修改影响。移动或重命名文件会形成新的评论串。
