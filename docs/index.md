---
icon: lucide/rocket
---

# 开始使用

要获取完整的文档，请访问 [zensical.org](https://zensical.org/docs/)。

## 命令

* [`zensical new`][new] - 创建一个新项目
* [`zensical serve`][serve] - 启动本地 Web 服务器
* [`zensical build`][build] - 构建您的网站

  [new]: https://zensical.org/docs/usage/new/
  [serve]: https://zensical.org/docs/usage/preview/
  [build]: https://zensical.org/docs/usage/build/

## 示例

### 警告框

> 可参考[文档](https://zensical.org/docs/authoring/admonitions/)

!!! note

    这是一个 **note** 警告框。用它来提供有用的信息。

!!! warning

    这是一个 **warning** 警告框。请小心！

### 详情

> 可参考[文档](https://zensical.org/docs/authoring/admonitions/#collapsible-blocks)

??? info "点击展开查看更多信息"
    
    此内容在您点击展开之前是隐藏的。
    非常适合用于常见问题解答或较长的解释。

## 代码块

> 可参考[文档](https://zensical.org/docs/authoring/code-blocks/)

``` python hl_lines="2" title="代码块"
def greet(name):
    print(f"Hello, {name}!") # (1)!

greet("Python")
```

1.  > 可参考[文档](https://zensical.org/docs/authoring/code-blocks/#code-annotations)

    代码注释允许将注释附加到代码行。

代码也可以内联高亮显示: `#!python print("Hello, Python!")`。

## 内容选项卡

> 可参考[文档](https://zensical.org/docs/authoring/content-tabs/)

=== "Python"

    ``` python
    print("Hello from Python!")
    ```

=== "Rust"

    ``` rs
    println!("Hello from Rust!");
    ```

## 图表

> 可参考[文档](https://zensical.org/docs/authoring/diagrams/)

``` mermaid
graph LR
  A[开始] --> B{有错误?};
  B -->|是| C[嗯...];
  C --> D[调试];
  D --> B;
  B ---->|否| E[太棒了!];
```

## 脚注

> 可参考[文档](https://zensical.org/docs/authoring/footnotes/)

这是一个带有脚注的句子。[^1]

将鼠标悬停在上面，可以看到工具提示。

[^1]: 这是脚注。


## 格式化

> 可参考[文档](https://zensical.org/docs/authoring/formatting/)

- ==这段文字被标记（高亮）了==
- ^^这段文字被插入（下划线）了^^
- ~~这段文字被删除（删除线）了~~
- H~2~O
- A^T^A
- ++ctrl+alt+del++

## 图标、表情符号

> 可参考[文档](https://zensical.org/docs/authoring/icons-emojis/)

* :sparkles: `:sparkles:`
* :rocket: `:rocket:`
* :tada: `:tada:`
* :memo: `:memo:`
* :eyes: `:eyes:`

## 数学公式

> 可参考[文档](https://zensical.org/docs/authoring/math/)

$$
\cos x=\sum_{k=0}^{\infty}\frac{(-1)^k}{(2k)!}x^{2k}
$$

!!! warning "需要配置"
    请注意，MathJax 是通过此页面上的 `script` 标签包含的，并且未在生成的默认配置中进行配置，以避免在不需要它的页面中包含它。有关如何在所有页面上配置它的详细信息，请参阅文档，如果它们比这些简单的入门页面更侧重于数学的话。

<script id="MathJax-script" async src="https://unpkg.com/mathjax@3/es5/tex-mml-chtml.js"></script>
<script>
  window.MathJax = {
    tex: {
      inlineMath: [["\\(", "\\)"]],
      displayMath: [["\\[", "\\]"]],
      processEscapes: true,
      processEnvironments: true
    },
    options: {
      ignoreHtmlClass: ".*|",
      processHtmlClass: "arithmatex"
    }
  };
</script>

## 任务列表

> 可参考[文档](https://zensical.org/docs/authoring/lists/#using-task-lists)

* [x] 安装 Zensical
* [x] 配置 `zensical.toml`
* [x] 编写出色的文档
* [ ] 随处部署

## 工具提示

> 可参考[文档](https://zensical.org/docs/authoring/tooltips/)

[将鼠标悬停在我身上][example]

  [example]: https://example.com "我是一个工具提示！"
