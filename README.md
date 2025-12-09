# Mdocs 项目

这是一个使用 [Zensical](https://zensical.org/) 生成的网站。

## 快速开始

### 环境要求

- 需要安装 Zensical。请参考 [Zensical 官方文档](https://zensical.org/docs/getting-started/) 进行安装。

### 本地开发

1.  **启动本地服务器:**

    ```bash
    zensical serve
    ```

    此命令将启动一个本地 Web 服务器，您可以在浏览器中实时预览您的更改。

2.  **构建网站:**

    ```bash
    zensical build
    ```

    此命令会将您的 Markdown 文件构建成静态 HTML 网站，输出到 `site` 目录中。

### 创建新项目

您可以使用以下命令创建一个新的 Zensical 项目：

```bash
zensical new <project-name>
```

## 项目结构

```
Mdocs/
├── docs/
│   ├── index.md         # 网站首页
│   └── markdown.md      # Markdown 语法示例
├── zensical.toml        # Zensical 配置文件
└── README.md            # 本文件
```

- `docs/`: 存放所有 Markdown 文档源文件。
- `zensical.toml`: 项目的配置文件，您可以在此文件中配置网站名称、主题、导航、插件等。

## 功能特性

本项目已启用 Zensical 的多项功能，包括：

- **代码块复制**
- **内容选项卡**
- **图表 (Mermaid)**
- **脚注工具提示**
- **任务列表**
- **明暗主题切换**
- 还有更多功能请查看 `zensical.toml` 文件中的 `features` 列表。

## 版权

Copyright &copy; 2025 Rogerma
