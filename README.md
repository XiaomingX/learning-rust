<div class="oranda-hide">

# Rustlings 🦀❤️

</div>

欢迎来到 Rustlings 项目！
这个项目包含了一些小练习，帮助你熟悉阅读和编写 Rust 代码，同时学习如何理解编译器的反馈。

我们建议你在学习 [官方 Rust 教程](https://doc.rust-lang.org/book/) 的同时，做 Rustlings 练习。官方教程是学习 Rust 的最全面的资源 📚️

另一个推荐的资源是 [Rust By Example](https://doc.rust-lang.org/rust-by-example/)，它包含了与 Rustlings 类似的代码示例和在线练习。

## 开始之前

### 安装 Rust

在安装 Rustlings 之前，你需要先安装 **最新版本的 Rust**。
请访问 [www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install) 按照说明进行安装。
这个过程也会安装 _Cargo_，Rust 的包管理器和项目管理工具。

> 🐧 如果你使用的是 Linux，确保你已经安装了 `gcc`（链接器）。  
> 你可以使用以下命令安装：  
> Deb: `sudo apt install gcc`  
> Dnf: `sudo dnf install gcc`  

> 🍎 如果你使用的是 macOS，确保你已经安装了 Xcode 以及其开发工具，可以通过运行 `xcode-select --install` 来安装。

### 安装 Rustlings

执行以下命令来下载并编译 Rustlings：

```bash
cargo install rustlings
```

<details>
<summary><strong>如果安装失败...</strong> (<em>点击展开</em>)</summary>

- 请确保你的 Rust 版本是最新的，使用 `rustup update` 来更新。
- 如果遇到问题，可以尝试添加 `--locked` 标志：`cargo install rustlings --locked`
- 如果问题依然存在，请 [报告问题](https://github.com/rust-lang/rustlings/issues/new)

</details>

### 初始化

安装完成后，执行以下命令来初始化 `rustlings/` 目录：

```bash
rustlings init
```

<details>
<summary><strong>如果找不到 <code>rustlings</code> 命令...</strong> (<em>点击展开</em>)</summary>

如果你使用 Linux 并通过包管理器安装了 Rust，可能遇到这个问题。

Cargo 会将二进制文件安装到 `~/.cargo/bin` 目录。  
但很多包管理器并不会自动将该目录添加到 `PATH` 环境变量中。

解决方法是：

- 手动将 `~/.cargo/bin` 添加到 `PATH` 中，或者
- 卸载通过包管理器安装的 Rust，并使用官方的 `rustup` 工具重新安装： [安装 Rust](https://www.rust-lang.org/tools/install)

</details>

初始化完成后，进入新创建的目录并启动 Rustlings，开始练习：

```bash
cd rustlings/
rustlings
```

## 开发环境

### 编辑器

我们推荐使用 [VS Code](https://code.visualstudio.com/) 编辑器，并安装 [rust-analyzer 插件](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)。  
不过任何支持 [rust-analyzer](https://rust-analyzer.github.io/) 的编辑器都可以用来完成练习。

### 终端

为了获得最佳体验，建议使用现代终端。Linux 和 macOS 默认的终端应该就足够了。  
在 Windows 上，我们推荐使用 [Windows Terminal](https://aka.ms/terminal)。

## 完成练习

这些练习按主题分类，存放在 `exercises/<topic>` 子目录下。每个主题都有一个附带的 `README.md` 文件，里面包含了一些资源，帮助你快速上手。我们建议你在开始之前先阅读这些资源 📚️

大部分练习中都会有一个错误，导致代码无法编译，你的任务就是修复它！  
一些练习中还包含了需要通过的测试，表示练习已经完成 ✅

查找 `TODO` 或 `todo!()`，了解需要修改的地方。  
在 _监视模式_ 中按 `h` 获取提示 💡

### 监视模式

安装完成后，可以通过运行 `rustlings` 启动 Rustlings。

它将进入 _监视模式_，按照预定顺序引导你完成练习（我们认为这是最适合新手的顺序）。  
每当你修改 `exercises/` 目录下的文件时，它会自动重新运行当前练习。

<details>
<summary><strong>如果无法检测到文件更改...</strong> (<em>点击展开</em>)</summary>

> 你可以添加 `--manual-run` 标志（`rustlings --manual-run`），进入手动模式，通过按 `r` 来手动重新运行当前练习。
>
> 如果你遇到问题，请 [报告问题](https://github.com/rust-lang/rustlings/issues/new)，并提供你的操作系统信息，以及是否在容器或虚拟机（例如 WSL）中运行 Rustlings。

</details>

### 练习列表

在 [监视模式](#监视模式) 中（启动 `rustlings` 后），可以按 `l` 打开交互式练习列表。

列表中可以查看每个练习的状态（已完成或待完成），并可以执行以下操作：

- `c`：跳转到其他练习（跳过某些练习或回到之前的练习）
- `r`：重置选定练习的状态和文件（之后需要在编辑器中重新打开该文件）

你还可以查看列表底部的所有可用快捷键。

## 有问题？

如果在做练习过程中遇到困难，而内置提示无法解决你的问题，欢迎在 [讨论区的 _Q&A_ 分类](https://github.com/rust-lang/rustlings/discussions/categories/q-a?discussions_q=) 提问。

## 第三方练习

第三方练习是由社区维护的练习集。你可以继续使用通过 `cargo install rustlings` 安装的 `rustlings` 程序来运行这些练习：

- [日本语版 Rustlings](https://github.com/sotanengel/rustlings-jp)：Rustlings 的日文翻译版本。

想要创建自己的 Rustlings 练习集吗？  
或者想翻译原版的 Rustlings 练习？请参考 [第三方练习指南](https://github.com/rust-lang/rustlings/blob/main/THIRD_PARTY_EXERCISES.md)。

## 继续前进

完成 Rustlings 后，可以通过构建自己的项目、贡献代码到 Rustlings 或者参与其他开源项目来继续提高 Rust 技能。

## 卸载 Rustlings

如果你想卸载 Rustlings，可以运行以下命令：

```bash
cargo uninstall rustlings
```
