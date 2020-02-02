# my orbslam2
改成适合自己的文件组织结构，代码风格。

以其为框架学习slam。
# 库版本
eigen3.2
opencv3.4


## 运行单目
### TUM
    ./bin/examples/monocular/mono_tum Vocabulary/ORBvoc.bin Examples/Monocular/TUM1.yaml ~/G-ORBSLAM/data/rgbd_dataset_freiburg1_desk/

### EuRoC
./bin/examples/monocular/mono_euroc Vocabulary/ORBvoc.bin Examples/Monocular/EuRoC.yaml ~/G-ORBSLAM/data/euroc/mav0/cam0/data Examples/Monocular/EuRoC_TimeStamps/V201.txt