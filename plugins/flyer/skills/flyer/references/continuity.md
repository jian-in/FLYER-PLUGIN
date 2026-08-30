# FLYER Continuity System

Use this reference for any recurring character, multiple shot, continuation, edit, or reference-driven task.

## Reference Map

Number every input and assign exactly one primary role.

| Role | Extract | Do not infer |
| --- | --- | --- |
| Character identity | face geometry, feature spacing, hairline, hairstyle, skin tone, age cues, body proportions | wardrobe details hidden by crop |
| Wardrobe | silhouette, layers, closures, colors, materials, wear, accessories | facial identity |
| Prop | dimensions, material, damage, grip points, orientation | character scale unless shown |
| Location | geometry, entrances, windows, horizon, practical lights, fixed props | time changes not shown |
| Composition | subject placement, camera height, depth arrangement | identity or material |
| Motion | trajectory, tempo, body mechanics, camera relation | still-frame appearance |
| Style | palette, contrast, texture, lens feel, atmosphere | identity, wardrobe, exact location |

If one image serves several roles, state each role separately. Never say only “use the reference.”

## Main Character Lock

Create a concise canonical block and reuse it without synonyms that could drift.

Lock:

- face shape and bone structure
- eye shape, spacing, iris color, brows
- nose, mouth, ears, distinctive marks
- hairline, length, texture, part, accessories
- skin tone and age cues
- height impression and body proportions
- wardrobe silhouette, layers, fasteners, colors, materials
- footwear and signature accessories

Allow:

- expression, gaze, breath, pose, and action
- physically caused dirt, wetness, sweat, wrinkles, or damage
- explicitly approved story changes

Do not “beautify,” age-shift, slim, masculinize, feminize, or redesign the character unless requested.

## Scene Lock

Record:

- floor plan and screen directions
- doorway, window, horizon, furniture, and major-prop positions
- time of day, weather, atmosphere, and motivated light direction
- palette, contrast, texture, and exposure baseline
- accumulated state such as broken glass, wet floor, smoke density, footprints, or displaced objects

If time changes, state what changes and what remains.

## Shot Boundary State

For every cut, carry the outgoing state into the next shot:

- character location and screen side
- gaze and eyeline target
- body orientation and weight-bearing foot
- hand positions and held-object orientation
- wardrobe closure, wrinkles, wetness, dirt, blood, or damage
- prop position and condition
- light direction, weather, and atmosphere
- camera axis and direction of travel

Do not cross the action axis unintentionally. If the axis changes, show the transition or use a neutral connecting shot.

## Keyframe Strategy

Use the minimum set that controls the risky variables.

- No reference character: first make a clean character anchor before scene keyframes.
- Strong character reference: create a hero style frame that combines identity, wardrobe, location, and lighting.
- Simple one-beat motion: one approved start keyframe can be enough.
- Transformation, reveal, or precise landing: use compatible start and end frames.
- Multiple shots: make separate keyframes; do not rely on a single nine-panel sheet for final identity control.

The first approved frame becomes the visual source of truth. Later frames must restate the lock and name only the intended changes.

## Prompt Invariant Pattern

For each generation or edit:

1. Name the input image roles.
2. State the visible change requested in this iteration.
3. Repeat the exact invariant block.
4. State camera and lighting elements that must remain.
5. Add a short exclusion list targeted at known drift.

For edits, prefer “change only X; keep everything else unchanged.” Make one controlled change at a time when identity or layout is fragile.

## Drift Repair

Repair the smallest broken layer.

- Face drift: return to the character anchor, restate facial geometry, change only pose or expression.
- Wardrobe drift: use the approved wardrobe frame, restate silhouette, closures, material, and accessory positions.
- Color drift: restate light sources and palette; do not compensate with generic “same style.”
- Geography drift: re-anchor the location and prop positions before changing camera angle.
- Action discontinuity: explicitly write the prior ending pose and next starting pose.

Do not reroll an entire sequence to fix one local error unless the lock itself is wrong.
