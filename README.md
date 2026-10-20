# 文献阅读与分析 Skill

版本：V1.0

## 文件结构

```text
skill/
  README.md
  paper-reading-analysis/
    SKILL.md
```

提取论文元数据，按原文标题生成 Mermaid 思维导图，并形成研究背景、研究方法、研究意义和研究不足四部分中文笔记。缺失信息标注未知，区分作者观点、原文事实和分析者判断。

## 使用

将 paper-reading-analysis 文件夹复制到支持 SKILL.md 的工具的技能目录；实际发现和加载方式取决于使用工具。文件不依赖本机绝对路径或额外脚本。

示例请求：使用 paper-reading-analysis 分析我提供的论文，完成基本信息、原文标题思维导图及四部分笔记。

## 后续更新与版本

以 GitHub 仓库中的文件为维护来源。修改 SKILL.md 后同步更新 metadata.version，提交时说明修改内容。建议修正文案用 V1.0.1，新增兼容能力用 V1.1，改变输出约定用 V2.0。

首次发布可在 GitHub Releases 创建标签 v1.0.0，标题 V1.0，指向包含这两个文件的提交。后续版本各自创建新标签，不移动旧标签。

本地维护示例（首次克隆后在仓库目录执行）：

```sh
git pull --ff-only
git add paper-reading-analysis/SKILL.md README.md
git commit -m "Improve paper analysis instructions"
git push
```

需要固定版本时使用对应标签；更新已安装的 Skill 时，从选定版本复制整个 paper-reading-analysis 文件夹。GitHub 的提交不会自动同步到各工具已安装的副本。

本仓库仅保存 Skill 指令，不包含论文原文或私人阅读笔记。
