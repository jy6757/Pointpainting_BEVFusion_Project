# Pointpainting_Visualize


Naively implementing PointPainting and Visualizing PointPainting

#### Image segmentation & Point cloud projection on 2d image
![projection](https://github.com/jy6757/Pointpainting_Visualize/assets/143304578/2ecc5781-f46f-4724-9b59-929e475a65e0)

#### Pointclout segmentation
![front](https://github.com/jy6757/Pointpainting_Visualize/assets/143304578/d6b771dd-7635-4d3f-87f0-2a1088c50e54)
![lidarpainting](https://github.com/jy6757/Pointpainting_Visualize/assets/143304578/288ffe95-634d-4437-997d-5948ceb043ee)

#### Extract pointcloud by class
![Untitled](https://github.com/jy6757/Pointpainting_Visualize/assets/143304578/b4b81741-f419-4086-98e5-078459314190)

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



