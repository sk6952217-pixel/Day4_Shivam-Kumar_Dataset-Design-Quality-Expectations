#  Dataset Design & Quality Expectations

## Dataset Schema / Structure Note

### Project
Underwater Image Enhancement

### Dataset Type
Paired image-to-image dataset.

Each input image should have a corresponding target image showing the desired enhanced/clear version of the same scene.

### Expected Data

Input:
- Low-quality/degraded underwater image
- PNG/JPG image format
- RGB image
- Same scene as the target image

Target:
- Corresponding enhanced/clear underwater image
- PNG/JPG image format
- RGB image
- Same scene as the input image

### Expected Folder Structure

```text
Dataset/
├── train/
│   ├── input/
│   └── target/
├── val/
│   ├── input/
│   └── target/
└── test/
    ├── input/
    └── target/
```

### Pairing Rule

Every input image must have exactly one correct target image.

The input and target must represent the same underwater scene.

Image filename or image ID can be used for initial pairing, but visual checking is required because the same ID does not always guarantee a correct pair.

### Important Metadata

The following information should be recorded where available:

- Image filename
- Image ID
- Dataset/epoch folder
- Image width and height
- Image format
- Input/target type
- Train/validation/test split
