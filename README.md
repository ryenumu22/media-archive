# media-archive

A personal archive for storing images and videos.

## Structure

Organize your media however works best for you. Some ideas:

```
media-archive/
├── photos/
│   ├── 2024/
│   └── 2025/
├── videos/
│   ├── travel/
│   └── events/
└── screenshots/
```

## Adding files

Whenever you add images or videos to the folder, run:

```bash
git add .
git commit -m "add some photos"
git push
```

## Git LFS (for video files)

Large video files will bloat your repo history and GitHub will reject files over 100MB. Set up Git LFS first:

```bash
git lfs install
git lfs track "*.mp4" "*.mov" "*.avi" "*.mkv"
git add .gitattributes
git commit -m "track video files with LFS"
git push
```
