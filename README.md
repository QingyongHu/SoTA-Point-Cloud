# Deep Learning for 3D Point Clouds: A Survey

[Yulan Guo<sup>∗</sup>](http://yulanguo.me/), 
[Hanyun Wang<sup>∗</sup>](https://scholar.google.com.hk/citations?user=QG3LdUcAAAAJ&hl=zh-CN), 
[Qingyong Hu<sup>∗</sup>](https://qingyonghu.github.io/), Hao Liu<sup>∗</sup>,
[Li Liu](http://www.ee.oulu.fi/~lili/LiLiuHomepage.html), 
and [Mohammed Bennamoun](http://staffhome.ecm.uwa.edu.au/~00051632/). 



## Introduction
We present a comprehensive review of recent progress in deep learning methods for point clouds. Please see our [arXiv tech report](https://arxiv.org/abs/1912.12033).

This repository provides the **comparative results** of existing methods on several publicly benchmarks. 
It covers three major tasks, including 3D shape classification, 3D object detection, and 3D point cloud segmentation. 
Please feel free to <a href="mailto:qingyong.hu@cs.ox.ac.uk">contact me</a> 
or [create an issue](https://help.github.com/en/github/managing-your-work-on-github/creating-an-issue) on this page if you have new results to add or any suggestions! 

**Note:** 
- We will update this page on a regular basis! So stay tuned~ :tada::tada::tada:


## (1) 3D Shape Classification
### Public Datasets
- ModelNet (CVPR'15) [[paper]](http://3dvision.princeton.edu/projects/2014/3DShapeNets/paper.pdf) [[project page]](http://modelnet.cs.princeton.edu/)
    - ModelNet10 [[data]](http://3dvision.princeton.edu/projects/2014/3DShapeNets/ModelNet10.zip) [[results]](http://modelnet.cs.princeton.edu/) 
    - ModelNet40 [[data]](http://modelnet.cs.princeton.edu/ModelNet40.zip) [[results]](http://modelnet.cs.princeton.edu/) 
- PartNet (CVPR'19) [[paper]](https://arxiv.org/abs/1812.02713) [[data]](https://github.com/daerduoCarey/partnet_dataset) [[project page]](https://cs.stanford.edu/~kaichun/partnet/)
- ScanObjectNN (ICCV'19) [[paper]](https://arxiv.org/pdf/1908.04616.pdf) [[data]](https://github.com/hkust-vgd/scanobjectnn) [[project page]](https://hkust-vgd.github.io/scanobjectnn/)

### Benchmark Results
<p align="center"> <img src="./classification.png" width="95%"> </p>

## (2) 3D Object Detection
### Public Datasets
- KITTI (CVPR'12) [[paper]](http://www.cvlibs.net/publications/Geiger2012CVPR.pdf) [[project page]](http://www.cvlibs.net/datasets/kitti/eval_3dobject.php)
    - _3D objecct detection_ [[data]](http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=3d) [[results]](http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=3d)
    - _BEV_ [[data]](http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=bev) [[results]](http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=bev)
- ApolloScape (TPAMI'19) [[paper]](http://ad-apolloscape.bj.bcebos.com/public%2FApolloScape%20Dataset.pdf) [[data]](http://apolloscape.auto/tracking.html#to_data_href) [[results]](http://apolloscape.auto/leader_board.html)
- Argoverse (CVPR'19) [[paper]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_Argoverse_3D_Tracking_and_Forecasting_With_Rich_Maps_CVPR_2019_paper.pdf) [[data]](https://www.argoverse.org/data.html#download-link) [[project page]](https://www.argoverse.org/index.html)
- A*3D (arXiv'19) [[paper]](https://arxiv.org/pdf/1909.07541) [[data]](https://github.com/I2RDL2/ASTAR-3D#Download) [[project page]](https://github.com/I2RDL2/ASTAR-3D)
- Waymo (arXiv'19) [[paper]](https://arxiv.org/pdf/1912.04838) [[data]](https://waymo.com/open/licensing/) [[project page]](https://waymo.com/open/)

### Benchmark Results
<p align="center"> <img src="./detection.png" width="95%"> </p>
<p align="center"> <img src="./detection_bev.png" width="95%"> </p>


## (3) 3D Point Cloud Segmentation
### Public Datasets
- Semantic3D (ISPRS'17) [[paper]](https://www.ethz.ch/content/dam/ethz/special-interest/baug/igp/photogrammetry-remote-sensing-dam/documents/pdf/Papers/Hackel-etal-cmrt2017.pdf) [[project page]](http://www.semantic3d.net/)
    - _semantic-8_ [[data]](http://www.semantic3d.net/view_dbase.php?chl=1#download) [[results]](http://www.semantic3d.net/view_results.php?chl=1)
    - _reduced-8_ [[data]](http://www.semantic3d.net/view_dbase.php?chl=2#download) [[results]](http://www.semantic3d.net/view_results.php?chl=2)
- S3DIS (CVPR'17) [[paper]](http://buildingparser.stanford.edu/images/3D_Semantic_Parsing.pdf) [[data]](https://docs.google.com/forms/d/e/1FAIpQLScDimvNMCGhy_rmBA2gHfDu3naktRm6A8BPwAWWDv-Uhm6Shw/viewform?c=0&w=1) [[project page]](http://buildingparser.stanford.edu/dataset.html#Download)
- ScanNet (CVPR'17) [[paper]](https://arxiv.org/pdf/1702.04405) [[data]](https://github.com/ScanNet/ScanNet) [[project page]](http://www.scan-net.org/) [[results]](http://kaldir.vc.in.tum.de/scannet_benchmark/)  
- NPM3D (IJRR'18) [[paper]](https://arxiv.org/pdf/1712.00032) [[data]](https://cloud.mines-paristech.fr/index.php/s/JhIxgyt0ALgRZ1O) [[project page]](http://npm3d.fr/) [[results]](http://npm3d.fr/paris-lille-3d) 
- SemanticKITTI (ICCV'19) [[paper]](https://arxiv.org/pdf/1904.01416) [[data]](http://semantic-kitti.org/dataset.html#download) [[project page]](http://semantic-kitti.org/index.html) [[results]](https://competitions.codalab.org/competitions/20331#results)

### Benchmark Results
<p align="center"> <img src="./Segmentation.png" width="95%"> </p>


### Citation
If you find our work useful in your research, please consider citing:

    @article{guo2019deep,
      title={Deep Learning for 3D Point Clouds: A Survey},
      author={Guo, Yulan and Wang, Hanyun and Hu, Qingyong and Liu, Hao and Liu, Li and Bennamoun, Mohammed},
      journal={arXiv preprint arXiv:1912.12033},
      year={2019}
    }


## Updates
* 26/02/2020: Adding the dataset information
* 27/12/2019: Initial release.
