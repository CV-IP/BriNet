# BriNet: Towards Bridging the Intra-class andInter-class Gaps in One-Shot Segmentation
By Xianghui Yang, Bairun Wang, Kaige Chen, Xinchi Zhou, Shuai Yi, Wanli Ouyang, Luping Zhou

## Paper

You can find our paper at https://arxiv.org/abs/205.03410


## Citation

If you find BriNet useful in your research, please consider to cite:

```
 ```

## Training

You will also need to

1) Download/Prepare SBD dataset (http://home.bharathh.info/pubs/codes/SBD/download.html).
2) Download pre-trained ResNet50 from pytorch model zoo.


```shell 
cd BriNet

# if you want to use default setting
python train.py -fold=0

# if you want to use default setting
python train.py -fold=0 -input_size=[353,353] -gpu=0 -checkpoint_dir='./checkpoint'
```

## Testing

Download trained models from: https://google/drive or load your trained model. We assume you have downloaded the repository into ./checkpoint path.

```shell 
cd BriNet

# if you want to use default setting
python test.py -fold=0

# if you want to use default setting
python test.py -fold=0 -input_size=[353,353] -gpu=0 -checkpoint_dir='./checkpoint'
```


## Contact

For further questions, you can leave them as issues in the repository, or contact the authors directly:
xianghui.yang@sydney.edu.au