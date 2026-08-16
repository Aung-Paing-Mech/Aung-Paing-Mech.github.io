# APP Portfolio — GitHub Pages Upload Package

This folder is ready to upload to your GitHub repository. Upload **everything inside this folder** to the top level of the repository, keeping both `index.html` and the `assets` folder.

| Item | What to do |
| --- | --- |
| `index.html` | Keep this file name exactly. GitHub Pages opens it automatically as the home page. |
| `assets/` | Upload the entire folder without changing its name. It contains an offline fallback copy of every portfolio photo. |
| Public image URLs | Leave the full `https://files.manuscdn.com/...` URLs in the HTML unchanged. They are the primary image sources. |

The page is protected in two ways. It first loads the permanent public image links. If an image cannot load, the embedded JavaScript automatically uses the matching local file from the `assets/` folder. This prevents the missing-image problem when the complete folder is uploaded together.

## GitHub Pages steps

1. In your GitHub repository, upload all files from this folder to the repository root.
2. Commit the files.
3. Open **Settings → Pages** in the repository.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select your `main` branch and the **/(root)** folder, then save.
6. Wait a few minutes for GitHub to provide your website address.

## Editing text or a photo

Open `index.html` with Notepad or Visual Studio Code. The page contains comments beside the key image areas. To replace a photo safely, put the new photo in `assets/`, update the image `src` to a permanent public URL if available, and update its `data-fallback` value to the new file inside `assets/`.
