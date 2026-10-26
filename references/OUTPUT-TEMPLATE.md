# UGC agent output template and quality gate

Use this format for the agent's final answer. Explain the short brief in Hinglish; write the copy-ready generation prompt in English unless the user asks for another language.

## 1. Hinglish brief

State:

- Product and exact variant understood
- Audience situation and chosen UGC archetype
- One viewer value / supported product action
- Observed facts, source-supported facts, creative assumptions and material unknowns
- Whether a face/actor is needed and why

Keep this section concise. Never hide an important uncertainty.

## 2. Reference upload map

Use actual user filenames, links or returned handles. Mark each as required or optional:

| Role | Asset | Use |
|---|---|---|
| PRODUCT_REFERENCE | actual product image/link | exact packaging, shape, color, label, scale |
| ACTOR_IDENTITY | actual authorized or generated adult reference | face, hair, stable identity |
| WARDROBE_REFERENCE | actual optional view | try-on/body/outfit continuity |
| STYLE_OR_MOTION_REFERENCE | actual optional ad reference | camera, pacing, lighting only |
| OPENING_FRAME | actual optional scene frame | first frame only when supported |

If an asset is planned but not generated, mark it `pending`; do not claim it exists.

## 3. Timed storyboard

Use a table with these columns:

| Time | Shot / camera | Actor action and emotion | Product action / visibility | Exact dialogue | Post text / sound |
|---|---|---|---|---|---|

The time range must start at 0.0 and end at 20.0. Dialogue must be complete, natural and assigned to the creator or voiceover. Do not hide the CTA in a paragraph.

## 4. Master prompt

Give one standalone English block with:

- target, format and duration
- reference roles and product/creator locks
- location, lighting and camera grammar
- exact action and dialogue by time
- emotion direction tied to actions
- audio and caption plan
- continuity locks
- negative/avoid constraints

The user should be able to paste this block without combining it with the storyboard.

## 5. Edit and safety notes

Mention only relevant items:

- add exact logo/package copy, subtitles and CTA in post if generation may distort them;
- keep disclosure for synthetic actor/spec work separate from spoken dialogue;
- use a voice/caption edit if synchronized speech is not verified;
- check product identity, hands, eyes, body/wardrobe, timing and audio at 100%;
- do not publish unsupported claims, fake testimonials or unverified pricing/offer language.

## Final quality gate

Do not deliver until each answer is yes or clearly marked as a limitation:

- Can the viewer understand the product's useful role with audio muted?
- Is the product visible early and faithful to the supplied reference?
- Is there one viewer situation, one demonstration and one CTA?
- Is every claim supported or explicitly framed as a creative assumption?
- Does each action fit the product's size, weight, mechanism and intended use?
- Does the emotional change have a visible cause?
- Are actor, wardrobe, room, light and product continuous across cuts?
- Do the dialogue words fit a calm 20-second delivery with pauses?
- Does the time map cover exactly 20 seconds without padding or cut-off speech?
- Are generated text, captions and disclosure assigned to post where appropriate?
- Is the reference/upload map honest and free of invented IDs or tool syntax?
