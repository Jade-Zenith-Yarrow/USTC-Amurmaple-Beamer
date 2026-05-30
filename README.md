# USTC Amurmaple Beamer Theme

面向中国科学技术大学报告场景的 LaTeX Beamer 模板，在 [Amurmaple Beamer Theme](https://github.com/mchupin/Amurmaple) 及众多二次开发者的基础上整理而成。仅供学习参考。

## 预览

| 封面 | 目录 |
|----------|----------|
| ![](./Figures%20Display/main_页面_01.png) | ![](./Figures%20Display/main_页面_02.png) |

| 基础环境 | 图片 |
|----------|----------|
| ![](./Figures%20Display/main_页面_14.png) | ![](./Figures%20Display/main_页面_18.png) |

| 表格 | 算法 |
|----------|----------|
| ![](./Figures%20Display/main_页面_19.png) | ![](./Figures%20Display/main_页面_21.png) |

| 分隔页 | 参考文献 |
|----------|----------|
| ![](./Figures%20Display/main_页面_26.png) | ![](./Figures%20Display/main_页面_29.png) |

| 数学样式 | 致谢页 |
|----------|----------|
| ![](./Figures%20Display/main_页面_32.png) | ![](./Figures%20Display/main_页面_37.png) |

> [📄 下载完整 PDF 预览](./main.pdf)

## 环境要求

- **LuaLaTeX**（Delaunay 网格背景必需）
- 常用宏包：`ctex`、`luamesh`、`tcolorbox`、`algorithm2e` 等

## 快速开始
下载 .zip 解压直接运行 main.tex 即可

```bash
# 克隆仓库
git clone https://github.com/<your-username>/USTC-Amurmaple-Beamer.git
cd USTC-Amurmaple-Beamer

# 编译（含参考文献时建议四次）
lualatex main.tex
bibtex main.aux
lualatex main.tex
lualatex main.tex
```

## 项目结构

```
├── main.tex                  # 入口文件
├── beamerthemeAmurmaple.sty  # 主题样式
├── Configure/                # 宏包、命令、数学样式
├── Sections/                 # 正文内容
├── Figures/                  # 图片资源
├── Figures Display/          # PDF 预览截图
└── Bibliography/             # 参考文献
```

## 使用说明

1. 编辑 `Sections/TitlePageInformation.tex` 填写封面信息
2. 在 `main.tex` 中设置主题选项：`\usetheme[amurmapleblue, delaunay, nomail]{Amurmaple}`
3. 正文内容按节写在 `Sections/SectionX.tex` 中
4. 编译后生成的 `main.pdf` 即为完整使用手册

详细使用说明请参见编译后的 `main.pdf`。

## 主题选项

| 选项 | 说明 |
|------|------|
| `amurmapleblue` | USTC 蓝色主题 |
| `delaunay` | 封面/分隔页网格背景 |
| `nomail` | 隐藏左侧栏邮箱 |
| `nogauge` | 隐藏进度条 |

## 致谢

- 原始主题 [Amurmaple Beamer Theme](https://github.com/mchupin/Amurmaple) by Maxime CHUPIN
- 众多二次开发者的贡献

## 说明

本项目非官方模板，仅供学习参考。
