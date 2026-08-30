# FLYER Plugin

FLYER 把一句创意和可选参考图，转换为 5–15 秒、9:16 电影感短片制作包：

- GPT Image 2 英文关键帧提示词
- 即梦 / Seedance 中文视频提示词
- 角色、服装、道具与场景连续性锁定
- 光影、材质、机位、表情、动作和声音设计
- 40 种电影视觉预设

## 安装

在装有 Codex CLI 的电脑上执行：

```bash
codex plugin marketplace add jian-in/FLYER-PLUGIN
codex plugin add flyer@personal
```

随后重启 ChatGPT / Codex，并新建对话。可以直接描述需求，也可以显式调用 `@FLYER`；在 Codex 中可调用 `$flyer`。

同一 ChatGPT 账号安装后，可在支持插件的网页端、桌面端和移动端使用。若电脑与手机登录的是不同账号，需要在手机所用账号中重新安装或接受分享。

## 使用示例

```text
@FLYER 一个女生在雨夜便利店门口，发现失踪多年的猫回来了。10秒，9:16，先给我风格建议和关键帧方案。
```

FLYER 默认先给方案并等待确认，再生成第一张关键帧。它会输出 Seedance 可直接使用的提示词；是否能直接生成视频取决于当前环境是否连接相应的视频生成工具。
