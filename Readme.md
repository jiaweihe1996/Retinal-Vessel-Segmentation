# UNet for Retina Blood Vessel Segmentation


安装依赖库：
```
pip install -r requirements.txt
```

需要将数据文件夹改名为DRIVE，并按下面结构存放数据：

```
DRIVE
│
└───test
|    ├───1st_manual
|    └───2nd_manual
|    └───images
|    └───mask
│
└───training
    ├───1st_manual
    └───images
    └───mask
```
数据预处理：
```
python prepare_datasets_DRIVE.py
```
训练：
```
python run_training.py
```
测试，测试结果在test文件夹下：
```
python run_testing.py
```

