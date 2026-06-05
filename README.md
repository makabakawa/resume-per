# resume-per

`resume-per` 是一个用于实际简历改写的 Codex skill。  
`resume-per` is a Codex skill for practical resume rewriting.

它适用于这样一类任务：你已经有一份 demo 简历，但它还不够聚焦、不够精炼、不够利于招聘方快速筛选，需要被重构为更强的一页版、岗位定向版或双语版。这个 skill 以用户现有简历为输入，不负责凭空生成可信简历；在优化过程中，会优先调用或参考猎聘简历模板思路，对排版和内容同时进行调整。这个 skill 尤其面向算法、计算机视觉、LLM 应用、人工智能相关实习和校招场景。  
It is designed for cases where you already have a demo resume, but it still needs to become more targeted, shorter, cleaner, and easier for recruiters or interviewers to screen quickly. This skill uses an existing resume as the source input rather than inventing a credible resume from scratch, and it can use Liepin-style resume templates as the main reference for both layout and content optimization. It is especially suitable for algorithm, computer vision, LLM application, AI internship, and campus hiring scenarios.

## 使用前提 / Prerequisite

- 你需要先准备一份自己的 demo 简历，作为这个 skill 的输入基础。  
  You should prepare your own demo resume first, because this skill works from an existing source resume.
- 这个 skill 的核心能力是调优、重写、压缩和重排，而不是从零杜撰经历。  
  Its core capability is optimization, rewriting, compression, and restructuring, not fabricating experience from scratch.
- 当你希望版式和内容一起优化时，这个 skill 会优先调用或参考猎聘模板逻辑进行处理。  
  When layout and content both need improvement, this skill will prioritize Liepin-style template logic during optimization.

## 功能 / What It Does

- 针对明确岗位方向重写现有简历  
  Rewrites an existing resume for a concrete target role.
- 在需要时压缩为更有筛选力的一页版本  
  Compresses the resume into a stronger one-page version when required.
- 围绕“技术方法 + 实际动作 + 结果指标”重写项目经历  
  Rewrites project bullets around methods, actions, and measurable results.
- 在需要时结合猎聘模板思路优化模块层级、版式节奏和内容呈现  
  Uses Liepin-style template logic when needed to improve section hierarchy, layout rhythm, and content presentation.
- 支持中文、英文或中英双语简历  
  Supports Chinese, English, or bilingual resumes.
- 保留硬事实，删除冗余、空泛或削弱说服力的内容  
  Preserves factual details while removing weak, redundant, or low-value content.
- 以最终可交付的 PDF 简历为输出标准  
  Uses final PDF-ready delivery as the output standard.

## 适用场景 / Suitable Scenarios

- 技术实习简历优化  
  Technical internship resume revision.
- 算法 / 计算机视觉 / AI 岗位定向改写  
  Resume targeting for algorithm, computer vision, or AI roles.
- 面向外企投递的双语简历整理  
  Bilingual resume preparation for international or foreign-company applications.
- 将学术化、信息过载的简历压缩为招聘友好版本  
  Converting a content-heavy academic resume into a recruiter-friendly version.
- 参考平台模板逻辑重组版式，但不复制模板废话  
  Rebuilding a resume with platform-inspired layout logic without copying template filler.

## 仓库结构 / Repository Structure

```text
.
├── SKILL.md
└── agents/
    └── openai.yaml
```

## 安装方式 / Install

将本仓库复制到你的 Codex skills 目录，并命名为：  
Copy this repository into your Codex skills directory as:

```text
$CODEX_HOME/skills/resume-per
```

Windows 常见路径：  
Typical Windows path:

```text
C:\Users\<your-user>\.codex\skills\resume-per
```

## 调用方式 / Invoke

示例提示词：  
Example prompts:

```text
Use $resume-per to rewrite this resume into a one-page computer-vision internship version.
```

```text
使用 $resume-per，把这份简历改成一页内、面向算法岗的版本，并输出 PDF。
```

对于非常明确的简历改写请求，这个 skill 也支持隐式触发。  
This skill also supports implicit invocation for clear resume-rewrite requests.

## 设计标准 / Design Standard

这个 skill 是刻意收窄范围、强调执行质量的。  
This skill is intentionally narrow and execution-oriented.

- 不做泛泛的职业规划建议  
  No generic career coaching.
- 不保留模板说明性废话  
  No decorative template explanation.
- 不堆砌无法自证的自我评价  
  No unverifiable self-praise.
- 不输出字面对齐但读起来生硬的中英翻译  
  No literal but awkward bilingual translation.

目标输出很明确：简洁、可辩护、岗位相关，并且能在短时间筛选中快速传达价值。  
The target output is simple: concise, defensible, job-targeted, and easy to screen quickly.
