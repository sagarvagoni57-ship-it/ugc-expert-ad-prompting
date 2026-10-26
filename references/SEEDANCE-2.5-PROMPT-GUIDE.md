# Seedance 2.5 UGC prompt guide

This is a prompt-writing guide, not a claim about a particular Seedance 2.5 interface. The receiving agent must use the connected tool's current schema when one exists. If no schema is available, use the natural-language prompt and do not invent parameter names or reference limits.

## 1. Prompt architecture

Write the master prompt in this order so the model can prioritize what must stay consistent:

1. **Deliverable and runtime:** "Create a 20-second vertical 9:16 ecommerce UGC ad concept..." Treat 20 seconds as an edit target.
2. **Product authority:** name the supplied product reference and describe only visible, verified identity details. State that it controls silhouette, packaging, color, label layout, hardware and scale.
3. **Creator authority:** name the supplied or planned adult actor reference. State what must remain identical: face, hair, complexion, age presentation, body/wardrobe when relevant.
4. **Audience and viewer situation:** a concrete US/UK viewer moment, not a vague demographic.
5. **Location and light:** a plausible real room, time of day, key-light direction, exposure and background context.
6. **Camera grammar:** selfie/front camera, fixed phone, handheld close-up, mirror or POV. State lens distance and when a motivated reframing or insert occurs.
7. **Performance:** eye line, posture, exact emotion cause, breath, pause, gesture and physical contact.
8. **Timed action and dialogue:** local beat timings that sum to 20 seconds; every spoken line exact.
9. **Continuity locks:** product variant, actor, wardrobe, location, light direction, prop anchor and hand used for the action.
10. **Post-production:** captions, exact package copy, CTA, disclosure, sound mix and any composited logo/text.
11. **Avoid list:** only the failure modes relevant to this prompt.

Do not hide critical details in a separate note and write "use the above". The master prompt must stand alone when pasted into a new generation request.

## 2. Reference hierarchy

Use semantic roles in the prompt and upload map:

```text
PRODUCT_REFERENCE = supplied product image or product cutout; appearance authority
ACTOR_IDENTITY = supplied/authorized or fictional adult creator portrait; identity authority
WARDROBE_REFERENCE = optional outfit/body reference for try-on or consistent styling
OPENING_FRAME = optional scene-specific first frame; only if the destination workflow supports it
STYLE_REFERENCE = optional reference for camera, pacing or lighting only
```

Never let a style frame replace the actual product image. Never let an actor portrait define the final room. Do not assume a contact sheet or multi-view character sheet is a valid first video frame. If the tool accepts only one reference, prioritize the product for product-led ads; add the actor only when facial identity is essential and the tool supports multiple roles.

## 3. Twenty-second timing template

Use these as edit targets and adapt them to the product. The final timestamps must cover 0.0 to 20.0 seconds without gaps or overlaps.

| Time | Visual job | Dialogue job |
|---|---|---|
| 0.0–2.0 | Start mid-action; product context visible or immediately revealed | 4–6 conversational words, one hook |
| 2.0–6.0 | Show the viewer situation and establish the product in hand/position | Name what is happening; avoid a benefit pile |
| 6.0–13.0 | One simple demonstration; use close insert only when it improves comprehension | One feature/method line with a natural pause |
| 13.0–17.0 | Show the observable result/detail: fit, texture, movement, sound, organization or completion | Explain what the viewer can actually see |
| 17.0–20.0 | Set product down or hold steady; protect end-card space | One low-pressure CTA; leave a half-second visual hold |

If a reference is a 4–15 second clip, borrow its pacing and action design, then extend by adding a useful detail or a calm product hold. Do not loop the hook or pad time with random hand movement. If the model only renders shorter clips, write complete local prompts, preserve the continuity lock and provide an assembly map that totals 20 seconds.

## 4. Dialogue and audio

- Write natural US English by default; use UK spelling or phrasing only when requested or appropriate to the market.
- Keep most 20-second scripts around 35–45 spoken words, but prioritize intelligibility over a quota. Count words and estimate a calm delivery with pauses.
- Spoken copy must match the visual action. A creator should not describe a feature before it appears or claim a result not visible in the shot.
- Use an on-camera line when eye contact and trust are useful; use voiceover for hands-only, ASMR or product-led shots.
- Mark pauses with punctuation or `[beat]`, not with vague directions such as "sound excited".
- Specify room tone and only the necessary effects: zipper, cap click, pump, pour, fabric movement, button press, crunch or soft music bed.
- If synchronized speech is not verified, write: "Dialogue may be recorded/added in edit; use this exact script and preserve the shot timing." Never promise lip-sync.
- Captions are post-production text, not a substitute for dialogue. Keep captions short and readable on a phone.

