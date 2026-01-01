
# Mult-PDF Splitter & Merger Pro

# PDF 超级工坊：多文件混排与分割工具

### 🔒 100% Client-Side Processing | 纯本地处理，拒绝上传

**[English]**
Mult-PDF Splitter & Merger Pro is a secure, browser-based tool designed for researchers and professionals. Unlike traditional online converters, **your files never leave your computer**. All processing happens locally in your browser, ensuring absolute privacy for your sensitive documents and papers. It allows you to load multiple PDF sources, mix and match pages freely, and export them exactly how you want—either merged into one document or grouped into a ZIP archive.

**[中文]**
PDF 超级工坊是一款专为科研人员和专业人士设计的安全 PDF 处理工具。与传统的在线转换器不同，本工具**绝不会上传您的文件**。所有的分割、合并与压缩操作均在您的浏览器本地完成，最大限度地保护您的文档隐私。支持同时加载多个 PDF 源文件，您可以自由跨文件提取页面、混合排版，并按需导出——既支持合并为单一 PDF，也支持按组分割打包下载。

---

### ✨ Key Features | 核心功能

* **🛡️ Privacy First (隐私优先):** Powered by WebAssembly technology, no data is sent to any server. Perfect for confidential contracts or unpublished research data.
* 基于 WebAssembly 技术，数据不经过服务器，非常适合处理保密合同或未发表的科研数据。


* **📚 Multi-Source Workbench (多文件作业台):** Upload multiple PDFs at once. The system automatically assigns IDs (A, B, C...). You can mix pages from File A and File B seamlessly.
* 支持批量上传。系统自动分配代号（A, B, C...），您可以无缝混合提取文件 A 和文件 B 的页面。


* **👁️ Visual Interaction (可视化交互):** Click on page thumbnails to automatically add them to your layout instructions. No need to memorize page numbers.
* 点击缩略图即可将页码自动添加到指令框，所见即所得，无需死记页码。


* **🚀 Advanced Grouping (高级分组):**
* **Merge Mode:** Combine `A1-5` and `B2` into a single continuous PDF.
* **Split Mode:** Use semicolons (`;`) to define groups. `A1-5; B1` creates two separate PDF files inside a ZIP.
* **合并模式：** 将不同来源的页面连接成一个完整的 PDF。
* **分割模式：** 使用分号（`;`）作为切割点，批量生成多个 PDF 文件并打包下载。



---

### 📝 Syntax Guide | 排版指令指南

The tool uses a simple syntax to organize pages.
本工具使用简洁的语法来组织页面。

| Syntax (语法) | Description (说明) | Example (示例) |
| --- | --- | --- |
| **A, B, C...** | **File Identifier (文件代号)**<br>

<br>Identifies which PDF the page comes from.<br>

<br>指向页面来源的 PDF 文件。 | `A1` (Page 1 of File A)<br>

<br>`B5` (Page 5 of File B) |
| **-** | **Range (范围)**<br>

<br>Selects a continuous range of pages.<br>

<br>选择连续的页面范围。 | `A1-5` (Pages 1 to 5 of File A) |
| **,** | **Comma (逗号)**<br>

<br>Separates pages within the same group.<br>

<br>连接同一组内的不同页面。 | `A1, A5, B2` |
| **;** | **Semicolon (分号)**<br>

<br>Separates distinct output files (in Split Mode).<br>

<br>分隔不同的输出文件（仅在分割模式下生效）。 | `A1-3; B1-2`<br>

<br>*(Output: 2 separate PDFs)* |

---

### 💡 Quick Example | 快速演示

**Scenario:** You have a main paper (File A) and supplementary material (File B).
**场景：** 您有一篇主论文（文件 A）和一份补充材料（文件 B）。

**Goal:** Create a new PDF containing the first 3 pages of the paper, followed by page 1 of the supplement.
**目标：** 生成一个新的 PDF，包含论文的前 3 页，紧接着补充材料的第 1 页。

> **Input:** `A1-3, B1`
> **Mode:** Merge (合并)

**Goal:** Split them into two separate files for archiving.
**目标：** 将它们拆分为两个独立文件归档。

> **Input:** `A1-3; B1`
> **Mode:** Split & Group (分割)

---

### 🛠️ Tech Stack | 技术栈

* **PDF-Lib:** For robust PDF manipulation and modification.
* **PDF.js:** For high-fidelity page rendering and preview.
* **JSZip:** For client-side file compression.
* **Tailwind CSS:** For a clean, responsive user interface.
