# This Repo is Under construction!
MSCN<sub>NS</sub> (Multi-scale Sub-pixel Convolutional Network with a Neighborhood Smoothness constraint) is a CNN-based approach for monocular depth estimation.

For technical details, please see the paper (comming soon).

## Prerequisites
* matlab R2017a (or other proper version)
* python v3.5.x
* pytorch v0.3.0 (or later version)
* numpy
* scipy

## How to test

### Quick test

You may use the provided model (comming soon) and test samples to test this apporach as follows,

```python3 test.py --model <the pytorch model> --image ./test_samples/nyu_v2_175.mat```

### Test on the whole NYU Depth v2 dataset.

1. Download [The Dataset](https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html) and [The Train/Test Split file](https://cs.nyu.edu/~silberman/projects/indoor_scene_seg_sup.html).
2. Suppose you have saved the dataset in <path_to_data> and the split file in <path_to_split>. Open ```matlab/gen_test_data_for_mscn.m``` and assign <path_to_data> to 'NYUv2_data' and <path_to_split> to 'split_file'.
3. run ```matlab/gen_test_data_for_mscn.m``` and the test data will be generated in '../Dataset/test'. You may change the save root 'test_root' to anywhere you like.
4. Test the model as follows,

```python3 test.py --model <the pytorch model> --data <path to the generated test data>```

## Results
// TODO
