# LVGL Pinyin Dictionary Generator / LVGL 拼音字典生成器

[![License](https://img.shields.io/github/license/iamshiqing/lvgl-pinyin-dict-generator.svg)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/demo-online-blue)](https://iamshiqing.github.io/lvgl-pinyin-dict-generator)
[![Stars](https://img.shields.io/github/stars/iamshiqing/lvgl-pinyin-dict-generator.svg?style=social)](https://github.com/iamshiqing/lvgl-pinyin-dict-generator/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/iamshiqing/lvgl-pinyin-dict-generator.svg)](https://github.com/iamshiqing/lvgl-pinyin-dict-generator/issues)


> 🌐 A web-based tool for generating LVGL-compatible Pinyin dictionaries.  
> 🌏 一个用于生成 **LVGL 拼音字典** 的纯前端网页工具。

---

## 📖 Introduction | 简介

**LVGL Pinyin Dictionary Generator** 是一个纯前端网页工具，用于为 [LVGL](https://lvgl.io) 的中文输入法控件（如 `lv_100ask_pinyin_ime`）生成兼容的拼音字典文件（`.c` 格式）。  
无服务器、无依赖、可离线使用。

你只需输入字典名、Unicode 范围、额外汉字，即可一键生成可直接编译到 LVGL 工程中的 C 源文件。

---

## 🚀 Online Demo | 在线演示

👉 [https://iamshiqing.github.io/lvgl-pinyin-dict-generator](https://iamshiqing.github.io/lvgl-pinyin-dict-generator)

无需安装任何依赖，直接打开网页即可使用。

---

## 🧩 Features | 功能特性

| 功能 / Feature | 描述 / Description |
|----------------|--------------------|
| 🌈 图形化生成 | 可视化配置 LVGL 拼音字典 |
| ⚙️ 自动拼音匹配 | 基于 [pinyin-pro](https://github.com/zh-lx/pinyin-pro) 实时转换 |
| 🔠 多范围支持 | 支持多个 Unicode 段与附加符号 |
| 💾 一键下载 | 直接导出 `.c` 文件 |
| 💻 离线可用 | 无需后端、完全在浏览器中运行 |
| 🧱 完全兼容 LVGL | 输出结构匹配 `lv_100ask_pinyin_dict_t` |

---

## 📄 Usage | 使用方法

### 1️⃣ 打开网页
访问：  
[https://iamshiqing.github.io/lvgl-pinyin-dict-generator](https://iamshiqing.github.io/lvgl-pinyin-dict-generator)

### 2️⃣ 输入参数
- **字典名 / Dict Name**：生成的数组名（如 `my_pinyin_dict`）  
- **Unicode 范围 / Range**：如 `0x4E00-0x9FA5`  
- **附加符号 / Extra Symbols**：自定义字符（如 “你好世界”）

### 3️⃣ 点击生成
点击「生成字典」即可生成结果。

### 4️⃣ 下载文件
点击「下载 `.c` 文件」保存生成的拼音字典。

### 5️⃣ 集成 LVGL
将 `.c` 文件添加到你的 LVGL 工程中：

```c
#include "my_pinyin_dict.c"
lv_100ask_pinyin_ime_set_dict(ime, my_pinyin_dict);
```

## 🌟 Acknowledgements / 致谢

感谢所有为本项目提供灵感与支持的开源项目与社区。

---

### 💡 Open Source Projects | 开源项目

- [**LVGL**](https://lvgl.io)  
  高性能嵌入式图形界面库，为本项目提供了拼音输入法控件（`lv_100ask_pinyin_ime`）的使用场景。

- [**pinyin-pro**](https://github.com/zh-lx/pinyin-pro)  
  一个优秀的 JavaScript 拼音解析库，提供了高准确度的汉字转拼音功能。

---

### ❤️ Community | 社区

感谢开源社区的持续贡献与精神支持。  
你的每一个 Star、Fork、或建议，都是本项目前进的动力。
 


