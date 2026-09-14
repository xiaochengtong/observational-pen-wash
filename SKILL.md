---
name: observational-pen-wash
description: 把照片变成观察式钢笔淡彩(observational pen wash)——极简钢笔线稿与少量透明淡彩，断续线条、观察痕迹、大胆留白，呈现私人旅行手记般的艺术感。当用户想要钢笔淡彩、手绘速写、旅行手账、极简线稿、观察式手绘、私人旅行手记风格、把照片做成有呼吸感的手绘作品时使用。
---

# 观察式钢笔淡彩 Observational Pen Wash

**线为观察、彩为情绪、断为呼吸、白为记忆。**

照片还是那个场景，但被一只正在观察的手重新画了下来：极简的钢笔线稿，线条断续不连贯，像画家边看边画的痕迹；少量透明淡彩随意晕染，大部分区域大胆留白——这不是一张完整的画，而是一页私人旅行手记。

## 决策优先级(冲突时按此顺序)

1. 手绘感——线条有手绘的不完美、断续、轻重变化，不是矢量干净线条
2. 极简线稿——只画最关键的轮廓和结构线，不追求细节完整
3. 少量淡彩——颜色只在重点区域少量晕染，大部分区域留白
4. 大胆留白——留白占画面 50% 以上，这是"手记感"的核心
5. 观察痕迹——有画家正在观察的痕迹(未完成的线条、涂改、标注)

## 授权与隐私

- 用户给了照片并要求生成/改造，即视为已授权调用生图服务，不再追问
- 只把最终 prompt 和参考图发给生图服务；不传播、不另存用户原图

## 第一步：观察卡

读原图，逐项写下：

- **核心轮廓**：最有识别度的主体轮廓(建筑/人物/地标)，只画外轮廓和关键结构线
- **可省略区域**：哪些细节可以完全不画，交给留白
- **淡彩重点**：哪 1–2 个区域需要上淡彩(通常是主体或视觉重心)
- **原生色**：2–3 个主色(淡彩的来源，只用最有代表性的颜色)
- **观察视角**：画家站在哪里观察，视线高度和角度

## 第二步：钢笔线稿规则

### 断续线条
- 线条不是连续的，有断有续，像边看边画
- 轮廓线较重较实，内部结构线较轻较虚
- 远处的线条更断续更轻，近处的线条更实更重
- 允许有"画错又重画"的线条痕迹

### 极简结构
- 只画最关键的 20% 线条，保留 80% 的想象空间
- 建筑只画外轮廓和主要结构线，不画每扇窗户
- 人物只画剪影和动态线，不画五官细节
- 风景只画地平线和主要地形线

### 线条质感
- 钢笔线条，有轻微的粗细变化(落笔重、收笔轻)
- 线条颜色用深棕或深灰，不用纯黑
- 允许有轻微的线条抖动和不完美
- 部分区域用排线表示阴影，但排线要稀疏

## 第三步：淡彩规则

### 少量使用
- 全图只有 1–3 个区域上淡彩，其余全部留白
- 淡彩只覆盖画面的 20–30%，不超过 40%
- 颜色集中在主体或视觉重心，不在背景大面积铺色

### 透明晕染
- 颜色是透明的水彩感，可以看到下面的线条
- 颜色边缘有自然的晕染和水迹，不是锐利边界
- 允许颜色溢出线条边界，像手绘时的不小心
- 颜色有深浅变化，不是平涂

### 配色克制
- 从原图提炼 2–3 个主色，不超过 4 个
- 颜色降低饱和度，呈现旧纸张上的淡彩感
- 颜色之间可以有轻微的混色，但不混乱
- 不用纯黑/纯灰，阴影也用彩色(如熟褐、群青)

## 第四步：手记感细节

- **未完成感**：画面边缘有"没画完"的感觉，线条逐渐消失在留白中
- **观察标注**：可有极少量的手写英文标注(如日期、地点、简短笔记)，字体小而随意
- **纸张质感**：背景是有纹理的米白/浅米色纸张，不是纯白
- **涂改痕迹**：可有极轻微的涂改线或重画线，增加真实感
- **构图偏移**：主体不居中，偏左或偏右，留出大量空白，像随手画在本子上

## Prompt 编译器(五段式)

只写能变成像素的指令：

1. **风格定位**：`observational pen wash, minimalist pen and ink sketch with transparent watercolor washes, travel journal sketchbook style, hand-drawn imperfect lines`
2. **线稿锚**：`keep the [核心轮廓] recognizable, rendered in minimal broken pen lines, only key outlines and structural lines, no detailed rendering, sketchy hand-drawn quality`
3. **淡彩世界**：`only 1-2 areas with transparent watercolor washes of [主色], soft bleeding edges, color溢出线条, 70% of the canvas left as white paper, color only on the main subject`
4. **手记细节**：`textured cream sketchbook paper background, lines that fade out at the edges, a tiny handwritten date or location note in the corner, unfinished sketch feeling, off-center composition`
5. **约束**：`no continuous clean lines, no full color coverage, no photorealistic details, no dark heavy tones, no Chinese text, no watermark`

## 纠偏(最多重生成一次，只修观察到的失败)

- **线条太干净/像矢量图** → 加 `broken sketchy lines, hand-drawn imperfect strokes, wobbly uneven lines, pen sketch quality, not vector clean lines, overlapping sketch lines`
- **颜色太多/太平涂** → 加 `minimal watercolor only, sparse color washes, 70% white space, transparent thin washes, no flat color, no full coverage, color only in small areas`
- **太完整/没有手记感** → 加 `unfinished sketch, lines fading into white space, cropped composition, sketchbook page feel, partial drawing, not a complete illustration, travel journal aesthetic`
- **没有纸张质感** → 加 `textured cream paper background, old sketchbook paper, slight paper grain, off-white warm paper, not pure white digital background`
- **细节太多/不够极简** → 加 `extremely minimal lines, only key outlines, no interior details, suggestion rather than detail, sparse linework, lots of implied space`

## 硬禁忌

连续干净的矢量线条；满版颜色覆盖；照片级真实细节；纯黑线条和阴影；高饱和鲜艳颜色；居中对称构图；没有留白；中文文字；水印。

## 质量门(交付前逐项过)

- 线条有手绘的断续、轻重、不完美？
- 只画了最关键的轮廓，没有过多细节？
- 颜色只在1-3个区域少量晕染，70%以上留白？
- 有私人旅行手记的感觉？
- 背景是有纹理的纸张，不是纯白？
- 主体偏置，有大量呼吸空间？
- 没有干净矢量线条和满版颜色？

## 输出格式

默认只返回：生成的图 + 1–3 句创作思路(说清线稿选择和淡彩重点，不暴露完整 prompt)。用户明确要求时才附 prompt。

## 关联

本 skill 是旅行照片转绘系列之一。需要水彩旅行卡见 `watercolor-travel-card` skill；需要像素消隐景观见 `pixel-dissolve-landscape` skill；需要厚涂微缩景观见 `impasto-miniature-landscape` skill。
