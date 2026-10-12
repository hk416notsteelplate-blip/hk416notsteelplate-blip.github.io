---
title: "栏目 02 · Markdown 示例文章"
subtitle: "文字、图片、表格和代码的排版示例"
order: 10
layout: null
---

## 一、普通文字

这是一篇可以直接修改的示例文章。正文支持 **加粗**、*斜体*、~~删除线~~和 `行内代码`。

每个段落之间空一行，就会形成独立段落。标题和可选小标题会从文件顶部的设置读取，上传时间默认读取 GitHub 的首次提交记录。

### 小标题示例

使用 `##` 表示二级标题，`###` 表示三级标题。

## 二、列表与引用

- 第一条记录
- 第二条记录
- 第三条记录

1. 在 GitHub 打开这个板块的文件夹。
2. 上传或编辑 Markdown 文件。
3. 提交修改，等待网站自动发布。

> 这是引用样式。可以放引文、补充说明或者自己的备注。

## 三、图片

![示例图片：暮色中的山峰](../../assets/article-sample.svg)

上图使用站内图片路径。也可以使用 `![说明](https://example.com/photo.jpg)` 插入外部图片。

## 四、表格

| 内容 | 写法 | 是否可选 |
| --- | --- | --- |
| 文章标题 | title | 否 |
| 小标题 | subtitle | 是 |
| 上传时间 | uploaded_at | 是，省略时读取 GitHub |
| 排序 | order | 是 |

## 五、代码

```cpp
#include <iostream>
using namespace std;

int main()
{
    cout << "Hello, Mayuri!" << endl;
    return 0;
}
```

---

文章末尾是 GitHub 评论区。各篇文章有独立的评论串。
