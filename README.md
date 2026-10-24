# Awesome-Web-Photo-Editing-Software

## Top Web Photo Editing Software Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Browser-Native Editing, Self-Hosted Privacy & Layer-Based Non-Destructive Workflows*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Web Photo Editing Software**. These tools run in the browser to edit raster images — layers, masks, selections, filters, and color correction — without installing desktop software or uploading originals to a stranger's server.

**Examples** include miniPaint, BitMappery, OpenShop, Photopea, Pixlr, and Canva (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, offline-capable browser editing, and transparent data handling — ideal for users who want Photoshop-class layer editing without a subscription, and developers who need an embeddable editor that never phones home.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Photopea** — **The most capable browser-based Photoshop clone.** Free with side advertisements; paid tier (around $5/month) removes ads. **Opens native .psd files directly** with full layer, mask, and smart object support, making it the fastest way to edit a Photoshop file without Photoshop installed [citation:1][citation:6]. **Crammed full of functionality** — users report it handles everything needed for image editing and artwork preparation [citation:1]. **Trade-offs**: **interface is complex for beginners** [citation:13]; **not all .psd files work perfectly** [citation:1]; **requires an internet connection** to use [citation:1]. **Best for users who need Photoshop compatibility in a browser** without installing anything.

- **Pixlr E** — **The modern, AI-assisted browser editor.** Free tier with limitations; paid plans from around $5/month. **Cleaner and faster than Photopea for simple tasks**, with AI-powered background removal, generation, and upscaling [citation:13]. **Trade-offs**: **limited features in the free tier** and **advertisements** [citation:13]. **Best for quick edits** where speed matters more than deep layer control.

- **Canva** — **The template-first design platform.** Free tier with paid Pro. **Ultra-simple editing with one-click AI tools** (Magic Eraser, background removal, auto-correction) [citation:13]. **Trade-offs**: **no real layer system** and **basic retouching capability** compared to dedicated editors [citation:13]. **Best for social media graphics** rather than serious photo editing.

## Open-Source GitHub Projects

- **miniPaint** — **The lightweight, self-hostable browser editor that covers most Photoshop use cases.** MIT licensed [citation:4]. **Runs entirely in the browser** — nothing is sent to any server, and it works offline after initial load via service workers [citation:2][citation:4]. **Layer-based non-destructive editing** with multi-layer support, differences, merging, and flattening [citation:4]. **Broad format support**: PNG, JPG, BMP, WebP, animated GIF, TIFF, and **JSON layer data export** for future edits [citation:4]. **Filters include** box/gaussian/zoom blur, denoise, oil painting, solarize, vignette, vibrance, and Instagram-style presets [citation:4]. **Tools include** pencil, brush, magic wand, eraser, fill, clone, crop, text, and content fill [citation:4]. **The honest limitation**: **selection tools are basic** — only rectangle selection, no lasso or magnetic selection — and **masking requires menu navigation** rather than right-click workflows [citation:2]. **No smart objects or perspective editing** [citation:2]. **Best for self-hosting and privacy** — everything stays local, no account needed, and the code is auditable.

- **BitMappery** — **The self-hosted editor with non-destructive layers and a minimal interface.** Free, open-source, **runnable in the browser or self-hosted via Docker** [citation:11]. **Non-destructive layer-based system** — adjustments live on their own layers, so you can toggle visibility, reorder, or re-tweak without losing earlier work [citation:11]. **Comprehensive text tool** with a large font selection, which many lightweight editors neglect [citation:11]. **Selection tools include** rectangle, **polygonal lasso** (accurate for detailed masks), and magic wand [citation:11]. **The trade-off**: **watered-down effects toolkit** compared to Photoshop — essentially one adjustment window with color/tone controls, filter (duotone), opacity, and blend mode [citation:11]. **Best for users wanting non-destructive editing** in a self-hosted package with better selection tools than miniPaint.

- **OpenShop** — **The most feature-complete open-source browser editor for layered work and PSD interchange.** Free, open-source, **no account, no editing server, no telemetry** [citation:10]. **Layers are real working structure** — nested groups, raster masks, adjustment layers, editable vectors, **embedded Smart Objects**, and editable text survive in the native project format [citation:10]. **34 editing tools** including brush presets, imported ABR tips, clone stamp, healing, dodge, burn, smudge, and symmetry modes [citation:10]. **Precise selections**: marquee, lasso, **magnetic lasso**, Quick Selection, Magic Wand, Color Range, Refine Edge, feathering, and pixel masks [citation:10]. **Format support is exceptional**: imports PSD, OpenRaster, PDF, camera RAW, HEIC, JPEG XL, AVIF, and SVG; exports PNG, JPEG, WebP, AVIF, SVG, PDF, PSD, and OpenRaster [citation:10]. **Optional local AI models** run in the browser after download — background removal, depth maps, object detection, click-guided segmentation, and 2x/4x enlargement [citation:10]. **Portable**: works as a single HTML file or installable PWA with offline shell [citation:10]. **Best for users wanting the most complete open-source Photoshop alternative** with real PSD interchange and smart objects.

- **Graphite** — **The node-based procedural 2D design suite.** Apache 2.0 licensed, **runs in the browser via Rust and WebAssembly** with GPU acceleration through wgpu [citation:3]. **Node graph at its core** — every action is a composable node, making edits non-destructive in a way that goes beyond simple undo history [citation:3]. **Layer panel works like traditional tools** if you ignore the node graph, so the learning curve is optional [citation:3]. **Long-term roadmap** includes raster editing, digital painting, desktop publishing, motion graphics, animation, and compositing — aiming to be the "2D counterpart to Blender" [citation:3]. **The honest caveat**: **current alpha is primarily vector-focused** — raster import for JPEG/PNG/PSD is not yet available, and animation is not yet implemented [citation:14]. **Best for designers wanting a procedural, future-proof workflow** who can wait for raster and animation features.

- **MirrorLab** — **The Lightroom-style RAW editor in the browser.** MIT licensed. **RAW file support** for .CR2, .NEF, .ARW, .DNG, and others directly in the browser [citation:12]. **Advanced tone curve** with multi-channel (Master, Red, Green, Blue), precise numeric inputs, and spline-based interpolation [citation:12]. **Comprehensive color tools**: HSL/Color Mixer for 8 channels, exposure/contrast/highlights/shadows/whites/blacks, and white balance [citation:12]. **Client-side processing** — images never leave your device [citation:12]. **The caveat**: **roadmap items** include full RAW decoding via libraw (currently preview extraction only), masking tools, and AI-based subject selection — these are planned, not shipped [citation:12]. **Best for photographers** wanting RAW editing in the browser without Lightroom's subscription.

### Additional Strong Open-Source Options

- **PixelForge** — Vanilla TypeScript browser editor with layers, tools, filters, tabbed projects, and export. Apache 2.0 licensed [citation:8]. Best for developers wanting a clean, framework-free TypeScript codebase to extend.
- **OpenShop** — Already listed above; notable for its single-HTML-file portability and PSD smart object support [citation:10].

**Frameworks for building custom systems**: Combine **miniPaint** for lightweight self-hosted editing with offline capability, **OpenShop** for the most complete PSD-compatible layer editing with smart objects and local AI, **BitMappery** for non-destructive layers with polygonal lasso selection, **Graphite** for procedural node-based design (vector-first), and **MirrorLab** for RAW photo processing in the browser — to build a web photo editing stack tailored to your need for privacy, Photoshop compatibility, or RAW workflows.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Web photo editors differ significantly in layer depth, PSD compatibility, and self-hosting capability. **Photopea is the most capable free browser editor** for .psd files but shows ads and requires internet [citation:1][citation:6]. **miniPaint is the most privacy-focused** — nothing leaves the browser and it works offline — but its selection tools are basic (no lasso) and it lacks smart objects [citation:2][citation:4]. **OpenShop is the most feature-complete open-source option** with PSD smart objects, magnetic lasso, and local AI models, but it is newer and less battle-tested [citation:10]. **Graphite is vector-first in its current alpha** — raster import and animation are roadmap items, not shipped features [citation:14]. **MirrorLab's full RAW decoding is planned but not yet implemented** — current RAW support uses embedded previews [citation:12]. **No open-source browser editor matches Photopea's Photoshop compatibility today**, but OpenShop comes closest for layered PSD work.
- Self-hosted open-source solutions require proper Docker deployment (BitMappery), static file serving (miniPaint, OpenShop), and awareness that browser-based editors are limited by available RAM for very large images.

---

**Made for designers, photographers, and developers choosing browser-based photo editing tools they can own and control.**
Let's make web photo editing more open, self-hostable, and subscription-free.
