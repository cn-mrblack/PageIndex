<div align="center">

<a href="https://vectify.ai/pageindex" target="_blank">
  <img src="https://github.com/user-attachments/assets/46201e72-675b-43bc-bfbd-081cc6b65a1d" alt="PageIndex Banner" />
</a>

<br/>
<br/>

<p align="center">
  <a href="https://trendshift.io/repositories/14736" target="_blank"><img src="https://trendshift.io/api/badge/repositories/14736" alt="VectifyAI%2FPageIndex | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
</p>

# PageIndex：无向量、基于推理的RAG

<p align="center"><b>基于推理的RAG  ◦  无需向量数据库  ◦  无需分块  ◦  类人检索</b></p>

<h4 align="center">
  <a href="https://vectify.ai">🏠 首页</a>&nbsp; • &nbsp;
  <a href="https://chat.pageindex.ai">🖥️ 聊天平台</a>&nbsp; • &nbsp;
  <a href="https://pageindex.ai/mcp">🔌 MCP</a>&nbsp; • &nbsp;
  <a href="https://docs.pageindex.ai">📚 文档</a>&nbsp; • &nbsp;
  <a href="https://discord.com/invite/VuXuf29EUj">💬 Discord</a>&nbsp; • &nbsp;
  <a href="https://ii2abc2jejf.typeform.com/to/tK3AXl8T">✉️ 联系我们</a>&nbsp;
</h4>

</div>


<details open>
<summary><h3>📢 最新更新</h3></summary>

