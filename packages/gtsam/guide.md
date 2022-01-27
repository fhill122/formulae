```bash
git clone https://github.com/borglab/gtsam.git
cd gtsam
git checkout 4.1.1
mkdir build
mkdir install
cd build
cmake -G Ninja -DCMAKE_INSTALL_PREFIX=../install -DGTSAM_USE_SYSTEM_EIGEN=ON -DGTSAM_BUILD_WITH_MARCH_NATIVE=OFF -DGTSAM_WITH_TBB=OFF ..
ninja install
```

