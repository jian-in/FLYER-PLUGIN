# GPT Image 2 Keyframe Workflow

Use this reference when FLYER prepares or generates a character anchor, hero style frame, start frame, end frame, or shot keyframe.

## Purpose

GPT Image 2 is the still-image look-development stage. Its output should lock the variables that Seedance must preserve: identity, wardrobe, scene geometry, light direction, palette, materials, framing, and the action state at a shot boundary.

## Sequence

1. Map every input image by number and role.
2. If identity is undefined, create a clean character anchor first.
3. Create one hero style frame after the user approves the proposed direction.
4. Treat the approved frame as the visual source of truth.
5. Create additional shot frames through controlled edits or reference-driven generations. Change only the variables needed by the new shot.
6. Use start and end frames only when the action has a precise transformation, reveal, landing, or state change.

Do not generate an image before the user confirms the visual plan.

## Prompt Order

Write the final prompt in English with short labeled sections:

1. Purpose and format
2. Reference map
3. Scene and visible event
4. Subject identity and wardrobe
5. Performance: gaze, expression, breath, pose, hand action, body weight
6. Composition: aspect ratio, framing, camera height, angle, depth, negative space
7. Light and color
8. Materials and atmosphere
9. Invariants and exact constraints

Use concrete visual language. Camera and lens language should steer perspective and composition, not pretend to be an exact physical simulation.

## 9:16 Recommendation

For API workflows, 1152 × 2048 is an exact 9:16 size with edges divisible by 16. Use high quality for identity-critical anchors and final keyframes; use medium for exploratory drafts when speed matters. If the active product does not expose these parameters, state only the 9:16 requirement in the prompt.

## Reference Pattern

Use explicit roles:

- Image 1: identity reference. Preserve facial geometry, feature spacing, hairline, hairstyle, skin tone, and body proportions.
- Image 2: wardrobe reference. Preserve garment silhouette, layers, fasteners, colors, materials, and accessory placement.
- Image 3: location reference. Preserve architecture, fixed props, entrances, window positions, and practical-light locations.
- Image 4: style reference only. Borrow palette, contrast, texture, and atmosphere; do not borrow identity, wardrobe, or exact composition.

Do not write only “match the references.”

## Generation Template

Purpose and format:
Create a photorealistic cinematic keyframe for a 5–15 second vertical short film. 9:16 composition. This is the approved visual source for later image-to-video generation.

References:
[Numbered role map]

Scene and visible event:
[Location, time, weather, start state, visible action, emotional turn]

Main subject:
[Exact character lock and wardrobe lock]

Performance:
[Gaze target, micro-expression, breath, posture, body weight, hands, prop contact]

Camera and composition:
[Shot size, camera height, angle, perspective feel, subject placement, depth layers, negative space, safe zones]

Lighting and color:
[Motivated source, direction, softness, contrast, exposure, palette, highlight and shadow behavior]

Materials and atmosphere:
[Skin, fabric, hard surfaces, wear, weather interaction, particles only if motivated]

Continuity and constraints:
[Exact invariants]
No identity redesign, beauty retouching, plastic skin, extra fingers, duplicated props, random text, logos, or watermark. Keep the visual hierarchy clean and the environment physically believable.

## Edit Template

Change only:
[One requested change]

Preserve exactly:
[Identity, wardrobe, location geometry, camera, lighting, palette, and all approved elements that must remain]

Do not:
[Targeted drift exclusions]

## Realism Rules

- For live-action realism, explicitly request photorealistic or real-photograph behavior.
- Describe pores, fine hair, wrinkles, wear, moisture, fabric weave, scratches, fingerprints, or condensation only when appropriate.
- Avoid glamour retouching unless the story is a deliberate fashion image.
- Preserve a plausible relationship between skin exposure and background exposure.
- Use one dominant composition and one motivated light structure.
- Do not substitute generic “8K” or “ultra detailed” for material description.

## Iteration

When a frame is close, edit rather than restart.

- Change one high-risk variable at a time.
- Repeat the invariant block on every identity-sensitive edit.
- If the face drifts, return to the character anchor.
- If only color drifts, keep geometry and identity fixed and change the light/palette instruction only.
- If the new camera angle requires unseen wardrobe or location detail, ask rather than inventing a permanent trait.

