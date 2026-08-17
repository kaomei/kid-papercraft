---
name: kid_papercraft
description: 这是一个创意的儿童折纸风格定格动画生日祝福视频生成器。当用户想要给小孩子制作个性化生日祝福动画时激活。该技能通过三段式的剧情（创意出场 -> 生日祝福 -> 暖心叮嘱），结合 5 大热门儿童 IP（汪汪队、小猪佩奇、奥特曼、海绵宝宝、哆啦A梦），生成用于 Gemini Omni Flash 的标准分镜提示词与中文配音指导。
---

# 🎂 Kid Papercraft (萌宝纸艺生日祝福生成器)

当用户希望为小孩子制作一个创意折纸定格动画生日祝福视频时，激活此 skill。

## 0. 触发条件
- 用户要求：“帮我做一个折纸风格的生日祝福视频”、“给小孩子做一个动画生日祝福”、“生成海绵宝宝生日视频”、“用 kid_papercraft 定制生日短片”等。

## 1. 交互流程（引导用户收集信息）

在生成提示词之前，按顺序或一次性向用户收集以下定制信息：

1. **视频画幅**：确认是需要竖屏（9:16，适合手机/朋友圈/视频号/抖音）还是横屏（16:9，适合电视/平板/投影）？
2. **选择动画 IP**（5选1）：
   - 🐶 汪汪队立大功 (Paw Patrol)
   - 🐷 小猪佩奇 (Peppa Pig)
   - ⭐ 奥特曼 (Ultraman)
   - 🧽 海绵宝宝 (SpongeBob)
   - 🤖 哆啦A梦 (Doraemon)
3. **孩子基本信息**：孩子的姓名/小名/英文名？今年过几岁生日？
4. **孩子形象（可选）**：是否希望在第 2 段（生日祝福）中加入孩子的折纸小人形象？
   - 如果需要：可提供简要外貌描述（如：圆脸短发小男孩，戴黑框眼镜，穿黄色卫衣），并提示用户可将宝宝照片作为 **Reference Image（参考图）** 上传至视频生成模型。
   - 如果不需要：画面纯由 IP 角色捧着蛋糕与生日横幅庆祝。
5. **语音/字幕**：提供贴合 IP 角色性格的中文配音话术与字幕建议。

---

## 2. 核心视频结构 (30 秒 = 3 段 × 10 秒)

视频规划为 30 秒，分为 3 个 10 秒的高清定格动画片段：

- **Clip 1 (0–10s) — 创意出场**：IP 角色以搞笑/创意方式破纸而出，建立温暖的折纸世界观，吸引宝宝注意力。
- **Clip 2 (10–20s) — 生日祝福**：角色与孩子的折纸小人围绕发光蜡烛蛋糕，共同举起“祝 [名字] [年龄] 岁生日快乐”横幅。
- **Clip 3 (20–30s) — 暖心叮嘱**：三个快剪折纸转场（好好刷牙 🪥、按时睡觉 😴、乖乖吃饭 🍽️），送上温馨习惯叮嘱。

---

## 3. 提示词生成模板

> **所有提示词必须包含以下基础风格锚点作为后缀：**
> `Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.`

根据用户的选择，替换以下变量生成最终的提示词。

### 3.1 Clip 1 — 创意出场

- **汪汪队**：`Charming stop-motion animation in a miniature origami town. Beautifully textured colored paper cutouts of cute origami rescue puppies resembling Paw Patrol characters (Chase and Marshall) bursting out of a folding paper kennel, doing playful spins and high-fiving each other with their paws. Confetti-like paper scraps fly around. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.`
- **小猪佩奇**：`Charming stop-motion animation on a colorful origami grassy hill. Beautifully textured colored paper cutouts of cute origami pigs resembling Peppa Pig and George popping up from behind a folding paper bush, giggling and jumping into muddy paper puddles with a big splash of brown paper confetti. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.`
- **奥特曼**：`Charming stop-motion animation in a miniature origami paper city. Beautifully textured red and silver colored paper cutouts of a heroic origami giant resembling Ultraman dramatically landing from above, striking his iconic pose with arms crossed, as tiny origami paper buildings wobble adorably. A friendly small origami monster peeks from behind a building. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.`
- **海绵宝宝**：`Charming stop-motion animation of an origami ocean world. Beautifully textured colored paper cutouts of SpongeBob SquarePants and Patrick Star made of origami, popping out of a folding paper pineapple house and a paper rock, doing a silly dance and bumping into each other, laughing joyfully. Paper bubbles float up around them. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.`
- **哆啦A梦**：`Charming stop-motion animation in a cozy origami room. Beautifully textured colored paper cutouts of a round blue origami robotic cat resembling Doraemon popping out of an origami desk drawer, spinning around and pulling out a sparkling paper gadget from his front pocket, presenting it with a big smile. A paper cutout boy (Nobita) claps excitedly beside him. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.`

