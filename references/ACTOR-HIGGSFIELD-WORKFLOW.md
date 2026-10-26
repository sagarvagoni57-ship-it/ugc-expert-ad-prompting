# Higgsfield actor-reference workflow

This workflow is only for a fictional adult actor/influencer reference. It does not render the final UGC ad, product hero, commercial, static image, storyboard, voice, music or published asset.

## Decide whether an actor is needed

Use no actor when the product is understood better through hands, packaging, a machine operation, ASMR or a clean product-only POV. Use a face when eye-line trust, a verbal explanation, try-on, reaction or couple interaction materially helps the viewer.

## Intake for a fictional adult

Collect only what changes the ad: adult age presentation, general appearance, hair, skin texture, wardrobe, casting tone, market-neutral accent and whether a waist-up or full-body view is needed. Do not request identity documents, sensitive traits or celebrity likenesses. Do not equate nationality, ethnicity or gender with expertise.

If the user already supplied an authorized actor reference, reuse it. Do not create a new identity merely to vary a prompt. Keep a creator roster when several portfolio ads share an actor, but do not present the actor as a real customer.

## Bounded generation plan

Prefer:

1. one identity portrait;
2. one optional matching body/wardrobe view only when the ad needs it;
3. one targeted correction only if a concrete defect blocks use.

Keep the total to at most three output images for one ad request unless the user explicitly changes the budget and scope. Never purchase credits or change a subscription. Inspect the result when the connected tool allows it and report actual status or a real URL; never invent a job ID or asset handle.

## Portrait prompt pattern

```text
Create one photorealistic reference portrait of a fictional adult creator for a later ecommerce UGC video. [age presentation and stable facial/hair traits]. Waist-up framing, relaxed direct gaze, natural skin texture, ordinary approachable expression, neutral wardrobe suitable for [product category], soft directional window light, plain unobtrusive background. Single person, single image, no text, no collage, no celebrity resemblance, no product endorsement, no beauty-filter smoothing. This is an identity reference, not the final advertisement.
```

For a body/wardrobe view, preserve the exact selected identity and outfit. For an opening frame, include the actual product reference only if the destination workflow supports a scene-specific reference and the product can be preserved accurately. A portrait background does not become the ad location automatically.

## Handoff map

Return a plain-language map:

- `PRODUCT_REFERENCE`: actual product image or handle, used for product identity.
- `ACTOR_IDENTITY`: actual Higgsfield result/filename, used for face and hair.
- `WARDROBE_REFERENCE`: optional body/outfit image, used only for continuity.
- `OPENING_FRAME`: optional first-frame scene reference, only if the final video workflow supports it.

Do not invent syntax such as `@Creator`, image counts or Seedance fields. If the connector is missing or actor creation fails, say `Actor reference abhi generate nahi hua`, give the complete portrait prompt and continue with an ad prompt marked `ACTOR_IDENTITY pending`.

## Quality inspection

Check apparent adulthood, face and hair consistency, natural eyes/skin/hands, wardrobe fit, unwanted text, celebrity resemblance, and whether any product shown is only a supporting prop. A good actor sheet does not guarantee downstream identity, lip-sync, hands or package-label fidelity; the final video must still be reviewed.
