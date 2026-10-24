# C-Learning

学习 C 语言的练习仓库。按章节/主题拆分目录，一个主题一个文件夹，代码和笔记一起提交。

## 目录约定

```
C-Learning/
├── src/            临时试验、环境自检
├── 01-基础语法/     按章节命名，序号 + 主题
├── 02-数组与字符串/
├── 03-指针/
├── 04-结构体/
├── 05-文件操作/
└── ...
```

新建章节时直接在根目录建 `序号-主题/`，里面放 `.c` 源文件和可选的 `notes.md`。

## 编译运行

**Visual Studio**：新建空项目，把 `.c` 文件加进去（注意文件扩展名是 `.c` 而不是 `.cpp`，否则 MSVC 会按 C++ 编译）。

**命令行（MinGW g++ / gcc）**：

```bash
cd 01-基础语法
gcc main.c -o main.exe -Wall
./main.exe
```

`-Wall` 建议常开，能提前抓出很多问题。

## 提交习惯

```bash
git add .
git commit -m "03-指针：完成指针与数组的练习"
git push
```

commit message 写清「做到哪了」，回头看进度一目了然。

## 说明

`.gitignore` 已排除 VS 的 `.vs/`、`Debug/`、`Release/`、`*.exe`、`*.obj` 等产物，只提交源码和笔记。