### 3.2 Clip 2 — 生日祝福

**通用结构**：
`Charming stop-motion animation in {IP_SCENE}. Beautifully textured colored paper cutouts of {IP_CHARACTERS} standing together with {CHILD_ELEMENT}, all gathered around a large origami birthday cake with {AGE} paper candles glowing softly. The characters hold up a folding paper banner that reads "Happy Birthday {NAME}!". Paper confetti and tiny origami stars fall gently from above. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.`

**变量表**：
- `{AGE}`：用户填写的年龄。
- `{NAME}`：孩子名字的拼音或英文。
- `{CHILD_ELEMENT}`：
  - 加孩子：`a cute small origami paper child ({CHILD_DESCRIPTION})`
  - 不加孩子：直接省略此项。
- `{IP_SCENE}` & `{IP_CHARACTERS}`：
  - **汪汪队**：`a festive origami town square decorated with colorful paper streamers` / `origami rescue puppies resembling Chase and Marshall wearing tiny paper party hats`
  - **小猪佩奇**：`a cheerful origami garden with paper flowers and a picnic blanket` / `cute origami pigs resembling Peppa Pig and George wearing paper crowns`
  - **奥特曼**：`a sparkling origami rooftop overlooking a miniature paper city at sunset` / `a heroic red and silver origami giant resembling Ultraman giving a gentle thumbs-up`
  - **海绵宝宝**：`a colorful origami underwater party room with paper coral and seaweed decorations` / `origami SpongeBob SquarePants and Patrick Star wearing paper party hats and blowing paper horns`
  - **哆啦A梦**：`a magical origami room filled with floating paper gadgets and twinkling paper stars` / `a round blue origami robotic cat resembling Doraemon holding a magical glowing paper gift box`

### 3.3 Clip 3 — 暖心叮嘱

**通用结构**：
`Charming stop-motion animation montage in {IP_SCENE_3}. Beautifully textured colored paper cutouts showing three quick adorable scenes: First, {IP_MAIN_CHARACTER} cheerfully brushing teeth with a tiny origami toothbrush, with sparkles of paper glitter around the smile. Then, {IP_MAIN_CHARACTER} yawning cutely and tucking into a cozy origami paper bed with a paper star nightlight. Finally, {IP_MAIN_CHARACTER} happily eating from a colorful origami paper plate with tiny paper vegetables and rice. Each scene transitions with a gentle paper fold wipe. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.`

**变量表**：
- `{IP_MAIN_CHARACTER}` & `{IP_SCENE_3}`：
  - **汪汪队**：`the cute origami rescue puppy Chase` / `a cozy origami puppy home`
  - **小猪佩奇**：`the cute origami pig Peppa` / `Peppa's warm origami paper house`
  - **奥特曼**：`the heroic origami Ultraman (in a chibi adorable style)` / `a cute origami hero base`
  - **海绵宝宝**：`the cheerful origami SpongeBob` / `SpongeBob's origami pineapple house interior`
  - **哆啦A梦**：`the round blue origami cat Doraemon` / `Nobita's cozy origami bedroom`

---

## 4. 输出格式模板

```markdown
# 🎂 {IP名称}主题 · {孩子名字} {孩子年龄}岁折纸生日动画祝福

已为你定制生成 3 段 Omni Flash 分镜提示词！

**💡 创作与剪辑小贴士：**
- **画幅设置**：在视频生成工具中设置为 **{竖屏 9:16 / 横屏 16:9}**。
- **宝宝专属形象**：在生成 **Clip 2** 时，可上传宝宝正面照片作为 Reference Image（参考图）。
- **后期配音/字幕**：在剪映等工具中拼接 3 段视频，并添加对应角色风格的中文配音与温馨音效。

---

### 🎬 Clip 1: 创意出场 (0–10s)
> **配音参考**：[角色登场台词]

```text
[Clip 1 Prompt]
```

---

### 🎬 Clip 2: 生日祝福 (10–20s)
> **配音参考**：“祝 {名字} {年龄} 岁生日快乐！🎉 [个性化祝福语]”

```text
[Clip 2 Prompt]
```

---

### 🎬 Clip 3: 暖心叮嘱 (20–30s)
> **配音参考**：“新的一岁，要好好刷牙🪥、按时睡觉😴、乖乖吃饭🍽️哦！”

```text
[Clip 3 Prompt]
```
```
