---
description: How to add a new game review with cover image
---

# Adding a New Game Review

## Steps

### 1. Create the Review File
Create a new markdown file in `titles/` directory:
```
titles/[game_name_lowercase_underscores].md
```

### 2. Generate Cover Image
Ask to generate a cover image for the game:
```
"Generate cover image for [Game Name]"
```

The image will be saved to `images/[game_name]_cover.png`

### 3. Add Review Template
Use this structure:

```markdown
# [Game Title]

![Game Cover](../images/[game_name]_cover.png)

| |                             |
|--------------------|-----------------------------| 
| Release Date       | [Date]                      |
| Developer          | [Developer]                 |
| Publisher          | [Publisher]                 |
| Genre              | [Genre]                     |
| Status             | [Playing/Completed/On Hold] |
| Time Played        | [X Hours Y Minutes]         |
| Rating             | ★ ★ ★ ★ ☆                 |
| Platform           | [Steam/Epic/etc]            |
| Achievements       | [X/Y or Not Available]      |

## Overview
[Brief overview of the game and your experience]

## Story & Atmosphere
[Story details and game atmosphere]

## Gameplay
[Gameplay mechanics and your thoughts]

## Verdict
[Final verdict and recommendation]
```

### 4. Update Tracking Files
Update the following files:
- `README.md` - Add to appropriate genre section
- `utils/temporal_distribution.md` - Add to Playing Timeline and Time by Title

### 5. Commit Changes
```bash
git add .
git commit -m "Added [Game Name] review"
git push
```
