# Gulper

A 3D browser game about feeding a giant Venus flytrap until the humans declare war on it. Open `index.html` in any modern browser with WebGL; there is no build step. It loads three.js r128 from cdnjs.

## Controls

- **Aim:** mouse, a dragged finger, or the arrow keys / WASD. The trap locks onto prey near the cursor (yellow ring = edible, red = dangerous, grey = too big).
- **Snap:** click, tap or Space.
- **Shop:** the buttons along the bottom, or keys 1, 2, 3.
- **Camera:** Q and E turn around the plant. P or Escape pauses.

## How it plays

- Fullness drains over time; when it hits zero the plant loses health. Health also shows on the plant itself, which browns as it gets hurt.
- Every catch earns coins. Bigger meals, later stages and combos (catches within 2.5 s of each other, up to ×5) pay more.
- The shop sells a **free meal** (+60 fullness), a **swarm** of stage-appropriate prey (flies, beetles, bats, pigeons, ducks, then a tour bus of tourists) and a **regrow** (+50 health). Prices rise with each stage.
- Each growth stage enlarges the plant and its reach, pulls the camera back, unlocks bigger prey and heals some health:

| Digested | Stage | What changes |
| --- | --- | --- |
| 0 mg | Seedling | Flies and moths. Wasps sting, pebbles stun the jaws. |
| 1 g | Snapper | Beetles and golden flies. |
| 30 g | Bog Brute | Bats and thrown steaks. |
| 1 kg | Greenhouse Menace | Wasps and pebbles are harmless snacks. Pigeons and ducks. |
| 20 kg | Leviathan | Goats wander in. |
| 100 kg | Titan | Tourists arrive to take photos, plus cows. |
| 1 t | Doom Bloom | Army jeeps become edible. |
| 10 t | World Eater | Tanks become edible. |

- Eat four humans (or reach 400 kg as a Titan) and the humans declare war: rifle squads, then jeeps with machine guns and tanks firing shells.
- Your best score is kept in the browser's local storage.
