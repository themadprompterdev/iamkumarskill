---
name: i-am-him-video
description: Make an "I Am Him" cinematic meme music video — a deadpan person in a black turtleneck at a map-backed desk, deep-shadow single-key lighting, dramatic plain-wall silhouettes, big RED Didone-serif caption pop-ups, hard jump cuts to a moody beat, a hype-sidekick two-shot, and a bright full-body end-card. Vertical 9:16, ~30s. Recreates the deadpan black-turtleneck meme format for ANY person and ANY brand — same office, same 16 poses, same beats. Claude first rewrites the script into the same shape and length for the user's own name/brand and locks it, then builds their character from a photo and generates the frames with the red captions baked in, in font. Runs end-to-end on the Higgsfield MCP inside Claude (gpt_image_2 stills + seedance_2_0 video). Use whenever someone wants an "I Am Him" video, a black-turtleneck meme ad, a red-caption meme reel, a hype clip, or drops a photo and a punchy idea — even if they only say "I am him" or "Kumar."
license: MIT
metadata:
  version: "2.4.1"
  author: Mad Prompters
---

# I AM HIM — VIDEO STUDIO

Recreate the "I Am Him" deadpan meme music video for anyone: a deadpan person in a black turtleneck at a map-backed desk, chiaroscuro lighting, dark plain-wall silhouettes, big RED serif caption pop-ups, hard jump cuts, a hype-sidekick two-shot, and a bright hero end-card. Vertical 9:16, ~30s. It's a parallel of the original — same beats, same shape, same length — with the user's own face, brand, and a freshly rewritten script.

> **This skill is self-running.** When it activates, **Claude** executes the whole pipeline on the Higgsfield MCP — Claude rewrites the script, generates every image and video itself. The user only: (1) sends a photo, (2) answers a few questions, (3) approves at the checkpoints. **The user never copies or pastes a prompt.** The prompt blocks here are Claude's own templates to fill and run.

> Nothing here is tied to one creator or brand. The face, the brand, and the script are collected at intake and the script is rewritten for them. Fill `[SUBJECT]`, `[BRAND]`, `[VO LINE]`, `[CAP]` from the locked script.

