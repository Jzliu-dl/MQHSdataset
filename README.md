
# Math Expressions Dataset with Handwritten Quadrilateral Datasets

This is an open-source dataset of handwritten mathematical expressions, where each sample is annotated with quadrilateral bounding boxes that represent the boundaries of the expressions, along with additional metadata. The dataset can be used for training and testing mathematical formula recognition, image processing, deep learning, and related tasks.

## Directory Structure

```
Math-Expressions-Dataset/
│
├── README.md                  # This file
├── train_images/              # Folder containing training images
├── test_images/               # Folder containing testing images
├── train_gts/                 # Folder containing ground truth annotations for the training images
├── test_gts/                  # Folder containing ground truth annotations for the test images
├── train_list.txt             # List of training image and annotation pairs
├── test_list.txt              # List of testing image and annotation pairs
└── LICENSE                    # Open-source license
```

## Data Format

Each annotation file in the `train_gts/` and `test_gts/` directories contains several quadrilateral bounding boxes, with the format as follows:

```
25,40,258,15,262,53,30,77,HME
27,89,274,64,279,97,35,129,HME
243,134,336,119,345,168,253,182,HME
120,172,178,164,184,192,127,199,HME
70,131,79,169,254,141,245,105,HME
```

Each line represents one quadrilateral bounding box with coordinates (`x1, y1, x2, y2, x3, y3, x4, y4`), followed by an additional label (e.g., "HME"). These coordinates define the boundaries of the mathematical expressions in the image.

## Dataset Statistics

The dataset contains the following statistics:

## Dataset Statistics

The statistics of the self-collected dataset are as follows:

| Index                           | Value             |
|---------------------------------|-------------------|
| Number of samples               | 798               |
| Number of expressions           | 3012              |
| Number of overlapping expressions | 1368             |
| Mean aspect ratio of expressions | 3.72              |
| Max aspect ratio of expressions  | 24.56             |
| Mean distance between expressions | 1.52 pixels      |

## Usage

### Cloning the Repository

To use the dataset, you can clone the repository:

```bash
git clone https://github.com/Jzliu-dl/MQHSdatabase.git
```

### Data Overview

- The images are stored in the `train_images/` and `test_images/` directories.
- The ground truth annotations are stored in the `train_gts/` and `test_gts/` directories.
- The `train_list.txt` and `test_list.txt` files contain pairs of image filenames.



## Contributions

We welcome contributions to this dataset, including new data samples or enhancements to the existing set. If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Add new images and annotations to your fork.
3. Submit a pull request.

Before submitting, please ensure your data follows the same format as the existing dataset.

## License

This dataset is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the contents of this repository, provided you comply with the terms of the license.

## Contact Us

If you have any questions or suggestions, or if you would like to discuss the usage of the dataset, feel free to contact us via GitHub Issues.
