# Seedance Video Prompt Workflow

Use this reference after the keyframe and continuity locks are approved. Write the final Seedance prompt in Chinese.

## Default Strategy

FLYER is keyframe-first:

1. Bind the approved character or hero frame as the identity and look reference.
2. Bind wardrobe, location, motion, or sound references by role when supplied.
3. Use the smallest number of shots needed for the visible event.
4. Preserve one global identity, wardrobe, scene, palette, and light-direction block.
5. Describe each beat as an observable physical change with a beginning, peak, and settling state.

Do not claim a feature or reference-binding syntax that the active Seedance interface does not expose. If direct reference mentions are unavailable, provide a plain reference-binding list for the user to apply manually.

## Shot Count

- One story beat: prefer one continuous shot.
- One clear reversal or point-of-view change: one continuous shot with a reveal, or two shots if the cut improves clarity.
- Several independent events: reduce or prioritize. A 5–15 second clip should not become a compressed trailer by default.
- Use a cut only for a change in time, place, viewpoint, or information.

## Prompt Order

Write one copyable block using this order:

1. 视频规格与全局风格锁
2. 参考素材绑定
3. 主角与场景不可变项
4. 按时间或镜头描述可见动作
5. 运镜、构图与调度
6. 光影、材质与环境反应
7. 声音：环境声、动作声、呼吸、对白、配乐
8. 结尾停驻状态
9. 约束与避免项

## Action Design

- Use physical verbs and visible state changes.
- State who initiates the action, what they touch, the direction of movement, and where weight lands.
- Keep hands purposeful and in contact with objects when required.
- Preserve gravity, inertia, cloth response, water, dust, smoke, and prop motion.
- Leave enough time after the peak for the image to settle.
- If dialogue is used, quote the exact short line and identify the speaker and delivery.

Avoid abstract instructions such as “气场全开,” “情绪拉满,” or “震撼登场” unless translated into visible performance and physical effects.

## Camera Design

- Give each beat one main camera behavior.
- State shot size, camera height, angle, subject relation, travel direction, and stopping point.
- Prefer subject-led tracking, a restrained push, a lateral reveal, a stable observational frame, or gentle handheld drift when they serve the beat.
- Avoid stacking orbit, zoom, crane, whip pan, shake, and focus pull in one short beat.
- Preserve screen direction and eyelines across cuts.

## Sound Design

Design sound from the story.

- Environment: room tone, rain on material, traffic distance, wind through architecture, insects, crowd wash.
- Foley: fabric friction, shoe contact, hand on prop, metal resonance, water displacement, breath.
- Dialogue: exact words, speaker, distance, emotion, and whether on-screen.
- Music: use only when it adds rhythm, period, or narrative meaning. Default to restraint.
- Silence: explicitly retain room tone when silence is part of the tension.

Do not add a generic rising score to every emotional ending.

## Chinese Template

视频规格：9:16竖屏，时长[秒数]。画面目标为[题材和视觉方向]，保持克制、真实的材质反应与统一色彩逻辑。

参考绑定：
- 参考1：[身份/服装/场景/运动/声音用途]
- 参考2：[用途]

全局不可变项：
- 主角：[精确角色与服装锁]
- 场景：[空间、时间、天气、固定道具、光源方向]
- 视觉：[主预设、辅助预设、色彩、对比、纹理]

时间轴与可见动作：
- 0.0–[x]秒：[起始姿态、视线、身体重心、环境状态、镜头初始位置]
- [x]–[y]秒：[动作发起、接触、运动方向、表情变化、镜头关系]
- [y]–[结束]秒：[动作峰值后的回落、最终视线、身体和道具停驻状态]

运镜与构图：[景别、机位高度、角度、透视感、唯一主运镜、纵深、负空间和竖屏安全区]

光影与材质：[有来源的光、方向、软硬、反差、曝光；皮肤、织物、金属、木材、雨雾或尘埃的差异反应]

声音：[环境声]；[动作声]；[呼吸或对白]；[配乐策略或明确无配乐]

严格保持：[身份、服装、道具、场景、光向和动作连续性]
避免：[针对该镜头的4–6个高风险错误]

## Continuity Compression

Repeat a short invariant line in every shot, even when a global block exists:

“同一主角、同一五官与脸型、同一发型和服装结构、同一道具状态、同一光源方向与色彩基线。”

Customize it to the actual lock; do not leave it generic.

## Ending Rule

The last moment must be readable:

- a gaze lands
- a hand releases or grips
- cloth and particles settle
- the camera stops
- the environment continues naturally

Do not introduce a new action, explosion, costume change, or camera move in the final instant unless the story specifically requires a cliffhanger.

## Repair

If a generation fails:

- identity drift: reduce motion complexity, strengthen the identity reference, and restate the exact lock
- warped hands or contact: simplify the action and specify grip/contact geometry
- cheap lighting: name the motivated source and remove unrelated rim or neon effects
- plastic materials: add surface-specific wear and reduce beauty language
- chaotic camera: keep one main move and a clear stopping point
- story unreadable: simplify to one visible cause-and-effect beat

