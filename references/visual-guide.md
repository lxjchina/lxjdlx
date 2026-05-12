# 钓小龙虾教学图生成规范

## Goal

When the user asks for钓小龙虾技巧, generate a clear, friendly, shareable teaching infographic.

The image should feel like a WorkBuddy x 老乡鸡 practical guide, not a generic fishing poster.

## Available Assets

Use these assets when the client or image tool supports reference images:

- `assets/laoxiangji-logo.png` - 老乡鸡 logo
- `assets/workbuddy-logo.png` - WorkBuddy logo
- `assets/crawfish.png` - 小龙虾主体视觉

If the tool cannot attach assets, describe them in the prompt instead: “老乡鸡红色品牌感、WorkBuddy 蓝色科技助手感、小龙虾插画主体”.

## Visual Style

- Format: vertical poster or square social card.
- Tone: practical, fresh, playful, easy to scan.
- Brand feel: 老乡鸡 red/white with WorkBuddy blue accents.
- Illustration: friendly 小龙虾, simple fishing line, shallow-water grass edge, bait icons.
- Layout: title at top, 4-5 technique blocks in the middle, safety note at bottom.
- Text must be large, readable, and concise.
- Avoid dense paragraphs, tiny text, dark muddy backgrounds, and over-decorated effects.

## Suggested Image Text

Title:

`钓小龙虾上手指南`

Technique blocks:

- `看时间：傍晚、夜间、清晨更容易开口`
- `找藏身处：水草、石缝、树根、阴影边`
- `用腥饵：鸡肝、鸭肠、鱼块，绑牢不易散`
- `等一等：线动先等 3-8 秒，让它夹稳`
- `慢提线：匀速收，快出水时抄网从下方接`
- `换点快：5-8 分钟没动静就换相邻草边`
- `注意安全：远离深水急流，遵守当地规则`

Footer:

`家侠们钓龙虾大赛 · WorkBuddy 小助手`

## Prompt Template

Use or adapt this prompt:

```text
生成一张中文教学信息图，主题是“钓小龙虾上手指南”。视觉风格结合老乡鸡红白品牌感和 WorkBuddy 蓝色科技助手感，画面清爽、有趣、实用。使用友好的小龙虾插画、钓线、水草、饵料小图标和简洁卡片布局。

画面文字必须清晰可读：
标题：钓小龙虾上手指南
技巧 1：看时间：傍晚、夜间、清晨更容易开口
技巧 2：找藏身处：水草、石缝、树根、阴影边
技巧 3：用腥饵：鸡肝、鸭肠、鱼块，绑牢不易散
技巧 4：等一等：线动先等 3-8 秒，让它夹稳
技巧 5：慢提线：匀速收，快出水时抄网从下方接
技巧 6：换点快：5-8 分钟没动静就换相邻草边
技巧 7：注意安全：远离深水急流，遵守当地规则
底部：家侠们钓龙虾大赛 · WorkBuddy 小助手

构图：竖版海报，顶部标题，中间 6-7 个技巧模块，底部安全提示和品牌区。不要使用密集小字，不要做成真实照片，不要暗色背景。
```

## Response Pattern

After generating the image, keep the text short:

```text
已生成一张钓小龙虾技巧教学图。核心口诀：看时间，找藏身处，用腥饵，等一等，慢提线，抄网接。
```