**🔥 发布内容：**
- [**PageIndex Chat**](https://chat.pageindex.ai)：第一个为专业长文档设计的类人文档分析代理平台。可通过 [MCP](https://pageindex.ai/mcp) 或 [API](https://docs.pageindex.ai/quickstart) 集成（测试版）。
<!-- - [**PageIndex Chat API**](https://docs.pageindex.ai/quickstart)：API 直接将 PageIndex 的高级长文档智能引入您的应用和工作流程。 -->
<!-- - [PageIndex MCP](https://pageindex.ai/mcp)：将 PageIndex 引入 Claude、Cursor 或任何支持 MCP 的代理。以基于推理的、类人的方式与长 PDF 聊天。 -->

**📝 文章：**
- [**PageIndex 框架**](https://pageindex.ai/blog/pageindex-intro)：介绍 PageIndex 框架 —— 一个**智能体化、上下文内**的**树索引**，使 LLM 能够对长文档执行**基于推理的**、**类人检索**，无需向量数据库或分块。
<!-- - [我们还需要 OCR 吗？](https://pageindex.ai/blog/do-we-need-ocr)：探讨基于视觉的、原生推理 RAG 如何挑战传统 OCR 管道，以及文档 AI 的未来为何可能是**无向量**和**基于视觉**的。 -->

**🧪 示例代码库：**
- [无向量 RAG](https://docs.pageindex.ai/cookbook/vectorless-rag-pageindex)：使用 PageIndex 的基于推理的 RAG 的最小、实践示例。无向量，无分块，类人检索。
- [基于视觉的无向量 RAG](https://docs.pageindex.ai/cookbook/vision-rag-pageindex)：免 OCR，纯视觉 RAG，使用 PageIndex 的原生推理检索工作流程，直接在 PDF 页面图像上工作。
</details>

---

# 📑 PageIndex 简介

您是否对专业长文档的向量数据库检索准确性感到沮丧？传统的基于向量的 RAG 依赖语义**相似性**而非真正的**相关性**。但**相似性 ≠ 相关性** — 我们在检索中真正需要的是**相关性**，而这需要**推理**。当处理需要领域专业知识和多步骤推理的专业文档时，相似度搜索往往力不从心。

受 AlphaGo 启发，我们提出了 **[PageIndex](https://vectify.ai/pageindex)** — 一个**无向量、基于推理的 RAG** 系统，它从长文档构建**层次化树索引**，并使用 LLM 对该索引进行**推理**，以实现**智能体化、上下文感知的检索**。
它模拟了*人类专家*通过**树搜索**导航和从复杂文档中提取知识的方式，使 LLM 能够*思考*和*推理*，找到最相关的文档部分。PageIndex 的检索分为两个步骤：

1. 生成文档的“目录”**树结构索引**
2. 通过**树搜索**执行基于推理的检索

<div align="center">
  <a href="https://pageindex.ai/blog/pageindex-intro" target="_blank" title="The PageIndex Framework">
    <img src="https://docs.pageindex.ai/images/cookbook/vectorless-rag.png" width="70%">
  </a>
</div>

### 🎯 核心功能

与传统的基于向量的 RAG 相比，**PageIndex** 具有以下特点：
- **无向量数据库**：使用文档结构和 LLM 推理进行检索，而非向量相似度搜索。
- **无需分块**：文档按自然章节组织，而非人工分块。
- **类人检索**：模拟人类专家导航和从复杂文档中提取知识的方式。
- **更好的可解释性和可追溯性**：检索基于推理 —— 可追溯且可解释，带有页面和章节引用。不再有不透明的、近似的向量搜索（"氛围检索"）。

PageIndex 支持的基于推理的 RAG 系统在 FinanceBench 上实现了**98.7%的准确率**[最新状态](https://github.com/VectifyAI/Mafin2.5-FinanceBench)，在专业文档分析中表现优于基于向量的 RAG 解决方案（有关详细信息，请参阅我们的 [博客文章](https://vectify.ai/blog/Mafin2.5)）。

### 📍 探索 PageIndex

要了解更多信息，请参阅 [PageIndex 框架](https://pageindex.ai/blog/pageindex-intro) 的详细介绍。查看此 GitHub 仓库获取开源代码，以及 [示例代码库](https://docs.pageindex.ai/cookbook)、[教程](https://docs.pageindex.ai/tutorials) 和 [博客](https://pageindex.ai/blog) 以获取更多使用指南和示例。

PageIndex 服务可作为 ChatGPT 风格的 [聊天平台](https://chat.pageindex.ai) 使用，也可通过 [MCP](https://pageindex.ai/mcp) 或 [API](https://docs.pageindex.ai/quickstart) 集成。

### 🛠️ 部署选项
- **自托管** — 使用此开源仓库在本地运行。
- **云服务** — 立即在我们的 [聊天平台](https://chat.pageindex.ai/) 上试用，或通过 [MCP](https://pageindex.ai/mcp) 或 [API](https://docs.pageindex.ai/quickstart) 集成。
- **企业版** — 私有或本地部署。[联系我们](https://ii2abc2jejf.typeform.com/to/tK3AXl8T) 或 [预约演示](https://calendly.com/pageindex/meet) 了解更多详情。

### 🧪 快速上手

- 尝试 [**无向量 RAG**](https://github.com/VectifyAI/PageIndex/blob/main/cookbook/pageindex_RAG_simple.ipynb) 笔记本 — 使用 PageIndex 进行基于推理的 RAG 的*最小*、实践示例。
- 体验 [*基于视觉的无向量 RAG*](https://github.com/VectifyAI/PageIndex/blob/main/cookbook/vision_RAG_pageindex.ipynb) — 无需 OCR；直接在页面图像上工作的最小、原生推理 RAG 管道。

<div align="center">
  <a href="https://colab.research.google.com/github/VectifyAI/PageIndex/blob/main/cookbook/pageindex_RAG_simple.ipynb" target="_blank" rel="noopener">
    <img src="https://img.shields.io/badge/Open_In_Colab-无向量_RAG-orange?style=for-the-badge&logo=googlecolab" alt="Open in Colab: Vectorless RAG" />
  </a>
  &nbsp;&nbsp;
  <a href="https://colab.research.google.com/github/VectifyAI/PageIndex/blob/main/cookbook/vision_RAG_pageindex.ipynb" target="_blank" rel="noopener">
    <img src="https://img.shields.io/badge/Open_In_Colab-视觉_RAG-orange?style=for-the-badge&logo=googlecolab" alt="Open in Colab: Vision RAG" />
  </a>
</div>

---

# 🌲 PageIndex 树结构
PageIndex 可以将冗长的 PDF 文档转换为语义**树结构**，类似于*目录*，但针对大型语言模型（LLM）进行了优化。它非常适合：财务报告、监管文件、学术教科书、法律或技术手册，以及任何超过 LLM 上下文限制的文档。

下面是一个 PageIndex 树结构示例。另请参阅更多示例 [文档](https://github.com/VectifyAI/PageIndex/tree/main/tests/pdfs) 和生成的 [树结构](https://github.com/VectifyAI/PageIndex/tree/main/tests/results)。

```jsonc
...
{
  "title": "金融稳定性",
  "node_id": "0006",
  "start_index": 21,
  "end_index": 22,
  "summary": "美联储 ...",
  "nodes": [
    {
      "title": "监测金融脆弱性",
      "node_id": "0007",
      "start_index": 22,
      "end_index": 28,
      "summary": "美联储的监测 ..."
    },
    {
      "title": "国内和国际合作与协调",
      "node_id": "0008",
      "start_index": 28,
      "end_index": 31,
      "summary": "2023年，美联储合作 ..."
    }
  ]
}
...
```

您可以使用此开源仓库生成 PageIndex 树结构，或使用我们的 [API](https://docs.pageindex.ai/quickstart)

---

# ⚙️ 包使用方法

您可以按照以下步骤从 PDF 文档生成 PageIndex 树。

### 1. 安装依赖项

```bash
pip3 install --upgrade -r requirements.txt
```

### 2. 设置您的 OpenAI API 密钥

在根目录创建一个 `.env` 文件并添加您的 API 密钥：

```bash
CHATGPT_API_KEY=your_openai_key_here
```

### 3. 在您的 PDF 上运行 PageIndex

```bash
python3 run_pageindex.py --pdf_path /path/to/your/document.pdf
```

<details>
<summary><strong>可选参数</strong></summary>
<br>
您可以使用额外的可选参数自定义处理：

```
--model                 使用的 OpenAI 模型（默认：gpt-4o-2024-11-20）
--toc-check-pages       检查目录的页面数（默认：20）
--max-pages-per-node    每个节点的最大页数（默认：10）
--max-tokens-per-node   每个节点的最大 token 数（默认：20000）
--if-add-node-id        添加节点 ID（是/否，默认：是）
--if-add-node-summary   添加节点摘要（是/否，默认：是）
--if-add-doc-description 添加文档描述（是/否，默认：是）
```
</details>

<details>
<summary><strong>Markdown 支持</strong></summary>
<br>
我们还为 PageIndex 提供 Markdown 支持。您可以使用 `-md_path` 标志为 Markdown 文件生成树结构。

```bash
python3 run_pageindex.py --md_path /path/to/your/document.md
```

> 注意：在这个函数中，我们使用 "#" 来确定节点标题及其层级。例如，"##" 是 2 级，"###" 是 3 级，以此类推。确保您的 Markdown 文件格式正确。如果您的 Markdown 文件是从 PDF 或 HTML 转换而来，我们不建议使用此函数，因为大多数现有转换工具无法保留原始层级。相反，使用我们的 [PageIndex OCR](https://pageindex.ai/blog/ocr)（专门设计用于保留原始层级）将 PDF 转换为 Markdown 文件，然后使用此函数。
</details>

<!--

# ☁️ 使用 PageIndex OCR 改进树生成

此仓库旨在为简单 PDF 生成 PageIndex 树结构，但许多实际用例涉及难以通过经典 Python 工具解析的复杂 PDF。然而，从 PDF 文档中提取高质量文本仍然是一个非平凡的挑战。大多数 OCR 工具仅提取页面级内容，失去了更广泛的文档上下文和层级结构。

为了解决这个问题，我们引入了 PageIndex OCR — 第一个专为保留文档全局结构而设计的长上下文 OCR 模型。PageIndex OCR 在识别跨文档页面的真实层级和语义关系方面显著优于其他领先的 OCR 工具，例如来自 Mistral 和 Contextual AI 的工具。

- 在我们的 [仪表板](https://dash.pageindex.ai/) 上体验 PageIndex OCR 的下一代 OCR 质量。
- 通过我们的 [API](https://docs.pageindex.ai/quickstart) 将 PageIndex OCR 无缝集成到您的堆栈中。

<p align="center">
  <img src="https://github.com/user-attachments/assets/eb35d8ae-865c-4e60-a33b-ebbd00c41732" width="80%">
</p>
-->

---

# 📈 案例研究：PageIndex 引领金融 QA 基准

[Mafin 2.5](https://vectify.ai/mafin) 是一个由 **PageIndex** 支持的用于金融文档分析的基于推理的 RAG 系统。它在 [FinanceBench](https://arxiv.org/abs/2311.11944) 基准上实现了**98.7%的准确率**[最新状态](https://github.com/VectifyAI/Mafin2.5-FinanceBench)，显著优于传统的基于向量的 RAG 系统。

PageIndex 的层级索引和推理驱动的检索能够精确导航和提取复杂金融报告（如 SEC 文件和收益披露）中的相关上下文。

探索完整的 [基准结果](https://github.com/VectifyAI/Mafin2.5-FinanceBench) 和我们的 [博客文章](https://vectify.ai/blog/Mafin2.5)，获取详细的比较和性能指标。

<div align="center">
  <a href="https://github.com/VectifyAI/Mafin2.5-FinanceBench">
    <img src="https://github.com/user-attachments/assets/571aa074-d803-43c7-80c4-a04254b782a3" width="70%">
  </a>
</div>

---

# 🧭 资源

* 🧪 [示例代码库](https://docs.pageindex.ai/cookbook/vectorless-rag-pageindex)：实践、可运行的示例和高级用例。
* 📖 [教程](https://docs.pageindex.ai/doc-search)：实用指南和策略，包括*文档搜索*和*树搜索*。
* 📝 [博客](https://pageindex.ai/blog)：技术文章、研究见解和产品更新。
* 🔌 [MCP 设置](https://pageindex.ai/mcp#quick-setup) 和 [API 文档](https://docs.pageindex.ai/quickstart)：集成细节和配置选项。

---

# ⭐ 支持我们
如果您喜欢我们的项目，请给我们一个星标 🌟。谢谢！

<p>
  <img src="https://github.com/user-attachments/assets/eae4ff38-48ae-4a7c-b19f-eab81201d794" width="80%">
</p>

### 联系我们

[![Twitter](https://img.shields.io/badge/Twitter-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/PageIndexAI)&nbsp;
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/vectify-ai/)&nbsp;
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/invite/VuXuf29EUj)&nbsp;
[![联系我们](https://img.shields.io/badge/Contact_Us-3B82F6?style=for-the-badge&logo=envelope&logoColor=white)](https://ii2abc2jejf.typeform.com/to/tK3AXl8T)

---

© 2025 [Vectify AI](https://vectify.ai)
