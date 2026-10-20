# Self-expanding transcatheter valve

34-second anatomical motion study of a self-expanding transcatheter aortic valve. A 14-French delivery catheter crosses a calcified native valve, the outer capsule pulls back, a nitinol frame recovers its set shape, and three porcine pericardial leaflets open in systole and seal in diastole.

Open `index.html` in a browser. The study is 1,020 frames at 30 fps and loops. Scrub the timeline, or jump with keys `1` through `5`. Space plays and pauses. Arrow keys step frames.

| Frames | Time | What you are looking at |
| --- | --- | --- |
| 0–150 | 0–5 s | Axial view. Catheter across the stenotic valve. Marker bands settle on the annular plane. |
| 151–300 | 5–10 s | Capsule pullback. Uncovered nitinol opens. Diamond cells widen. |
| 301–510 | 10–17 s | Cutaway. Struts pin calcified leaflets into the sinuses. Coronary ostia stay above the skirt. |
| 511–750 | 17–25 s | Down-bore view. Three leaflets open, then coapt. |
| 751–1019 | 25–34 s | Dolly back to a cut section. Pulsatile streamlines, sinus recirculation, coronary fill in diastole. |

Geometry is stylized so the catheter, frame, and root read in one frame. This is not a device, not an instruction for use, and not a prediction of a clinical result. The sealed skirt is a property of this model.

Space Grotesk is included under the SIL Open Font License. See `fonts/OFL.txt`.

## GitHub Pages

From a machine that is already authenticated as `mizcausevic-dev`:

```bash
gh repo create mizcausevic-dev/tavr-valve-jig --public --source=. --remote=origin --push
gh repo edit mizcausevic-dev/tavr-valve-jig --description "34-second anatomical motion study of self-expanding transcatheter aortic valve deployment."
gh repo edit mizcausevic-dev/tavr-valve-jig --add-topic medical-animation --add-topic tavr --add-topic nitinol --add-topic heart-valve --add-topic anatomy --add-topic canvas --add-topic motion-design --add-topic education --add-topic hemodynamics --add-topic cardiac
gh api -X POST repos/mizcausevic-dev/tavr-valve-jig/pages -f build_type=legacy -f source[branch]=cursor/tavr-valve-jig-2c88 -f source[path]=/
```

The Pages entry file is `index.html`.
