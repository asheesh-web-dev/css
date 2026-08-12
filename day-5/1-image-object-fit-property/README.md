# Learn img `object-fit` property

The `object-fit` property controls how an image or video resizes to fill its own defined box.

## 💡 The Golden Rule

For `object-fit` to work, you must define both a `width` and a `height` on the `<img>` tag (either in pixels, percentages, or viewport units). [3]

## 🎨 The 5 object-fit Values

- **`fill` (Default)**
- Squeezes or stretches the image to exactly match the target dimensions.
  - Stretches the image, destroying its original aspect ratio.
- **`contain`**
  - Scales the image down or up to fit entirely inside the box.
  - Preserves the aspect ratio, which often leaves empty letterbox spaces.
- **`cover`**
  - Scales the image to completely fill the box, cropping the edges if needed.
  - Preserves the aspect ratio, making it ideal for banners and cards.
- **`none`**
  - Ignores the box dimensions completely and displays the image at its original size.
  - Overflows or crops heavily without any scaling. [10, 11, 12]
- **`scale-down`**
  - Compares none and contain automatically behind the scenes.
  - Selects whichever option results in the smaller final image size.

---
