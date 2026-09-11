# Hero render — wireframe

To-scale Three.js wireframe of the hall: screen bank on C-stands and Matthews stands,
the pallet rack, and every cable run. 1 unit = 1 metre. Built from
`herorenderlastlightclean.blend` / `herorenderlastlightclean1.obj`.

- `index.html` — landing page, the rotating ring opens the viewer
- `wireframe.html` — the viewer itself, fully self-contained (Three.js loads from jsDelivr)
- `.nojekyll` — stops GitHub Pages running Jekyll over the files

## Publish

1. Create a repo and copy these files into its root.
2. `git add . && git commit -m "wireframe" && git push`
3. Repo → Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
4. The site appears at `https://<user>.github.io/<repo>/` within a minute or two.

To publish from a `docs/` folder instead, put the files in `docs/` and pick that folder in step 3.

## Viewer controls

Drag to orbit, right-drag to pan, scroll to zoom. Click any line to identify the part.
`H` hides the HUD for a clean screenshot. Layers and preset views are in the left panel.

`wireframe.html` is ~4 MB because the line geometry is embedded — well inside the
100 MB GitHub file limit, but it is a single request, so expect a beat on first load.
