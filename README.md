# SJTUThesis 示例模板

[![Build Status](https://github.com/sjtug/SJTUThesis/actions/workflows/build.yml/badge.svg)](https://github.com/sjtug/SJTUThesis/actions)
[![SJTUTeX](https://img.shields.io/github/v/release/sjtug/SJTUTeX?label=SJTUTeX)](https://github.com/sjtug/SJTUTeX) 
[![Join Discussions](https://img.shields.io/github/discussions/sjtug/SJTUThesis)](https://github.com/sjtug/SJTUThesis/discussions)

## 欢迎使用东华大学论文模板

本示例模板是应用上海交通大学学位论文（非官方）LaTeX 文档类 SJTUThesis 的一个完整实现，经过二次修改（不完美）后可用于东华大学论文。模板演示了排版中常用的例子，包括公式、表格、算法、参考文献等。
用户可以参考或者直接基于此示例文档撰写论文。

SJTUThesis 支持 XeTeX 与 LuaTeX 引擎，字符编码仅支持 UTF-8。

## 获取模板

普通用户可以直接 `clone` 。

```bash
git clone https://github.com/angustar/SJTUThesis-DHU.git
```

模版更新频繁，且只维护最新版。如有问题，可以先尝试升级模版，而后根据“反馈问题”一栏进行反馈。

如果需要在其他在线 LaTeX 平台上使用（比如 Overleaf (https://www.overleaf.com/)），您可以下载 [最新版压缩包](https://github.com/angustar/SJTUThesis-DHU/archive/refs/heads/master.zip)，然后上传至相应平台。请注意，Overleaf 默认使用 pdflatex 编译，您需要设置使用 XeLaTeX 编译器。

## 模板使用

如果你不熟悉 LaTeX 的编译流程，请**不要**直接使用编译器进行编译。针对不同的平台，模版提供了相应的编译脚本。在编译前，需要安装最新的 TeXLive 发行版。

### Linux 与 macOS 用户

推荐使用模版提供的 `Makefile` 进行编译，具体来说我们提供了如下几条可用的命令：

```bash
make all                      # 编译生成 main.pdf
make clean                    # 删除编译所产生的中间文件
make cleanall                 # 删除 main.pdf 和所有中间文件
make wordcount                # 论文字数统计
```

### Windows 用户

对于 Windows 用户，我们也提供了编译脚本 `Compile.bat`。可以双击直接编译，也可以在命令提示符窗口中使用脚本提供的额外功能：

```bash
.\Compile.bat thesis          # 编译生成 main.pdf
.\Compile.bat clean           # 删除编译所产生的中间文件
.\Compile.bat cleanall        # 删除 main.pdf 和所有中间文件
.\Compile.bat wordcount       # 论文字数统计
```

更多关于模板的实现细节以及使用信息，请查看使用文档 `sjtuthesis.pdf`。

## 致谢

* 感谢 [CTeX-kit](https://github.com/CTeX-org/ctex-kit) 提供了 LaTeX 的中文支持；
* 感谢那位最先制作出博士学位论文 LaTeX 模板的物理系同学；
* 感谢 William Wang 同学对模板移植做出的贡献；
* 感谢 [@weijianwen](https://github.com/weijianwen) 学长开创性的工作；
* 感谢 [@sjtug](https://github.com/sjtug) 对 0.10 及之后版本的开发和维护工作；
* 感谢 [@moment-ggw](https://github.com/moment-ggw) 对模板二次修改的贡献；
* 感谢所有为模板贡献过代码的[同学们](https://github.com/sjtug/SJTUThesis/graphs/contributors)，以及所有测试和使用模板的各位同学。

## 软件许可证

上海交通大学校徽校名图片（`sjtu-vi-logo-blue.pdf` 等）的版权归上海交通大学所有。

`sjtuthesis.cls` 文档类与相关附属文件使用 [LPPL](https://www.latex-project.org/lppl.txt) 授权。

其他部分使用 [Apache License 2.0](LICENSE) 授权。
