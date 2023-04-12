---
{"dg-publish":true,"permalink":"/系统/示例/Callout/","noteIcon":"1","created":"2023-03-20T21:29:17.000+08:00","updated":""}
---

# Callout


> [!NOTE] Title
> Contents

> [!quote] Title
> Contents

> [!bug] Title
> Contents

> [!check] Title
> Contents

> [!help] Title
> Contents

> [!todo] Title
> Contents

note
abstract, summary, tldr
info, todo
tip, hint, important
success, check, done
question, help, faq
warning, caution, attention
failure, fail, missing
danger, error
bug
example
quote, cite

> [!error] Title
> Contents

> [!example] Title
> Contents

> [!attention] Title
> Contents

> [!important] Title
> Contents

> [!failure] Title
> Contents

>[!info|fuchsia] Color name: fuchsia
> This is the callout color fuchsia



## Callout Blocks 语法介绍

用 `> [! 类型]` 即可使用 callout blocks 功能，**注意：每行内容前面都必须添加 `>`**

**有如下类型可供使用：**

- note、abstract、info、todo、tip、success、question
- warning、failure、danger、bug、example、quote

## Callout 默认显示效果

> [!INFO]
> 这是 callout blocks

> [!Note]
> 这是 callout blocks

> [!abstract]
> 这是 callout blocks

> [!todo]
> 这是 callout blocks

> [!tip]
> 这是 callout blocks

> [!success]
> 这是 callout blocks

> [!question]
> 这是 callout blocks

> [!warning]
> 这是 callout blocks

> [!failure]
> 这是 callout blocks

> [!danger]
> 这是 callout blocks

> [!bug]
> 这是 callout blocks

> [!example]
> 这是 callout blocks

> [!quote]
> 这是 callout blocks

## 使用进阶

> [!info] Callouts Title，可修改此处标题
> 这是 callout blocks
>
> [!note]- Callouts Title，可折叠展开
> 这是 callout blocks，我可以折叠展开
>
> [!info] Can callouts be nested? 可嵌套
>
> > [!todo] Yes!, they can.
> >
> > > [!note] You can even use multiple layers of nesting.

## 自定义 Callout Blocks

可用如下代码对 callout 进行自定义：

```css
.callout[data-callout="my-callout-type"] {
	--callout-color: 0, 0, 0; 
	/*去 https://lucide.dev/ 找到喜欢的 icon-id*/
	--callout-icon: icon-id; 
	--callout-icon: '<svg>...custom svg...</svg>'; 
}
```

### 自定义的 Callout Blocks 显示效果

> [!ob-example]- ob-example
> 我是 ob-example
>
> 我是 ob-example
>
> - 测试 ur list
> - test ur list
>
> [!ob-info]- ob-info
> 我是 ob-info
>
> 我是 ob-info
>
> - 测试 ur list
> - test ur list
>
> [!ob-note]- ob-note
> 我是 ob-note
>
> 我是 ob-note
>
> - 测试 ur list
> - test ur list
>
> [!ob-tip]- ob-tip
> 我是 ob-tip
>
> 我是 ob-tip
>
> - 测试 ur list
> - test ur list
>
> [!ob-success]- ob-success
> 我是 ob-success
>
> 我是 ob-success
>
> - 测试 ur list
> - test ur list
>
> [!ob-question]- ob-question
> 我是 ob-question
>
> 我是 ob-question
>
> - 测试 ur list
> - test ur list
>
> [!ob-warning]- ob-warning
> 我是 ob-warning
>
> 我是 ob-warning
>
> - 测试 ur list
> - test ur list
>
> [!ob-failure]- ob-failure
> 我是 ob-failure
>
> 我是 ob-failure
>
> - 测试 ur list
> - test ur list
>
> [!ob-quote] ob-quote
> 我是 ob-quote
>
> 我是 ob-quote
>
> - 测试 ur list
> - test ur list

### 使用 Callout 实现高亮块功能

> [!orange]
> 测试内容 *重要*
>
> `测试行内代码`
>
> - 测试 ur list
> - <font style="color: #42b983; font-weight: 500"> 高亮块功能很好用 </font>，我可以输入不同颜色的文本
> - ==非常棒的功能==
> - <font style="background: rgb(253, 226, 226); font-weight: 500; color: rgb(216, 57, 49)"> 显示有背景的文本高亮 </font>
> - [开始在 GitHub 上编写和格式化 - GitHub Docs](https://docs.github.com/cn/github/writing-on-github/getting-started-with-writing-and-formatting-on-github)，我也可输入 URL 链接
> - [[ToDo\|ToDo]]

> [!light-orange]
> 测试内容

> [!blue]
> 测试内容
>
> [!light-blue]
> 测试内容
>
> [!red]
> 测试内容
>
> [!light-red]
> 测试内容
>
> [!green]
> 测试内容
>
> [!light-green]
> 测试内容
>
> [!purple]
> 测试内容
>
> [!light-purple]
> 测试内容
>
> [!gray]
> 测试内容
>
> [!light-gray]
> 测试内容

## 参考

- [callout blocks 官方介绍](https://help.obsidian.md/How+to/Use+callouts)
- Related：[[Admonition 如何使用\|Admonition 如何使用]]~~不再推荐~~
