# nuScenes-converter
Using nuScenes with detectron2 

## For what
Detectron2 doesn't support nuScence annotation out of the box. To use this dataset, you must transform annotation to the dictionary (see dict format [here](https://detectron2.readthedocs.io/tutorials/datasets.html)). This package does it for you. Also you can use it like 3b-box to 2d-bbox translator.

## Requirements
- Python ≥ 3.6
- PyTorch ≥ 1.4
- OpenCV
- [detectron2](https://github.com/facebookresearch/detectron2)
- [nuScenes devkit](https://github.com/nutonomy/nuscenes-devkit/tree/master) 
- [nuScenes](https://www.nuscenes.org/), demo use mini version

## Installation
```
git clone https://github.com/tdtce/nuScenes-converter.git
cd nuScenes-converter
pip install -e .
```

## Using example
Using example see [here](https://github.com/tdtce/nuScenes-converter/blob/master/nuscenes_with_detectron2.ipynb).
For import use:
```
from nusc_conv.conv import get_nuscenes_dicts
```

## Plans
- [x] Category support
- [ ] Train test support
