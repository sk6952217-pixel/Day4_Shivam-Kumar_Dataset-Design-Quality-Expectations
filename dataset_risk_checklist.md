## Dataset Quality Risks

### 1. Incorrect Pairing
An input image may be matched with the wrong target image.

### 2. Missing Images
Some input images may not have a corresponding target.

### 3. Duplicate Images
Duplicate or copied images can appear in the dataset.

### 4. Image Quality
Very dark, low-contrast or heavily degraded images may be difficult to process.

### 5. Data Imbalance
Some types of underwater scenes may occur much more frequently than others.

### 6. Data Leakage
Very similar or duplicate images should not appear in both training and test sets.

### 7. Split Leakage
Input and its corresponding target must remain in the same split.

### 8. Different Image Sizes
Images may have different resolutions and should be standardized during preprocessing.

### 9. Incorrect Targets
A target image may not actually correspond to its input image.

### 10. Limited Dataset
A limited number of correctly paired images may reduce model generalization.

## Train / Validation / Test Split

The split should preserve:

- Correct input-target pairs
- Similar scene distribution
- No duplicate images across splits
- No input-target leakage across splits
- Fixed test set for final evaluation

Training set:
Used for model learning.

Validation set:
Used for model checking and parameter tuning.

Test set:
Used only for final evaluation.

## Dataset Risk Checklist

- All input images have a target image

- Input-target pairs represent the same scene

- Incorrect pairs are removed

- Duplicate images are checked

- Missing images are checked

- Image dimensions are checked

- Image format is checked

- RGB channels are consistent

- Train/validation/test leakage is checked

- Input-target pairs stay in the same split

- Test set is kept fixed

- Dataset preprocessing is applied consistently

- Very dark and difficult images are identified

- Dataset limitations are documented

## Conclusion

The main dataset requirement is to maintain correctly matched input-target pairs. Dataset quality, pairing correctness
