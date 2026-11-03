# FeelMuse

一个面向 Codex CLI 的网页创意设计 Skill。适合从一个模糊想法开始做官网，也适合只给已有页面增加一个动效。设计方向在终端里讨论，效果在浏览器里验收。

## 安装

首次安装（macOS / Linux）可执行以下命令。已有本仓库时，从仓库根目录执行最后两行即可。符号链接跟随仓库更新；如目标位置已有同名 Skill，请先检查现有安装。

```sh
git clone https://github.com/TeresaPeng-zju/FeelMuse.git
cd FeelMuse
mkdir -p "$HOME/.agents/skills"
ln -s "$PWD/skills/feelmuse" "$HOME/.agents/skills/feelmuse"
```

如果只给单个项目使用，将仓库中的 `skills/feelmuse` 文件夹复制到目标项目的 `.agents/skills/` 下。在该项目打开 Codex CLI；若当前会话没有发现 Skill，重新启动 Codex。可输入 `$feelmuse` 显式调用，也可直接描述网页设计需求。详见 [Codex 官方 Skill 说明](https://developers.openai.com/codex/skills)。

## 怎么用

- “$feelmuse 我做了一个按地点听田野录音的档案，只有声音和地名。帮我想官网的第一屏。”
- “我喜欢第一个网站滚动时图层错速的效果，以及第二个网站的目录排版。用自己的作品设计版画工作室官网。” 接着贴两个网址。
- “保留现在的 3D 沙盘和相机，只让切换到月怒状态时多一圈短暂的脉冲。”
- “参考这个页面中段的固定滚动，先做一个能前后滚动的原型，我看过再接入官网。”

操作现站时请从目标项目启动 Codex，并给出本地入口或预览地址。FeelMuse 使用当前环境可用的浏览器和前端工具。没有浏览器时，视觉验收会标记为待验证。用户只要研究或方案时，会在该阶段交付。

[Skill 入口](skills/feelmuse/SKILL.md) · [何时需要用户决定](skills/feelmuse/references/interaction.md) · [四个验收场景](tests/acceptance.md)
