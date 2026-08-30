# FLYER Complete Production Pack

Use this structure by default for a full project. Keep it concise enough to operate. Do not reveal hidden chain-of-thought; provide decisions, assumptions, and production-ready artifacts.

## 1. Project Card

- Title
- One-sentence visible event
- Emotional turn
- Duration and aspect ratio
- Target models
- Assumptions, if any

## 2. Director Recommendation

- Primary preset
- Optional secondary preset
- Two or three sentences explaining why the choice serves the story
- The central anti-cheap decision: what FLYER deliberately refuses to overdo

## 3. Reference Map

Number every reference and state its role. Identify missing identity, wardrobe, prop, location, movement, or style evidence.

## 4. Lock Cards

### Main Character Lock

Canonical identity, proportions, hair, wardrobe, footwear, and signature accessories.

### Scene Lock

Geography, fixed props, time, weather, practical lights, light direction, palette, atmosphere, and accumulated damage or wetness.

### Visual Lock

Composition logic, lens feel, contrast, exposure, material response, image texture, and color limits.

### Change Budget

List what may change in this clip: expression, gaze, pose, action, dirt, damage, weather, or other approved variables.

## 5. Shot Plan

Use a table:

| Shot/time | Visible event | Performance and blocking | Camera and composition | Light and materials | Sound | Continuity in/out |
| --- | --- | --- | --- | --- | --- | --- |

Use the smallest useful shot count. For a one-shot clip, divide by meaningful time beats rather than inventing cuts.

## 6. GPT Image 2 Keyframe Prompts

- Output in English.
- Identify whether each prompt is a character anchor, hero style frame, start frame, end frame, or shot frame.
- Include the numbered reference map and exact invariants.
- Recommend one keyframe first. Do not generate it until the user confirms.

## 7. Seedance Prompt

- Output one Chinese copyable block.
- Include reference binding, global invariants, timed visible action, camera, light, materials, sound, settling state, and targeted avoid list.
- Preserve approved wording of identity and wardrobe locks.

## 8. Generation Order

Give an operational sequence:

1. Approve project card, preset, and locks.
2. Generate one hero style frame.
3. Correct the smallest broken layer and approve the frame.
4. Generate any additional start/end or shot keyframes.
5. Run Seedance with bound references.
6. Repair only the failed layer; do not rebuild the entire project by default.

## 9. Preflight

Check:

- story is visible within 5–15 seconds
- 9:16 safe zones are protected
- main character lock is exact and repeated
- reference roles do not conflict
- lighting source and direction are plausible
- materials respond differently and show appropriate imperfections
- pose, hand action, gaze, and expression are physically and emotionally aligned
- each camera move has one job and settles
- sound is specific and restrained
- final moment is readable
- prompts contain no empty quality slogans

## Revision Behavior

If the user changes one choice:

- rewrite only the affected section
- preserve approved locks and prompts
- state downstream changes in one short note
- request a new confirmation only if the change affects identity, the visual source of truth, or the generation plan
