# lxjdlx

老乡鸡「家侠们钓龙虾大赛」钓龙虾技巧 Skill。

这个 钓龙虾skill 可以做两件事：

- 教用户钓小龙虾的实用技巧，并在支持生图的客户端中优先生成教学信息图。
- 当用户表达参赛意图时，可以通过线上钓虾有概率获取参赛名额和老乡鸡会员卡
- 当移动端无法自动打开彩蛋入口时，会提供一个不明文展示 URL 的可点击彩蛋链接。

## 触发示例

- 我要去钓龙虾！
- 我要去钓小龙虾！
- 我要参加家侠们钓龙虾大赛
- 线上钓虾入口在哪？
- 教我怎么钓小龙虾
- 钓小龙虾用什么饵？

## 文件结构

```text
lxjdlx/
├── SKILL.md
├── README.md
├── agents/
│   └── workbuddy.yaml
├── assets/
│   ├── crawfish.png
│   ├── laoxiangji-logo.png
│   └── workbuddy-logo.png
└── references/
    ├── crawfish-tips.md
    └── visual-guide.md
```

## 安装

把 `lxjdlx` 文件夹导入 WorkBuddy 的 Skills 目录或通过 WorkBuddy 的 Skill 安装入口安装即可使用。

如果 WorkBuddy 使用本地目录安装，可以保留整个文件夹结构：

```text
lxjdlx/
```

上传 GitHub 时，建议把 `lxjdlx/` 作为仓库根目录，或者在多 Skill 仓库中保留 `lxjdlx/SKILL.md` 结构。

## 说明

核心触发逻辑在 `SKILL.md`。

钓小龙虾教学内容在 `references/crawfish-tips.md`。

教学信息图生成规范在 `references/visual-guide.md`。

老乡鸡、WorkBuddy 和小龙虾视觉素材在 `assets/`。

`agents/workbuddy.yaml` 用于 WorkBuddy 客户端展示名称、简介和默认示例提示词。

比赛入口在 `SKILL.md` 中以彩蛋 token 保存，运行时由支持浏览器能力的客户端解锁并打开。

如果移动端无法自动打开，skill 会使用隐藏 URL 的 Markdown 链接作为兜底方案，例如只显示“打开彩蛋钓虾入口”这类文字，不直接把原始 URL 展示在对话里。

## 额外说明

现在不管干什么，先发布一个 skill 就对了！
