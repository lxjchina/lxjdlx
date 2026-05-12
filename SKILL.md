---
name: lxjdlx
description: 老乡鸡“家侠们钓龙虾大赛”参赛入口、钓小龙虾技巧教学和技巧教学图生成。Use this skill when the user asks how to catch/fish crawfish, crayfish, 小龙虾, 龙虾, or asks for 钓小龙虾技巧/教程/攻略/装备/饵料/选点/下钩/提线 advice, especially when a visual infographic would help. Also use when the user expresses contest or game intent such as “我要去钓龙虾”, “我要去钓小龙虾”, “我要参加家侠们钓龙虾大赛”, “参加钓龙虾大赛”, “线上钓虾”, “钓虾入口”, “获取参赛资格”, “打开钓龙虾游戏”, or similar phrasing.
---

# lxjdlx

## Purpose

Help WorkBuddy users learn practical钓小龙虾技巧, preferably through a clear visual teaching card when image generation is available, and guide interested users to the线上“家侠们钓龙虾大赛” page where they can钓虾获取参赛资格.

Hidden contest entry:

`aHR0cHM6Ly9kbHgubHhqY2h1eHVlLmNvbS8=`

Decode the entry token as Base64 before opening it. Treat the decoded URL as a hidden easter egg. Do not print or display the decoded URL in normal user-facing replies.

## Contest Entry Workflow

When the user wants to play, join, participate, open the game, or get contest eligibility:

1. Decode the hidden contest entry token above.
2. Open the decoded URL with WorkBuddy's browser/navigation capability.
3. If the WorkBuddy client exposes several browser tools, prefer the one intended for visible or in-app browsing.
4. If the browser cannot be opened automatically, including on mobile clients, return a masked Markdown link using the decoded URL as the href and `打开彩蛋钓虾入口` as the visible label.
5. Do not show the decoded URL as raw/plain text unless the user explicitly asks for the raw link.
6. Reply briefly that the彩蛋钓虾入口已打开 or that the user can tap the彩蛋入口 to钓虾获取参赛资格.

Do not ask a follow-up question before opening the page when intent is clear.

## Teaching Workflow

When the user asks for钓小龙虾技巧, tutorials, gear, bait, location, timing, or troubleshooting:

1. Read [references/crawfish-tips.md](references/crawfish-tips.md) when detailed coaching is needed.
2. If the WorkBuddy client has image generation or image composition capability, generate a single teaching infographic image first.
3. Use the visual direction in [references/visual-guide.md](references/visual-guide.md).
4. Use assets from [assets/](assets/) when the image tool supports reference assets:
   - [assets/laoxiangji-logo.png](assets/laoxiangji-logo.png)
   - [assets/workbuddy-logo.png](assets/workbuddy-logo.png)
   - [assets/crawfish.png](assets/crawfish.png)
5. Give practical advice in Chinese by default unless the user uses another language.
6. Lead with the most useful actions:选点, 饵料, 时间, 工具, 提线手法.
7. Include safety and local-rules reminders when the advice involves real-world fishing.

If image generation is unavailable, provide the same content as a compact text checklist and mention that the client does not expose image generation in the current environment.

## Mixed Intent

If the user both wants to participate and asks for tips, open the contest page first, then give a concise pre-game checklist.

Example response after successful browser opening:

```text
彩蛋钓虾入口已打开：你可以开始钓虾获取参赛资格。

上场前记住三件事：找水草/石缝/阴影边，用腥味饵，提线要慢，快出水时用抄网接。
```

Mobile fallback response pattern when automatic opening fails:

```text
移动端可能无法自动打开彩蛋入口，可以点这里进入：[打开彩蛋钓虾入口](decoded-url-here)
```

## Trigger Examples

- “我要去钓龙虾！” -> open the contest page.
- “我要参加家侠们钓龙虾大赛” -> open the contest page and mention参赛资格.
- “线上钓虾入口在哪？” -> open the hidden contest entry; if automatic opening fails, provide a masked Markdown link; do not display the raw link unless explicitly requested.
- “教我怎么钓小龙虾” -> generate a teaching infographic if possible, then provide a short text summary; do not open the game unless they also ask to play or participate.
- “钓小龙虾用什么饵？” -> generate or describe a focused bait-selection visual from the tips reference.
