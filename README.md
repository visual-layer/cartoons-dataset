# The Simpsons & Tom & Jerry Dataset

## Overview

This repository contains a curated dataset of visual media inspired by *The Simpsons* and *Tom & Jerry*. It is intended for **educational and tutorial purposes**, such as testing computer vision workflows, experimenting with object detection, or building Quick Start examples.  

**Note:** No copyrighted material from the original shows is included. All images/videos are **created, modified, or sourced from free/open media**.

---

## Contents

The dataset is organized as follows:

dataset/
├── simpsons/
│   ├── images/
│   └── videos/
└── tom_and_jerry/
├── images/
└── videos/

- `images/` — sample frames or artwork  
- `videos/` — short clips for testing video processing  

---

## Example Usage

### Inspect files

```bash
ls dataset/simpsons/images | head -5

Load in Python

from pathlib import Path
from PIL import Image

dataset_path = Path("dataset/simpsons/images")
for img_file in dataset_path.glob("*.jpg"):
    img = Image.open(img_file)
    img.show()
    break

Notes
	•	The dataset is intentionally small for Quick Start/tutorial purposes.
	•	You can replace the contents with your own images/videos while keeping the same structure.

⸻

License

This dataset is released under the CC0 / Public Domain license for educational and tutorial use only.

Users are responsible for complying with any copyright or trademark laws when substituting real media.

⸻

References
	•	Inspired by: The Simpsons and Tom & Jerry franchises
	•	Tutorial use case: Quick Start, computer vision, object detection
