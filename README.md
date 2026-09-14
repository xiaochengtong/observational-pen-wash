# 观察式钢笔淡彩 · Observational Pen Wash

一个给 AI 编程/agent 工具用的图像生成 skill：把任意旅行照片变成**观察式钢笔淡彩**——极简钢笔线稿与少量透明淡彩，断续线条、观察痕迹、大胆留白，呈现私人旅行手记般的艺术感。

> 线为观察、彩为情绪、断为呼吸、白为记忆。

## 效果

把普通旅行照片变成有呼吸感的手绘速写，像画家旅行时随手画在本子上的一页，适合做手账插画、旅行纪念图、艺术海报。

## 安装

**Kimi Code / Claude Code / Codex / 豆包工作模式 等 agent 工具**：把本仓库的 `SKILL.md` 复制到你的 skills 目录（如 `~/.user_skills/observational-pen-wash/`），agent 会在你说"把这张照片做成钢笔淡彩"时自动调用。

**任何生图工具（ChatGPT / Midjourney / 即梦等）**：不用安装，直接按下面的配方手写 prompt。

## 用法（30 秒版）

1. 选一张照片，写下三行：核心轮廓是什么 / 哪1-2个区域上淡彩 / 主色是哪2-3个
2. 定线稿：只画最关键的轮廓和结构线，断续不连贯，有手绘感
3. 定淡彩：只在重点区域少量晕染，70%以上留白
4. 按五段式拼 prompt：

```
observational pen wash, minimalist pen and ink sketch with transparent watercolor washes,
travel journal sketchbook style, hand-drawn imperfect lines,
keep the [核心轮廓] recognizable, rendered in minimal broken pen lines,
only 1-2 areas with transparent watercolor washes of [主色], soft bleeding edges,
70% of the canvas left as white paper,
textured cream sketchbook paper background, unfinished sketch feeling,
no continuous clean lines, no full color coverage, no Chinese text, no watermark
```

完整规则（决策优先级、观察卡、线稿规则、淡彩规则、手记感细节、纠偏表、质量门）见 `SKILL.md`。

## 核心规则速览

- **手绘感第一**：线条有不完美、断续、轻重变化，不是矢量干净线条
- **极简线稿**：只画最关键的20%线条，保留80%想象空间
- **少量淡彩**：颜色只在1-3个区域，覆盖不超过40%画面
- **大胆留白**：留白占50%以上，这是"手记感"的核心
- **观察痕迹**：有未完成线条、涂改、标注，像画家正在观察

## License

MIT
