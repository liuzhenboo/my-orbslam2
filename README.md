# my orbslam2
改成适合自己的文件组织结构，代码风格。

以其为框架学习slam。
# 库版本
eigen3.2
opencv3.4



## 单目
### TUM
./bin/examples/monocular/mono_tum Vocabulary/ORBvoc.bin Examples/Monocular/TUM1.yaml ~/G-ORBSLAM/data/rgbd_dataset_freiburg1_desk/

### EuRoC
./bin/examples/monocular/mono_euroc Vocabulary/ORBvoc.bin Examples/Monocular/EuRoC.yaml ~/G-ORBSLAM/data/euroc/mav0/cam0/data Examples/Monocular/EuRoC_TimeStamps/V201.txt

## 双目
## EuRoc
./bin/examples/stereo/stereo_euroc Vocabulary/ORBvoc.bin Examples/Stereo/EuRoC.yaml ~/G-ORBSLAM/data/euroc/mav0/cam0/data ~/G-ORBSLAM/data/euroc/mav0/cam1/data Examples/Stereo/EuRoC_TimeStamps/V201.txt

## RGBD

### tips
Associate RGB images and depth images using the python script [associate.py](http://vision.in.tum.de/data/datasets/rgbd-dataset/tools),we also have download this file to the scripts fold. We already provide associations for some of the sequences in *Examples/RGB-D/associations/*. You can generate your own associations file executing:

  ```
  python associate.py PATH_TO_SEQUENCE/rgb.txt PATH_TO_SEQUENCE/depth.txt > associations.txt
  ```

./bin/examples/rgbd/rgbd_tum Vocabulary/ORBvoc.bin Examples/RGB-D/TUM1.yaml ~/G-ORBSLAM/data/rgbd_dataset_freiburg1_desk/ ~/G-ORBSLAM/data/rgbd_dataset_freiburg1_desk/associations.txt  