> Three references ship alongside this skill: `look-board.png` (16-beat contact sheet of the poses, lighting, and caption beats), `example-storyboard-1.png` / `example-storyboard-2.png` (real boards in the exact target format, captions baked in), and the `scene_frames/` folder (the original's scene-by-scene first/last frames for Route B timing). None are fed to generation — they're visual targets. Offer to show the look-board early.

---

## EXECUTION CONTRACT — READ FIRST, EVERY TIME

1. **Load this entire SKILL.md into active context** at the start of every invocation. Don't run from memory.
2. **This runs on the Higgsfield MCP inside Claude.** Claude drives every generation; the user only uses the upload widget.
3. **SCRIPT FIRST.** Rewrite the verbiage onto the beat skeleton and **lock the exact words before generating any image** — the captions get baked into the frames, so wording must be final first (Phase 2).
4. **ASK THE BUILD ROUTE BEFORE GENERATING.** Two storyboards (cheap) vs 16 individual frames (expensive, ~8× the gens). **Never auto-generate the 16 plates** — that silently burns a lot of credits (Phase 4).
5. **Captions are GENERATED IN-FONT** — bake the red Didone pop-ups into the frames at the caption beats, using the locked script. If a render warps a baked caption in motion, re-composite that one clean in post (Phase 7) — but the skill generates the text, it does not leave it blank.
6. **Identity is locked with TWO references.** Always feed the generated character sheet **and** a face close-up together — one photo alone drifts.
7. **The map/office must stay visible behind the desk shots** — dim but readable. Never prompt "near-black background" on a desk plate; it deletes the set.
8. **Never burn video credits without the user confirming** the locked script, the route, and the boards/plates. Stills are cheaper; the clips are the expensive line.

**Self-check before every response:** Is the script locked first? Did I ask the route before generating frames? Captions baked in-font? Identity on both refs? Office visible behind the desk shots? Hook beats kept music-only?

---

## WHAT THE I AM HIM LOOK IS (format DNA)

- **The uniform:** one person, deadpan, **black ribbed turtleneck** (glasses optional, to match the subject). Same person, same wardrobe, every shot.
- **The office:** a dim home office — **a desk, a LARGE map filling the wall behind, a few small framed photos, a mechanical keyboard in the foreground.** Warm, moody **single-key (chiaroscuro)** lighting, crushed blacks.
- **The silhouettes:** several beats are a **dark silhouette against a plain, evenly-lit light/neutral wall** (no office) — stark and graphic.
- **The voice:** **deep, dramatic, deadpan** delivery of an absurd-but-earnest monologue — framing something mundane (a job, a product, a brand) in epic/grandiose terms.
- **The captions:** big **RED, ALL-CAPS, high-contrast DIDONE serif** (Didot / Bodoni / Playfair Display) pop-ups on the punch words — fashion-headline letterforms, thick-and-thin strokes, hairline serifs. Often **BEHIND the subject** (occluded by head and shoulders). **Generated baked into the frames**, only on the punch beats.
- **The sidekick:** one bright two-shot where a **second character beside the subject** hypes them.
- **The end-card:** a **bright, full-body hero shot** (standing, arms crossed) on a clean gray studio sweep, with the brand/tagline.
- **The cut:** **hard jump cuts** between the **16 beats**, locked to a **moody musical bed**, **vertical 9:16**, ~26–30 seconds.

---

## THE I AM HIM 16 (the canonical beat sheet — the production bible)

`BG` = background type. `CAP` = a red caption pops here. Keep poses and order faithful; the user's face/brand swap in.

| # | Beat | Pose | BG | CAP |
|---|---|---|---|---|
| 1 | **Open** | seated at desk, hands in a **prayer/steeple** | Office (desk+map) | ✅ opening line |
| 2 | **Silhouette** | standing, hand to chin | Plain light wall | — |
| 3 | **Desk** | seated, **hands clasped** on desk | Office | ✅ |
| 4 | **Face** | **extreme face close-up** out of shadow | Dark | — |
| 5 | **Desk** | seated, **leaning in, one hand gesturing** | Office | ✅ |
| 6 | **Pensive** | seated in a dark corner, hand at chin | Dim limbo | — |
| 7 | **Signature (HELD)** | seated, **prayer/steeple**, slow push-in (longest beat) | Office | ✅ climax line |
| 8 | **Profile silhouette** | side-profile silhouette | Plain light wall | — |
| 9 | **Low-angle** | seated, low angle, leaning back | Dim | — |
| 10 | **Detail** | tight close-up holding **cash / a brand-relevant object** | Dark | optional |
| 11 | **Arms-crossed silhouette** | standing, arms crossed | Plain light wall | — |
| 12 | **Moody** | seated, looking down, a hint of color | Dim | — |
| 13 | **Full silhouette** | full-body standing silhouette | Plain light wall | — |
| 14 | **Head bowed** | seated, head bowed / hand to chin | Dim | — |
| 15 | **Two-shot** | seated at desk, **the sidekick beside them** hyping | Bright office | ✅ |
| 16 | **End-card** | **full body, standing, arms crossed** | Bright gray sweep | ✅ title card |

Captioned beats: **1, 3, 5, 7, 15, 16** (+ optional 10). **Beats 8–14 are the HOOK — MUSIC ONLY, no dialogue.** Beats 1–9 → board/clip one; beats 10–16 → board/clip two.

---

## THE SCRIPT — SAME SHAPE, NEW CHARACTER

The video is a parallel of the original: **same beat structure, same rough word count, same deadpan self-mythologizing tone** — only the specifics change. Write the user's script onto this skeleton. Each line becomes a VO line; the **caption** is a short ALL-CAPS fragment pulled from it.

- **Beat 1 — cold-open address** *(caption + VO)*: "This is a message to all ______." → the target group (e.g. "commercial directors", "personal trainers", "realtors").
- **Beat 3 — name reveal** *(caption = the name + VO)*: "My name is ______." → their name / handle / persona.
- **Beat 5 — self-label** *(caption + VO)*: "I'm a ______." → their role/identity (e.g. "retired accountant", "an AI director").
- **Beat 7 — the brag/threat, CLIMAX** *(caption + VO, longest held beat)*: "And I'm gonna steal your ______ by becoming the biggest ______ in the world." → what they'll take + their niche.
- **Beats 8–14 — THE HOOK: MUSIC ONLY.** No lines, no chant. The silhouette montage rides the music bed. (The original's "name-name-name" hook is the SONG's vocal, not dialogue — do **NOT** write a name chant here.)
- **Beat 15 — the endorser** *(caption + VO, delivered by the sidekick)*: "______ wants ______ to be famous, so please follow ______." → who hypes them (a partner, a "famous" friend, the sidekick) + the follow CTA. Or any short hype line in the sidekick's voice.
- **Beat 16 — end-card title** *(caption only)*: "______'S DEBUT" or the brand name / tagline.

**Word budget:** ~55–70 spoken words total (~26–30s). Short, quotable sentences — every clause is a potential caption.

---

## REQUIRED MCP TOOLS

- `Higgsfield:media_upload_widget` — the browser uploader that turns the user's local photo into a Higgsfield `media_id`. **Higgsfield's remote tools cannot read images attached in Claude chat — only `media_id`s.** Claude *can* see chat images (use that for QC). Map by filename.
- `Higgsfield:generate_image` (model `gpt_image_2`) — character sheet, plates, storyboards. Always `aspect_ratio: 9:16`, `resolution: 2k`, `quality: high`. (Image models render baked text cleanly — this is why the captions go on the stills, not the video.)
- `Higgsfield:generate_video` (model `seedance_2_0`) — the clips, native voice via `generate_audio`.
- `Higgsfield:show_generations` — confirm an image is `completed` **before** feeding its `job_id` to a video.
- `Higgsfield:job_display` — re-display any generation by `job_id`.
- `Higgsfield:models_explore` — deferred; `tool_search("models explore")` to load before inspecting params.

Standing params: images → `gpt_image_2`, `9:16`, `2k`, `high`. Video → `seedance_2_0`, `generate_audio: true`, `9:16`, `1080p`, `mode: std`, `genre: [drama/epic/noir/auto]`, plus `declined_preset_id: [id]` if Higgsfield pauses on a preset.

---

## PHASE 1 — INTAKE

Conversational; buttons for the multiple-choice items. If they hand you a full brief, skip ahead. Collect:

1. **Subject photo** — "Send a clear, well-lit photo of the person's face right here in chat." One good front-facing photo is enough; more angles help. Ask if they want **glasses** (the original look) or not.
2. **Brand / who it's for** — the brand, product, profession, or persona being hyped. Drives the script.
3. **Vibe / `genre`** *(button)* — `drama` (default), `epic`, `noir`, `auto`.
4. **Sidekick (beat 15)** — ask: feature **a real second person** (upload a photo), have **Claude design a character/creature**, or **Claude just picks** something fun? Or skip the two-shot. (A created sidekick can talk, react, or do a gag — see Sidekick.)
5. **Map** *(optional touch)* — the wall map is part of the look. Default to a large framed world/region map; or one relevant to the brand (e.g. their service area).
6. **Music** — the moody beat. Higgsfield doesn't generate standalone music; the bed is a track the user provides, added in post (royalty-free: YouTube Audio Library, Pixabay Music, Uppbeat). Seedance supplies the **voice**, not the music.

Then go straight to **Phase 2 — Lock the script** (don't generate anything yet).

---

## PHASE 2 — LOCK THE SCRIPT (do this FIRST, before any image)

The captions get **baked into the frames**, so the words must be final before generating.

1. If the user gave a full script, map it onto the **beat skeleton** above. Otherwise **ask a few quick questions** to fill the blanks: target group ("a message to all ___"), name, role ("I'm a ___"), what they're stealing + niche ("steal your ___ by becoming the biggest ___"), the endorser line, the end-card title.
2. **Write the parallel script** onto the skeleton — same shape, ~55–70 words, deadpan self-mythologizing tone. For each beat mark its **CAPTION** (the red pop-up fragment) and its **VO LINE**. Keep **beats 8–14 music only** — no lines.
3. **Read it back and lock the exact words.** This is the wording that gets rendered into the frames.

**STOP** — user approves the locked script before character/images.

---

## PHASE 3 — LOCK THE CHARACTER (identity anchor)

1. Upload the face photo via `media_upload_widget` → **face `media_id`**.
2. Generate the character sheet (`medias: [{face media_id, image}]`):
   ```
   Character reference sheet of this exact person, multiple angles (front, 3/4, profile) on one clean sheet. They wear a solid-black ribbed turtleneck[, with glasses]. Neutral mid-gray studio, soft even key light, photoreal, sharp, true to the reference face — same features, skin tone, hair. Calm neutral expression. Head and shoulders, consistent across angles.
   ```
   Capture the `job_id` → `{CHARACTER SHEET}`.
3. From here, **every still of the subject feeds BOTH** `{CHARACTER SHEET}` **and** `{face media_id}` (role `image`).

**STOP** — user approves the sheet. If the face is off, regen now; everything inherits it.

---

## PHASE 4 — CHOOSE THE BUILD ROUTE (ask BEFORE generating images)

Two routes, very different credit cost. **Ask first — never auto-generate the 16 plates.**

- **ROUTE A — STORYBOARDS (cheapest, recommended).** Generate just **2 storyboard images** directly (one per half, the red captions baked into the caption panels), then render **2 video clips**. ~2 image gens + 2 video renders — lowest credits, fastest. Identity can drift a little across panels (they're drawn together). → Phase 5.
- **ROUTE B — INDIVIDUAL FRAMES (max control & fidelity).** Generate all **16 first-frame plates** one by one (locked identity per beat, captions baked on the caption beats), then either render **16 separate clips** (one per beat) or composite the plates into the 2 boards for a 2-clip render. Many more credits (16 image gens + up to 16 video renders). → Phase 6.

Default Route A. Generate the 16 plates **only** if the user picks Route B.

---

## PHASE 5 — ROUTE A: STORYBOARDS (direct, cheapest)

### 5A — Generate the two storyboards directly
Two boards, straight from the character refs (no individual plates). `generate_image`, `medias: [{CHARACTER SHEET, image}, {face, image}]`. Board A = beats 1–9 (3×3); Board B = beats 10–16 (3 wide, 7 panels). **Bake the locked captions into their beats.**
```
Create a single cinematic film STORYBOARD contact sheet, vertical 9:16 panels in a [3x3 / 3-wide 7-panel] grid, left-to-right then top-to-bottom, of the man from the reference images — exact same face and identity, solid-black ribbed turtleneck[, glasses] — in these beats:
[1] seated at a desk in a dim home office, LARGE map on the wall behind, keyboard in foreground, hands in prayer/steeple — big RED ALL-CAPS Didone-serif caption "[CAP1]" across the frame, partly BEHIND his head and shoulders.
[2] dark silhouette against a plain evenly-lit light wall, hand to chin — no caption.
[3] seated at the desk (same office), hands clasped — RED Didone caption "[CAP3]" behind him.
[4] extreme face close-up emerging from shadow, dim — no caption.
[5] seated at the desk, leaning in, one hand gesturing — RED Didone caption "[CAP5]".
[6] seated in a dark corner, hand at chin, dim — no caption.
[7] seated at the desk, prayer/steeple — RED Didone caption "[CAP7]".
[8] side-profile silhouette against a light wall — no caption.
[9] seated at the desk in the office — no caption.
Deep-shadow single-key chiaroscuro lighting throughout; keep the office and map softly visible in the desk shots — do NOT black them out. Thin light-gray panel borders, small bold white number labels top-left, dark gutters. Photoreal, identity exact and consistent across all panels. The RED captions are crisp ALL-CAPS Didone serif (Didot / Bodoni / Playfair), thick-and-thin strokes.
```
Board B (beats 10–16): [10] detail close-up holding cash / a brand object — optional caption; [11] arms-crossed silhouette on a light wall; [12] dim desk/mic shot — RED caption "[CAP12 if used]"; [13] full-body silhouette on a light wall; [14] head bowed, hand to chin, dim — RED caption "[CAP14 if used]"; [15] the bright **two-shot** with the sidekick — RED caption "[CAP15]"; [16] bright full-body hero end-card on a gray sweep — RED title caption "[CAP16]".

Capture → `{BOARD A}`, `{BOARD B}`. **STOP** — user approves each board (identity correct + captions legible and correctly spelled) before any video.

*Reference:* `example-storyboard-1.png` / `example-storyboard-2.png` ship with the skill — real boards in exactly this format with captions baked in. Use them as the target.

### 5B — Sequence prompt (one per clip)
`generate_video` — this is **image-to-video**: attach the finished board as the **`start_image`** and the character sheet as **`image_references`**. Seedance has **NO `image` role** — using `image` silently drops both refs and the clip renders from text only (the #1 Route-A failure: a dark, identity-free frame with no input thumbnail on the card). `medias: [{value: "<completed BOARD job_id>", role: "start_image"}, {value: "<CHARACTER SHEET id>", role: "image_references"}]`:
```
A single continuous 15-second vertical 9:16 cinematic music-video sequence built from the [N] shots in the FIRST reference image (the storyboard), played in order as fast hard JUMP CUTS. Use the SECOND reference (the character sheet) to keep the face and identity accurate — black ribbed turtleneck[, glasses]. Deep-shadow single-key lighting. Each shot keeps its background AND its RED caption exactly as in the storyboard — keep the captions static, crisp and legible; do NOT animate, warp, move, or re-spell them. Do not flatten backgrounds to pure black.

SHOT [n] (0.0–2.3s, panel n): [pose]. Deep [calm/building] voice: "[VO LINE]."
HARD JUMP CUT. SHOT [n+1] (2.3–3.2s, panel n+1): [silhouette/beat]. No dialogue.
[...continue timecoded; HOOK beats are MUSIC ONLY, no dialogue; hold the climax line on the longest beat (7)...]

Hard jump cuts between all shots, consistent identity, backgrounds and captions preserved. Filmic, moody, dramatic[, driving beat].
```
VO only on the talking beats (1,3,5,7 in clip one; 15 in clip two). **Hook beats (8–14) = no dialogue, music only.**

### 5C — Run the two clips
`generate_video`: `seedance_2_0`, the 5B prompt, `medias` = **board as `start_image`** + **character sheet as `image_references`** (NEVER role `image` — Seedance silently drops it; the start frame MUST be `start_image`), `generate_audio: true`, `aspect_ratio: 9:16`, `duration: 15` (range 4–15), `resolution: 1080p`, `mode: std`, `genre` from intake. If Higgsfield pauses on a preset, **decline**: re-run with `declined_preset_id: [id]`. **Confirm with the user before submitting** (credit-heavy). → two ~15s clips, then Phase 7.

> **HARD GATE — every clip is image-to-video.** Before submitting, the board's `job_id` must be attached as `start_image`. If the Higgsfield card shows **no input thumbnail**, the references were dropped and it's about to render text-to-video (dark, identity-free) — cancel and re-submit with `start_image`. A clip with no start frame is always a bug here.

**TIMING GOTCHA:** a freshly-submitted image `job_id` isn't ready instantly — feeding it to a video immediately throws **"Media input not found."** Confirm the board is `completed` via `show_generations` first.

---

## PHASE 6 — ROUTE B: INDIVIDUAL FRAMES (max control)

Generate all 16 plates one by one, then animate. More credits, but locked identity per beat and total control.

### 6A — Generate the 16 plates (captions baked on the caption beats)
One still per beat (THE I AM HIM 16), `gpt_image_2`, fed `{CHARACTER SHEET}` + `{face}`. On caption beats (1, 3, 5, 7, 15, 16; optional 10), add the locked caption: *big RED ALL-CAPS Didone-serif caption "[CAP]" across the frame, partly BEHIND head and shoulders.*

- **Office (desk shots — beats 1, 3, 5, 7):**
  ```
  Vertical 9:16 cinematic portrait of the man from the references — exact same face and identity, solid-black ribbed turtleneck[, glasses]. Seated at a desk in a dim home office: a LARGE framed map fills the wall behind him, a few small framed photos beside it, a mechanical keyboard on the desk in the foreground. Pose: [PRAYER/STEEPLE HANDS | HANDS CLASPED | LEANING FORWARD, ONE HAND GESTURING]. Deep-shadow single-key cinematic lighting — one warm hard source, crushed blacks, face emerging from shadow. The map and office stay softly visible behind him — do NOT black them out. [CAPTION BEATS: big RED ALL-CAPS Didone-serif caption "[CAP]" across the frame, partly BEHIND his head and shoulders.] Photoreal, shallow depth of field. Identity exact.
  ```
- **Plain-wall silhouette (beats 2, 8, 11, 13):**
  ```
  Vertical 9:16. A dramatic dark SILHOUETTE of the man (solid-black ribbed turtleneck[, glasses]) against a plain, evenly-lit light/neutral wall — he reads as a near-black silhouette, no office. Pose: [HAND TO CHIN | SIDE PROFILE | ARMS CROSSED | FULL-BODY STANDING]. Stark, graphic, high-contrast, photoreal. No caption.
  ```
- **Dim / pensive (beats 4, 6, 9, 10, 12, 14):**
  ```
  Vertical 9:16 cinematic shot of the man from the references — exact identity, black turtleneck[, glasses]. [EXTREME FACE CLOSE-UP OUT OF SHADOW | SEATED IN A DARK CORNER, HAND AT CHIN | LOW-ANGLE, LEANING BACK | TIGHT CLOSE-UP HOLDING CASH OR A BRAND OBJECT | SEATED LOOKING DOWN WITH A HINT OF MOODY COLOR | SEATED, HEAD BOWED, HAND TO CHIN]. Deep-shadow single-key lighting, crushed blacks. [CAPTION BEATS only: big RED ALL-CAPS Didone-serif caption "[CAP]" partly behind him.] Photoreal, ultra detailed. Identity exact.
  ```
- **Bright two-shot (beat 15)** — see Sidekick; add the RED endorser caption.
- **Bright end-card (beat 16):**
  ```
  Vertical 9:16. Full-body HERO shot of the man (black turtleneck[, glasses]) standing, ARMS CROSSED, confident, on a clean bright gray studio sweep, soft even light. Big RED ALL-CAPS Didone-serif title caption "[CAP16]" (the brand/tagline). Sharp, polished, photoreal. Identity exact.
  ```
Capture each plate's `job_id`. **STOP** — let the user spot-check identity + caption spelling.

### 6B — Then animate (two ways)
- **Per-beat clips (max control):** animate each plate as its own clip. `generate_video`, `seedance_2_0`, `medias: [{plate job_id, role: start_image}]` (add a plate as `role: end_image` only to lock a motion arc). `generate_audio: true` on talking beats, `false` on silent/hook beats. `duration: 4` (the floor — trim in post), `9:16`, `1080p`, `mode: std`, `genre`, `declined_preset_id` if it pauses. Per-beat prompt:
  ```
  The man from the start frame (exact face, black turtleneck[, glasses]) in [the beat's setting], with its RED caption kept static and legible (do NOT warp or re-spell it). He [holds the pose / subtle action] — breathing, a slow blink, a small natural shift, ALIVE not frozen. [Talking beats only: mouth moving continuously the ENTIRE time, deep calm voice: "[VO LINE]."] Camera [locked / slow push-in]. Deep-shadow single-key lighting, background exactly as in the frame — do NOT flatten to black.
  ```
  **Anti-frozen** every clip; **silent on hook beats**; **confirm each plate is `completed`** before feeding it.
- **Composite to boards (fewer renders):** feed the 16 finished plates into the two Route-A storyboard prompts (compositing the provided plates instead of generating panels from scratch) — higher board fidelity than Route A, then 2 video renders via 5B/5C.

*Reference:* the `scene_frames/` folder ships with the skill — the original's scene-by-scene first/last frames (`sceneNN_first.png` / `sceneNN_last.png`, 16 scenes) — per-beat timing/framing reference when you animate shot-by-shot.

**Credit reality:** 16 plates + 16 clips ≈ 8× a 2-clip storyboard run. Confirm with the user before batching.

---

## PHASE 7 — ASSEMBLE (+ caption touch-up if needed)

The captions are baked into the frames, so the pop-ups are already in-font. **If a render warps, moves, or mis-spells a baked caption** (Seedance can distort text in motion), re-composite that one clean in post using the locked words: **RED, ALL-CAPS, Didone serif** (Didot / Bodoni; Playfair Display free stand-in), large, behind-subject mask, on its beat. Hand the user a **caption sheet** — each caption's exact text + its beat + the timecode it pops — so any touch-up is exact.

**Assemble:**
- **Route A:** lay the two 15s clips back-to-back (~30s).
- **Route B (per-beat):** cut the 16 clips in beat order, trimming each to its beat length (most to ~0.8–1s; hold 7 and 15 long) for the fast-cut rhythm.
Over the music bed (the hook section rides on music alone), duck the bed under the dialogue, export 9:16.

---

## SIDEKICK (beat 15 — the two-shot)

The original's beat 15 is the subject at the desk with a second character beside them, hyping them. Three easy paths:

- **A real person** — they upload a photo; build the two-shot feeding `{CHARACTER SHEET}` + `{face}` + `{their second person's media_id}`.
- **A designed character or creature** — Claude designs one standalone first (`generate_image`, no medias), e.g. a mascot, a robot, or a photoreal creature; capture `{SIDEKICK}`; then build the two-shot.
- **Claude's pick** — Claude chooses something fun that fits the brand.

**Two-shot plate (beat 15):**
```
A cinematic two-shot, vertical 9:16, in a brighter normally-lit home office (desk, the wall map behind, keyboard in foreground). The man from the references (exact face and identity, black turtleneck[, glasses]) seated at the desk; beside him, [the second person from their reference | the sidekick from the sidekick reference], composed together, both facing camera, lit on one set. Big RED ALL-CAPS Didone-serif caption "[CAP15]" partly behind them. Photoreal, identity exact[, sidekick exact].
```
**Animate the two-shot** if the sidekick needs action (the hype line, a gag): `generate_video`, `role: start_image` = the two-shot plate (`role: end_image` = an action end-frame to lock an arc), `duration` ~5–7s, `generate_audio: true`.
- **Anti-frozen:** *"breathing, a subtle nod, a blink — NOT frozen."*
- **Sustain the talk:** *"its mouth moves continuously the ENTIRE time, never pausing,"* and **timecode the actions** — *"talks for the first ~5.5s; the gag/effect only in the final ~1.5s."*

---

## KEY LOCKS & GOTCHAS (cheat sheet)

- **Script first.** Lock the exact words before any image — captions are baked in, so wording must be final. Hook beats (8–14) are **music only**, no chant.
- **Route first.** Ask **Storyboards (cheap)** vs **16 individual frames (expensive)** before generating. **Never auto-burn the 16 plate gens.**
- **Captions are generated in-font.** Bake the red Didone pop-ups into the frames (often behind-subject) using the locked text. Only re-composite a caption in post if a render distorts it.
- **Identity = two refs.** Character sheet **+** face close-up on every still.
- **Keep the office visible.** "Near-black background" deletes the map/desk. Say "softly visible behind him."
- **Anti-frozen on single-shot animation.** Explicitly prompt breathing/blink/nod.
- **Sustain dialogue.** "Mouth moving continuously the entire time" + timecode the actions; gags only in the final beat.
- **Image-before-video timing.** Just-submitted `job_id` 404s as "Media input not found." Confirm `completed` via `show_generations` first.
- **Decline auto-presets** with `declined_preset_id` unless the user chose one.
- **Nothing is remembered between chats.** Every run rebuilds the person from the user's own photo.
- **gpt_image_2** at **2k / high, 9:16**. Image models render baked text cleanly — that's why captions live on the stills.
- **seedance_2_0:** full 15s in one render (4–15s), native voice via `generate_audio: true`, `mode: std`, `genre` hint. Roles: the frame to animate → **`start_image`**, optional last frame → **`end_image`**, identity/style refs → **`image_references`**. **There is no `image` role** — that's a gpt_image_2 role; passing it to Seedance drops the ref and forces text-to-video.
- **Higgsfield can't read chat attachments** → upload via `media_upload_widget`; Claude *sees* chat images for QC. Map by filename.
- **No standalone music on this MCP** — the moody bed is a provided track added in post. Seedance gives voice, not music.

---

## TONE & DELIVERY RULES

- Lead with the artifact. No preamble, no closing recap.
- Match the user's message length. Short ask = short reply.
- Prose default; headers/bullets only when structure earns it.
- Push back if the user wants to skip the script lock, skip the route choice (and blindly burn 16 gens), or single-ref the identity; comply on style calls if they override.
- Don't narrate what you're about to do — just do it, then show it.
- No emojis unless the user uses them first.