## 5. Camera, light and physical realism

Use a small number of intentional camera instructions:

- **Selfie:** phone at eye height or slightly above, arm-length framing, minor hand movement, autofocus breathing, ordinary background.
- **Fixed phone:** phone on a shelf/tripod, stable medium shot, actor moves into the frame, cut to a close insert only when needed.
- **Hands/product insert:** close focus on the product, real contact shadow, believable grip, no floating object, no extra duplicate.
- **Mirror/try-on:** phone reflection is coherent, actor's gaze follows the mirror, outfit and body proportions stay consistent.
- **POV/security camera:** name the camera position and distortion once; keep the joke legible and the product safe.

Describe the light source and its consequence: soft window light from camera-left, warm kitchen practical, cool bathroom daylight, or overhead gym light. Avoid lists of contradictory lighting adjectives. Keep skin texture natural, with realistic exposure and no beauty-filter smoothing.

For product motion, state material behavior: a cap hinges, a zipper closes, a pouch flexes, liquid follows gravity, fabric folds, foam compresses, or a screen emits light. Never ask for impossible physical motion just because it looks cinematic.

## 6. Product continuity locks

Repeat the non-negotiables near the timeline and again in the avoid list:

- exact product/variant and supplied reference
- silhouette, dimensions relative to hand and visible markings
- one hero product unless a multipack is explicitly supplied
- label/logo text added in post when the model cannot render it reliably
- no redesign, invented accessory, altered cap, duplicate object or unexplained color shift
- same hand contact and anchor position when the shot cuts back

If only a front photo is supplied, keep the product front-facing or use a conservative angle. Do not invent a rear label, hidden button or mechanism.

## 7. Creator realism and continuity

The creator is a demonstrator, not a fabricated customer testimonial. Direct the actor with observable actions:

- opening: eyes on the action, one short glance to lens
- problem: a small brow pinch, pause or exhale; no panic or shame
- demonstration: focused look, slower hands, one clear gesture
- payoff: relaxed brow, small smile or confident nod caused by the visible action
- close: product held steady, calm CTA and a brief hold

Keep the same adult identity, hair, wardrobe, makeup level, body proportions, room, key light and product variant. A jump cut may change clothing only when the concept is a deliberate try-on transition; state the before and after explicitly.

## 8. Post-production and failure handling

Always separate generated action from edit work:

- add exact package text, logo, captions, CTA and disclosure in edit when spelling matters
- composite the supplied product photo for the end card if generated packaging is unreliable
- use a clean voice track or captions if the model's speech is not stable
- review hands, face continuity, product identity, timing, audio and text at 100% before delivery

When a first render fails, diagnose one cause at a time: product drift, actor drift, hand physics, dialogue timing, camera inconsistency or unsupported claim. Tighten the prompt locally; do not add twenty more realism adjectives. Do not silently change the product or the claim to make the render easier.

## 9. Prompt skeleton

```text
Create a 20-second vertical 9:16 ecommerce UGC ad concept for [audience/use case].

REFERENCES
PRODUCT_REFERENCE: [actual filename/handle]. It is the exact [product/variant]. Preserve [visible identity details]. Do not redesign the package.
ACTOR_IDENTITY: [actual filename/handle or fictional adult reference pending]. Preserve [identity traits].
STYLE_REFERENCE: [optional filename/handle], used only for [camera/pacing/light].

SCENE
[real location], [time of day], [light source/direction], [ordinary background]. [selfie/fixed/POV] camera at [position]. Natural texture and exposure.

PERFORMANCE + TIMELINE
0.0–2.0s: [visible hook]. [exact line]. [emotion caused by action].
2.0–6.0s: [use situation and product placement]. [exact line].
6.0–13.0s: [one demonstration]. [exact line].
13.0–17.0s: [observable payoff/detail]. [exact line].
17.0–20.0s: [product hold/end action]. [exact CTA]. Hold final product frame.

AUDIO
[voice type/accent], [room tone], [specific product sounds]. If sync is not supported, add the exact script in edit.

POST
Add [exact text/captions/CTA/disclosure] in post. Keep safe margins for vertical UI.

CONTINUITY + AVOID
[locks]. No [specific failure modes, unsupported claims, duplicate products, fake testimonial or impossible motion].
```
