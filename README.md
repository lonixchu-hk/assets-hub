# Assets Hub

This repository is designed as a central hub for storing and managing various digital assets. It can be used for a variety of resources, including but not limited to website assets, design files, documents, and other development-related content. The assets can be accessed and shared across different projects, providing a unified source of truth.

## 📌 How to Use

### 1. Upload Assets:

- Create a corresponding folder in the repository based on the type of asset (e.g., `website-assets/`, `design-files/`, `documentation/`).
- Upload your files (e.g., images, design files, markdown documents, API configuration files).

### 2. Enable GitHub Pages (Optional for Static Assets):

- Go to the GitHub repository **Settings** > **Pages**.
- Set `main` (or your primary branch) as the GitHub Pages source to serve static assets like images.
- Configure a custom domain if you have one.

### 3. Get Asset URL (For Static Assets):

- After uploading, access the asset via the following URL format:
  ```
  https://your-custom-domain.com/path/to/asset.jpg
  ```
- Example:
  ```
  https://llpzone.com/website-assets/example.jpg
  ```

### 4. Embed Assets:

- Use the asset in your webpage or Markdown as follows:
  ```md
  ![Asset Description](https://llpzone.com/website-assets/example.jpg)
  ```

## 🚀 Advanced Settings

### Disable Jekyll Processing

- If some assets do not load properly, create a `.nojekyll` file in the repository root to prevent GitHub from applying Jekyll rules, which can interfere with file names or folders starting with an underscore (`_`).

### Use CDN for Faster Loading (Optional)

- You may use Cloudflare or another CDN to speed up asset delivery, particularly for static assets like images and stylesheets.

## 💡 Notes

- Avoid uploading large assets (e.g., videos, large design files) to GitHub; use Git LFS (Large File Storage) or another storage solution.
- GitHub Pages has bandwidth limitations and is not suitable for high-traffic websites or large-scale asset storage.

---

📢 **Welcome to LLP Zone Asset Hub! Store, manage, and share your digital assets in one place!**
