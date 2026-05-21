# Seedance 2.0 九大商用玩法 / Nine Commercial Use-Cases

来源 / Source: 卡尔的AI沃茨 — [微信文章](https://mp.weixin.qq.com/s/d2YgM-7vVMQaRP67MtZVdQ)

九种商业应用场景：追热点、商业广告、品牌宣传、穿搭变装、直播带货、动态海报、广告复刻、真人短剧、AI漫剧。Reference media attaches in the Seedance UI as `@图片N` / `@视频N` / `@音频N`.

---

## 1. 追热点 / Chase Trends — 飞驰人生3同款

**技巧 / Technique:** 用不涉及真人版权的素材，把关键帧截取出来强调视频中关键的画面，做成同款效果。Use copyright-safe footage; key-frame the hero beat to emphasize it, then recreate the same effect.

**方法 / Method:**
1. 给一段同款视频 / supply a reference clip of the trend
2. 实拍一段关门视频 / shoot your own simple footage (e.g. a closing door)
3. 把关键帧截出来作为强调 / extract key frames as emphasis
4. 房间的门作为赛车在赛道上行驶 / map the metaphor (a door → a race car on the track)

---

## 2. 商业广告 / Product Ad — 运动饮料 / Sports Beverage

**提示词 / Prompt:**
```
为图中产品生成一个精美高级的运动饮料广告，注意分镜编排，明快的节奏和快剪，高级的商业广告。
```
EN: Generate a refined, high-end sports-beverage ad for the product in the image. Mind the storyboard editing, a brisk rhythm and fast cuts — a premium commercial.

**特点 / Notes:** Seedance 2.0 编排分镜出色；一次性产出配乐 + 文字 slogan；所有分镜对产品保持一致性。Strong storyboard sequencing, one-shot music + on-screen slogan, product consistency across all cuts.

---

## 3. 品牌宣传 / Brand Promo — 无印良品 / MUJI

**提示词 / Prompt:**
```
帮我生成一个讲述无印良品这个品牌的宣传片，中间植入这个台灯
```
EN: Generate a brand film about MUJI, with this desk lamp placed mid-film.

**特点 / Notes:** 直接给品牌名，它能按品牌调性写旁白；即使 5s 也呈现完整状态。Name the brand → on-tone VO; even a 5s clip reads complete.

---

## 4. 穿搭变装 / Outfit-Swap Showcase

**提示词 / Prompt:**
```
让一个女生依次换上@图1 @图2 @图3 @图4 @图5 @图6 六套服装进行卡点变装展示。每套服装需要包含半身走位和整体穿搭全身的展示。运镜要求使用不同景别流畅切换，加上符合调性的广告音乐
```
EN: Have one woman sequentially change into the 6 outfits in @图1…@图6 as a beat-synced transformation showcase. Each outfit shows a half-body walk and a full-body styling reveal. Smooth cuts across varied framings, plus on-tone ad music.

**特点 / Notes:** 完整呈现服装与包/鞋/袜等配饰，展现灵动。Renders every garment + accessories (bag, shoes, socks); lively delivery.

---

## 5. 直播带货 / Livestream Commerce — SK-II 面霜 / Face Cream

**提示词 / Prompt:**
```
生成一段 15 秒带货口播视频，产品为图中面霜。要求人物亲手涂手上，给出近景展示，侧脸转动展示细节，镜头从半身到特写切换 3 次。口播要包含卖点，最后给出强行动号召。自动生成字幕，节奏紧凑，带轻微环境音。
```
EN: Generate a 15s sell-script video; product = the cream in the image. The presenter applies it by hand, close-up demo, side-face turn for detail, 3 cuts from half-body to close-up. The script includes selling points and ends on a strong CTA. Auto subtitles, tight rhythm, light ambient sound.

**特点 / Notes:** 识别到产品是 SK-II，自动配上对应口播（高浓度 PITERA、五胜肽等成分），口播匹配画面。Auto-identifies the brand and writes matching ingredient copy synced to the visuals.

---

## 6. 动态海报 / Dynamic Poster

**提示词 / Prompt:**
```
一个15秒竖屏 9:16 的卡点音乐短片，背景音乐使用@音频1，视频全程保持固定机位景别不变，就像是在一个固定的位置定点拍摄一样，视频中的元素陆续按@图片1中的九宫格分镜依次显现，从左上角第一个镜头作为开始从左到右、从上到下依次推进。
```
EN: A 15s vertical 9:16 beat-synced clip, BGM = @音频1, fixed camera/framing throughout (as if shot from one locked position). Elements appear in sequence following the 3×3 grid of @图片1, starting top-left, left→right, top→bottom.

**流程 / Workflow:** ① 用 Nano Banana Pro 根据海报做出元素依次生成的九宫格分镜图 → ② 让 Seedance 2.0 按九宫格图做出元素依次展现。
① Build the 3×3 element-reveal grid in Nano Banana Pro → ② Seedance animates the ordered reveal.

**Tips:** 元素出现顺序把控可能不精准，在提示语中明确写出出现顺序。The model's ordering control is imperfect — spell out the appearance order explicitly.

---

## 7. 广告复刻 / Ad Remix — 无人机 / Drone

**提示词 / Prompt:**
```
模仿【@视频1】的分镜设计，把视频中所有产品都替换成【@图片1】的无人机，制作的视频完全是围绕【@图片1】的无人机进行多角度的展示，同时更换配音旁白和音乐为介绍无人机的内容，画面主要颜色使用蓝色和黑色
```
EN: Mimic the storyboard of @视频1, replace every product with the drone in @图片1, build the whole video around multi-angle shots of that drone, swap VO + music to drone-intro content, main palette blue and black.

**Tips:** 某个镜头替换效果不好时，先用 NanoBanana Pro 做出该分镜效果图，再让 Seedance 2.0 用它替换指定镜头。If a shot won't swap cleanly, render that frame in Nano Banana Pro first, then have Seedance replace that specific shot with it.

---

## 8. 真人短剧 / Celebrity Short-Drama — 豪门恩怨 / Dynasty Feud

**提示词 / Prompt:**
```
【风格】豪门恩怨、真假千金、极致反转、撕绿茶、高定礼服、美艳御姐

【角色】
真千金（烈焰红唇，黑天鹅高定礼裙，气场全开）
假千金（小白花扮相，泪眼装可怜）

【全局要求】
9:16 竖屏，电影质感，奢华宴会厅水晶灯与香槟塔，光影高级。真千金与假千金人物一致性稳定，脸不变，礼服不变。口型与字幕逐字完全一致，字幕即台词本身。每句台词控制在短句，清晰可读。

"[00:00-00:05] 奢华宴会厅中景，假千金故意撞翻桌边古董花瓶，清脆碎裂，她立刻坐地抱住碎片边缘假哭，抬手指向真千金，周围宾客围成半圈，纷纷侧目。口型与字幕：姐姐，你为什么这样"

"[00:05-00:10] 真千金近景，冷艳俯视，红唇微扬带嘲讽，抬手甩出一份文件砸到假千金面前。镜头切文件特写，画面只需要清晰看到大字 DNA 与红色印章 无血缘，不要密集小字。假千金抬眼，泪停住，脸色发白。口型与字幕：演够了吗"

"[00:10-00:15] 全场反应一瞬，宾客捂嘴惊呼，镜头立刻切回真千金。真千金走到主位旁，从假千金头上干脆取下皇冠，稳稳戴回自己头上，转身落座主位，抬眼扫全场。两名保安出现把假千金拖走，只给她被拖走的背影与无力挣扎。真千金定住女王姿态。口型与字幕：这是我家，滚"
```
EN structure: 【Style】dynasty feud, real-vs-fake heiress, extreme reversal, high-couture gowns. 【Characters】locked identities. 【Global】9:16, cinematic, crystal-chandelier ballroom, character consistency (face + gown unchanged), subtitle = exact spoken line, short clauses. Three time-coded beats with word-exact lip-sync.

**特点 / Notes:** 精准抓短剧节奏与分镜，人物一致性稳定。Nails drama pacing and storyboard; stable character identity.

---

## 9. AI漫剧 / AI Manga — 武侠 / Wuxia

**提示词 / Prompt:**
```
帮我根据下面的小说剧情要求生成动漫，将画风动作打斗表现严格对齐@视频1 的风格。

老者身形如鹤，袖袍一抖便卷起劲风，逼得年轻剑客连退三步。后者骤然低喝，剑尖挽出七朵虚影，正是"七星照月"的杀招。老者却似早有所料，枯瘦五指如鹰爪扣住剑身，内力一震——长剑寸寸崩断！年轻人弃剑疾退，反手抽出腰间软鞭，鞭梢如毒蛇吐信直取老者双目
```
EN: Generate anime from the novel passage below, strictly matching the art-style and fight choreography of @视频1. (Wuxia duel: an elder whose sleeve conjures wind forces a young swordsman back; the youth's blade spins seven phantom images — "Seven Stars Facing the Moon"; the elder claws the blade and shatters it with internal force; the youth draws a soft whip striking like a snake at the elder's eyes.)

**特点 / Notes:** 给一段画风视频/图片参考，直接产出对应风格动漫。Feed a style-reference clip/image → outputs anime in that style.

---

## 总结 / Takeaways

- 给一段参考或较详细的提示语，能实现七八成；中间不行的地方给更多参考画面；提示语写详细。A good reference + detailed prompt gets ~70–80%; feed more reference frames where a beat fails.
- **痛点 / Pain points:** 排队时间长（高峰 2 小时起）；凌晨较快（约十几分钟一个视频）。Long queues at peak (2h+); late night is faster (~10+ min per video).
