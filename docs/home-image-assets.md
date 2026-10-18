# Responsive home artwork

Generated with the built-in image generation tool from `assets/breezyhome.png`.
The original asset is retained. Generated artwork is visually similar, not pixel-identical.

- `assets/breezyhome-background.png`: scenery with the embedded logo removed.
- `assets/breezy-logo.png`: transparent purple logo silhouette, displayed white via CSS `brightness(0) invert(1)`. Purple extraction avoided artifacts from white foreground transparency processing.

## Final background prompt

Use case: precise-object-edit. Edit target: original Breezy game home background. Remove ONLY the white breezy! logo, its smile arc and decorative dots from the top-center sky. Fill that area with the exact uniform blue sky already surrounding it. Preserve ALL other artwork, tree shapes, clouds, butterfly, flowers, rocks, animals, colors, layout and framing unchanged. No other edits, no text, no logo, no new objects. Preserve original image aspect ratio 20:13. Production game scenery background.

## Final logo prompt

Create exact isolated cutout of the 'breezy!' logo and curved smile from reference. Recolor the entire white mark to SOLID DARK PURPLE #502080, preserving exact shapes, letter arrangement, tilted letters and smile swoosh; all holes and spaces transparent. Flat vector-style solid color, absolutely smooth crisp edges with no texture. Output only purple logo on actual transparent background. No scenery. Entire mark comfortably fits centered with 5% padding in wide 3:1 canvas. IMPORTANT solid DARK PURPLE foreground, not white. This asset will be recolored white via CSS in a website.

## Layout and validation

The scenery covers the viewport. The logo is a separate image, centered with a width bounded by both viewport width and height; portrait mode moves it below the header controls. UI sizing uses the smaller viewport dimension, with minimum sizes on the main buttons.

Chromium checks passed at 1440×825, 1912×987, 2560×1080, 1024×768, 375×812, and 812×375, including resizing the same page. Verified full viewport coverage, logo bounds and separation from Play, no horizontal overflow, and opening How to Play. No JavaScript page errors. Safari was not separately tested.
