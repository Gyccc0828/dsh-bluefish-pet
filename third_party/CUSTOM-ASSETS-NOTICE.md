# Custom Claude outfit asset · 2026-10-23

This file records the provenance of the customized asset
`assets/webm/变装-穿Claude衣服.webm`. This is unofficial fan artwork.

Original desktop pet and animation source: **PC2005-cloud/dsh-pet**
<https://github.com/PC2005-cloud/dsh-pet>.
The original project's code is MIT; its animation/artwork rules allow open-source
use and prohibit commercial use. Preserve the original project's attribution.

Outfit-only reference: **CrossPet**, by **lokicorvus**, Claude hoodie skin,
`characters/deepseek-hoodie/idle.webp`:
<https://github.com/lokicorvus/crosspet/blob/6e98970f6ff9b44e8ac85215241cabcd78f67d92/characters/deepseek-hoodie/idle.webp>.
CrossPet's character artwork is licensed **CC BY-NC-SA 4.0**:
<https://github.com/lokicorvus/crosspet/blob/6e98970f6ff9b44e8ac85215241cabcd78f67d92/characters/LICENSE.md>.
Character provenance credited by CrossPet: original Mingyue design by **上善无形**;
DeepSeek whale-maid interpretation by **ZipZipPipe**.

Changes made for this local customization: used the original dsh-pet idle sprite
as the identity/style target and the CrossPet sprite only as clothing reference;
recreated the hoodie artwork with the built-in OpenAI image_gen tool; retained the
navy hair, eyes, fin ears, lace headband, hair bow, whale tail, and original-scale
proportions; added cream/terracotta hoodie, a small Claude badge, gentle bob/sway,
and two short silhouette transitions. Encoded to a 640×360, 24 fps, 241-frame
VP9-alpha WebM, returning to the original outfit at the end.

The new derived clothing artwork and the new derived WebM are shared under
**CC BY-NC-SA 4.0**, subject to the underlying sources' applicable rights:
<https://creativecommons.org/licenses/by-nc-sa/4.0/>.
The asset is for noncommercial use. Preserve attribution and this notice with it.
Other files retain their existing licenses. The older third-party cos-Claude
sprite sheet is no longer used in the replacement animation.

## Falling deep basin action · 2026-10-23

Current asset: `assets/webm/头顶铁盆-落下晃稳.webm`, 640×360, 60 fps,
603 frames, VP9 with alpha. The original **PC2005-cloud/dsh-pet** idle video
is used continuously as the character layer, without replacing, redrawing,
reshaping, or flashing the character.

Only the independent deep, inverted silver basin prop was generated with the
built-in OpenAI image_gen tool. The original idle sprite was a drawing-style
reference. The large/deep, low-over-forehead basin silhouette reference was:
<https://github.com/Witherwithwinter/DeepSeek-Balance-Whale-Widget-Bowl/blob/2154a5deb30039f9f5825677b653a825975fcee2/assets/DSniang-bowl.png>.
The reference character image is no longer composited into the video.
`BASIN-SOURCE-LICENSE.txt` retains the reference repository's MIT notice.

Animation: the prop enters from above with alternating tilt, lands on the head,
has a small bounce and damped lateral wobble, then settles low over the forehead.
It holds steady before a short prop-only fade at the very end, restoring the
normal idle frame without a character cut or silhouette flash.

The previous static-pose basin clips, knock/rebound clip, steel-pipe clip and
steel-pipe work-error candidate have been removed. No pipe artwork or motion
code from dsh-bonk-pet is used by the current action.

Original animation: <https://github.com/PC2005-cloud/dsh-pet>.
Character provenance: **上善无形** and **ZipZipPipe**. Keep attribution and
applicable underlying rights. Use these local fan-art derivatives
noncommercially. The generated basin prop and new derived clip are shared
under CC BY-NC-SA 4.0, subject to the underlying character/animation rights.
The separately documented Claude asset keeps its existing terms.

## Approved Claude hoodie work actions · 2026-10-24

`assets/webm/变装-Claude羽毛笔写字.webm` and
`assets/webm/变装-Claude左右递文件.webm` use complete, unmodified
CrossPet / lokicorvus character images: `writing.webp`, `busy_left.webp`,
and `busy_right.webp` from `characters/deepseek-hoodie/` at commit
`6e98970f6ff9b44e8ac85215241cabcd78f67d92`:
<https://github.com/lokicorvus/crosspet/tree/6e98970f6ff9b44e8ac85215241cabcd78f67d92/characters/deepseek-hoodie>.

Animation adaptation: complete-character gentle vertical bob; the busy action
switches the complete left/right poses every 1.5 seconds. Both are 12-second,
640×360, 60 fps VP9-alpha WebM loops. No new artwork or separate limb layers are
generated or composited for these two clips. Fingers and props retain their
source pose; these clips are not continuous finger-typing animation.

Character provenance: original Mingyue by 上善无形; deep-blue whale-maid
interpretation by ZipZipPipe. CrossPet artwork and these derivative clips use
CC BY-NC-SA 4.0: attribution, noncommercial use and share alike. Preserve the
upstream notice in `CLAUDE-WORK-SOURCE-LICENSE.md` with these assets.
The earlier generated laptop/keyboard work clips were previews only and are
not installed by this revision. The existing basic Claude outfit stays intact.
