# Large Pose 3D Face Reconstruction from a Single Image via Direct Volumetric Regression

*Aaron S. Jackson, Adrian Bulat, Vasileios Argyriou and Georgios Tzimiropoulos*

*Try out the code without running it!* Check out our online demo [here](http://www.cs.nott.ac.uk/~psxasj/3dme/).

![image](http://ntustcgalgit.synology.me:30000/B10415042/PytorchVRN/raw/master/vrn.png)

Please visit our [project webpage](http://aaronsplace.co.uk/papers/jackson2017recon/) for a link to the paper and an
example video run on 300VW. This code is licenses under the MIT
License, as described in the LICENSE file.

This is an unguided version of the Volumetric Regression Network (VRN)
for 3D face reconstruction from a single image. This method approaches
the problem of reconstruction as a segmentation problem, producing a
3D volume, spatially aligned with the input image. A mesh can then be
obtained by taking the isosurface of this volume.

Several example images are included in the examples folder. Most of
these are AFLW images taken from [3DDFA](http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/main.htm).

If you are running the code to calculate error for a potential
publication, please use the MATLAB version, as this is what was used
to compute the error for the paper.


## Software Requirements

* Python 3.6.7+
* pytorch 0.4.1+(it may not work with other versions, ans you can get old version pytorch in [here](https://pytorch.org/get-started/previous-versions/#via-pip))
* cuda 9.0+

### python Library

* matplotlib
* scipy
* numpy
* opencv
* dlib
* skimage

```
pip install numpy matplotlib scipy opencv-python dlib skimage

```


## Getting Started

### Running with Python

```
#python demo.py --image inputImagePath --obj outputObjPath
python .\demo.py --image .\examples\AFLW_image00046.jpg --obj .\examples\AFLW_image00046.obj

```

## Acknowledgements
* [2D and 3D Face alignment library build using pytorch](https://github.com/1adrianb/face-alignment)
* [Large Pose 3D Face Reconstruction from a Single Image via Direct Volumetric Regression ](https://github.com/AaronJackson/vrn)
