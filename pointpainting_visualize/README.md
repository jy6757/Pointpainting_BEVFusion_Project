# Pointpainting_Visualize


Naively implementing PointPainting and Visualizing PointPainting

#### Image segmentation & Point cloud projection on 2d image
![projection](https://github.com/jy6757/Pointpainting_BEVFusion_Project/assets/143304578/63df92f0-cb43-4095-a6fa-7b32a9229729)

#### Pointclout segmentation
![point seg](https://github.com/jy6757/Pointpainting_BEVFusion_Project/assets/143304578/9cd2a30d-868b-4a23-a23c-7f804c7f6f31)

#### Extract pointcloud by class
![class](https://github.com/jy6757/Pointpainting_BEVFusion_Project/assets/143304578/ecff44f8-dbe1-4696-9651-cb956d6e8c91)

---

## Installation
mmsegmentation install


https://mmsegmentation.readthedocs.io/en/latest/get_started.html

```
cuda 11.7
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117
pip install opencv-python==4.8.0.76
```

## checkpoint download
```
!wget https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes/pspnet_r50-d8_512x1024_40k_cityscapes_20200605_003338-2966598c.pth -P checkpoint
```

## run instruction
```
python pointpainting.py
```

## data file structure(KITTI Dataset)
```
training
├── calid
├── image_2
├── label_2
├──velodyne
```



