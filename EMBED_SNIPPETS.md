# Example Embed Snippets

## Basic Luma AI Embed

Replace `YOUR_SCENE_ID` with the ID from your Luma share URL.
e.g. if the URL is `https://lumalabs.ai/capture/abc123` → scene ID is `abc123`

```html
<iframe
  src="https://lumalabs.ai/embed/YOUR_SCENE_ID?mode=sparkles&background=%230a0a0a&color=%23ffffff&showTitle=false&loadBg=true"
  width="100%"
  height="500"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen
></iframe>
```

## Luma Embed URL Parameters

| Parameter | Options | Notes |
|-----------|---------|-------|
| `mode` | `sparkles`, `grid`, `video` | `sparkles` = interactive 3D |
| `background` | hex color (URL-encoded) | `%230a0a0a` = dark bg |
| `color` | hex color (URL-encoded) | UI accent color |
| `showTitle` | `true` / `false` | Show/hide Luma branding |
| `loadBg` | `true` / `false` | Show loading background |

## SuperSplat Viewer (Self-hosted .splat files)

If you export a `.splat` file from Luma and want to self-host:

```html
<!-- Via PlayCanvas SuperSplat CDN -->
<iframe
  src="https://playcanv.as/e/YOUR_SUPERSPLAT_SCENE_ID/"
  width="100%"
  height="500"
  frameborder="0"
  allowfullscreen
></iframe>
```

GitHub: https://github.com/playcanvas/supersplat

## Responsive Full-Width Wrapper

```html
<div style="position:relative; width:100%; aspect-ratio:16/9; overflow:hidden;">
  <iframe
    src="https://lumalabs.ai/embed/YOUR_SCENE_ID?mode=sparkles"
    style="position:absolute; inset:0; width:100%; height:100%; border:none;"
    allowfullscreen
  ></iframe>
</div>
```
