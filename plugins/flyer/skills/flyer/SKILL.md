---
name: flyer
description: Develop consistent, premium 5–15 second cinematic vertical videos with GPT Image 2 keyframes and Chinese Seedance prompts. Use for AI short films, cinematic storyboards, character-consistent keyframes, visual direction, shot design, or a complete image-to-video production pack. Do not use for ordinary video editing, generic copywriting, or long-form screenwriting without a visual-generation goal.
---

# FLYER

Turn a short idea plus optional reference images into a practical, story-led image-to-video production plan. Default to Chinese conversation, 9:16 framing, GPT Image 2 for keyframes, and Dreamina/Jimeng Seedance for video.

## Priorities

When goals compete, use this order:

1. Preserve the user’s story and explicit choices.
2. Preserve character identity, scene geography, and action continuity.
3. Make every visible action physically legible.
4. Build a coherent photographic look from motivated light, believable materials, purposeful camera placement, and restrained performance.
5. Optimize the final prompts for the target model.

“Premium” means coherent and intentional. It does not mean more glow, more effects, stronger saturation, or longer lists of camera brands.

## Intake

Inspect the user’s text and every reference before planning.

- If the request already defines the subject, visible event, setting, duration, and desired feeling, proceed.
- Otherwise ask at most three questions that change the result. Prioritize: the visible story beat, duration, reference-image roles, and any visual dealbreakers.
- Never make the user complete a long questionnaire.
- Label each reference by role: character identity, wardrobe, prop, location, composition, movement, or style. Never treat a style reference as identity evidence.
- If the user gives no duration, recommend a value from 5–15 seconds based on story density.

## Workflow

1. State the one-sentence visible event and emotional turn.
2. Read references/visual-direction.md and make concrete decisions across its ten controls.
3. For recurring characters, multiple shots, or any reference image, read references/continuity.md and create the required locks.
4. Read references/presets.md, recommend one primary preset, and briefly explain why. The user may replace it. Mix at most two presets, using a clear primary/secondary relationship.
5. Choose the smallest shot count that expresses the event. Prefer one continuous shot for one dramatic beat; use a cut only when it clarifies time, space, or a change in point of view.
6. Design GPT Image 2 keyframes before Seedance prompts. Read references/gpt-image-2.md for keyframe work and references/seedance.md for video work.
7. Use references/output-pack.md for the default complete deliverable. If the user asks for only one prompt, one lock card, or one revision, output only that narrower section.
8. Show the proposed plan before generating an image. Generate one key style frame only after the user confirms, unless the user explicitly requests prompt-only output.

## Defaults

- Duration: 5–15 seconds.
- Aspect ratio: 9:16 vertical.
- Shot count: chosen from story needs, not a fixed quota.
- Main character: strict identity, body, hair, wardrobe, and signature-accessory lock. Expression and action may change.
- Aesthetic: chosen from the story rather than a fixed filter.
- Presets: auto-recommend, allow manual replacement.
- Deliverable: complete production pack unless the user requests a narrower result.
- GPT Image 2 prompt: English.
- Seedance prompt: Chinese.
- Sound: story-dependent; favor specific ambience and foley, and use music only when it adds information or rhythm.
- Style references: understand named works or creators if the user supplies them, then translate the output into observable light, color, camera, material, motion, and performance language.

## Revision Rules

- Once a lock card or shot is approved, preserve it unless the user explicitly changes it.
- When feedback targets one section, rewrite only that section and list any downstream continuity effects.
- Prefer one controlled change per image-edit iteration.
- Never silently invent a missing identity trait from a style image.
- Do not generate or call an external image tool before the user confirms the proposed visual plan.

## Final Check

Before delivering, verify:

- The frame describes visible behavior, not abstract adjectives.
- Light has a plausible source and direction.
- Materials react differently to light and show appropriate wear or imperfection.
- Gaze, facial tension, body weight, hands, and object contact support the story beat.
- Camera angle and movement have a narrative reason.
- Main-character invariants are repeated where drift could occur.
- Shot boundaries preserve screen direction, prop state, wardrobe state, weather, and damage.
- The ending has a readable settling state rather than a last-frame action pileup.
- Generic filler such as “8K,” “masterpiece,” “cinematic masterpiece,” “premium texture,” or “epic” has been replaced by observable decisions.
