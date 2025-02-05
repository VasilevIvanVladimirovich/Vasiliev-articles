- Required packages
    ```console
    $ sudo apt-get install build-essential cmake pkg-config unzip yasm git checkinstall  # generic tools
    $ sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev  # required
    ```
- Image I/O
    ```console
    $ sudo apt-get install libjpeg-dev libpng-dev libtiff-dev
    ```
- Video and audio
    ```console
    $ sudo apt install libavcodec-dev libavformat-dev libswscale-dev libavresample-dev
    $ sudo apt install libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev
    $ sudo apt install libxvidcore-dev x264 libx264-dev libfaac-dev libmp3lame-dev libtheora-dev 
    $ sudo apt install libfaac-dev libmp3lame-dev libvorbis-dev
    ```
- GTK for OpenCV highghui
    ```console
    $ sudo apt-get install libgtk-3-dev
    ```

- Parallelism C++ for CPU
    ```console
    $ sudo apt-get install libtbb2 libtbb-dev 
    ```

- OpenCV optimization
    ```console
    $ sudo apt-get install libatlas-base-dev gfortran
    ```

- Cudnn
    ```console
    $ sudo apt-get -y install cudnn9-cuda-11
    ```

```console
General configuration for OpenCV 4.10.0 =====================================
  Version control:               unknown

  Extra modules:
    Location (extra):            /home/echo/Загрузки/opencv_cuda_86/opencv_contrib/modules
    Version control (extra):     unknown

  Platform:
    Timestamp:                   2024-09-03T07:38:31Z
    Host:                        Linux 6.8.0-40-generic x86_64
    CMake:                       3.22.1
    CMake generator:             Unix Makefiles
    CMake build tool:            /usr/bin/gmake
    Configuration:               Release

  CPU/HW features:
    Baseline:                    SSE SSE2 SSE3
      requested:                 SSE3
    Dispatched code generation:  SSE4_1 SSE4_2 FP16 AVX AVX2 AVX512_SKX
      requested:                 SSE4_1 SSE4_2 AVX FP16 AVX2 AVX512_SKX
      SSE4_1 (18 files):         + SSSE3 SSE4_1
      SSE4_2 (2 files):          + SSSE3 SSE4_1 POPCNT SSE4_2
      FP16 (1 files):            + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 AVX
      AVX (9 files):             + SSSE3 SSE4_1 POPCNT SSE4_2 AVX
      AVX2 (38 files):           + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2
      AVX512_SKX (8 files):      + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2 AVX_512F AVX512_COMMON AVX512_SKX

  C/C++:
    Built as dynamic libs?:      YES
    C++ standard:                11
    C++ Compiler:                /usr/bin/c++  (ver 10.5.0)
    C++ flags (Release):         -fsigned-char -W -Wall -Wreturn-type -Wnon-virtual-dtor -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -O3 -DNDEBUG  -DNDEBUG
    C++ flags (Debug):           -fsigned-char -W -Wall -Wreturn-type -Wnon-virtual-dtor -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
    C Compiler:                  /usr/bin/cc
    C flags (Release):           -fsigned-char -W -Wall -Wreturn-type -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -O3 -DNDEBUG  -DNDEBUG
    C flags (Debug):             -fsigned-char -W -Wall -Wreturn-type -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -g  -O0 -DDEBUG -D_DEBUG
    Linker flags (Release):      -Wl,--exclude-libs,libippicv.a -Wl,--exclude-libs,libippiw.a   -Wl,--gc-sections -Wl,--as-needed -Wl,--no-undefined  
    Linker flags (Debug):        -Wl,--exclude-libs,libippicv.a -Wl,--exclude-libs,libippiw.a   -Wl,--gc-sections -Wl,--as-needed -Wl,--no-undefined  
    ccache:                      NO
    Precompiled headers:         NO
    Extra dependencies:          m pthread cudart_static dl rt nppc nppial nppicc nppidei nppif nppig nppim nppist nppisu nppitc npps cublas cudnn cufft -L/usr/local/cuda/lib64 -L/usr/lib/x86_64-linux-gnu
    3rdparty dependencies:

  OpenCV modules:
    To be built:                 alphamat aruco bgsegm bioinspired calib3d ccalib core cudaarithm cudabgsegm cudacodec cudafeatures2d cudafilters cudaimgproc cudalegacy cudaobjdetect cudaoptflow cudastereo cudawarping cudev cvv datasets dnn dnn_objdetect dnn_superres dpm face features2d flann freetype fuzzy gapi hdf hfs highgui img_hash imgcodecs imgproc intensity_transform java line_descriptor mcc ml objdetect optflow phase_unwrapping photo plot python3 quality rapid reg rgbd saliency shape signal stereo stitching structured_light superres surface_matching text tracking ts video videoio videostab viz wechat_qrcode xfeatures2d ximgproc xobjdetect xphoto
    Disabled:                    world
    Disabled by dependency:      -
    Unavailable:                 cannops julia matlab ovis python2 sfm
    Applications:                tests perf_tests apps
    Documentation:               NO
    Non-free algorithms:         NO

  GUI:                           QT5
    QT:                          YES (ver 5.15.3 )
      QT OpenGL support:         NO
    GTK+:                        YES (ver 3.24.33)
      GThread :                  YES (ver 2.72.4)
      GtkGlExt:                  NO
    VTK support:                 YES (ver 9.1.0)

  Media I/O: 
    ZLib:                        /usr/lib/x86_64-linux-gnu/libz.so (ver 1.2.11)
    JPEG:                        /usr/lib/x86_64-linux-gnu/libjpeg.so (ver 80)
    WEBP:                        /usr/lib/x86_64-linux-gnu/libwebp.so (ver encoder: 0x020f)
    PNG:                         /usr/lib/x86_64-linux-gnu/libpng.so (ver 1.6.37)
    TIFF:                        /usr/lib/x86_64-linux-gnu/libtiff.so (ver 42 / 4.3.0)
    JPEG 2000:                   OpenJPEG (ver 2.4.0)
    OpenEXR:                     build (ver 2.3.0)
    HDR:                         YES
    SUNRASTER:                   YES
    PXM:                         YES
    PFM:                         YES

  Video I/O:
    DC1394:                      NO
    FFMPEG:                      YES
      avcodec:                   YES (58.134.100)
      avformat:                  YES (58.76.100)
      avutil:                    YES (56.70.100)
      swscale:                   YES (5.9.100)
      avresample:                NO
    GStreamer:                   YES (1.20.3)
    v4l/v4l2:                    YES (linux/videodev2.h)

  Parallel framework:            pthreads

  Trace:                         YES (with Intel ITT)

  Other third-party libraries:
    Intel IPP:                   2021.11.0 [2021.11.0]
           at:                   /home/echo/Загрузки/opencv_cuda_86/opencv_build/3rdparty/ippicv/ippicv_lnx/icv
    Intel IPP IW:                sources (2021.11.0)
              at:                /home/echo/Загрузки/opencv_cuda_86/opencv_build/3rdparty/ippicv/ippicv_lnx/iw
    VA:                          NO
    Lapack:                      NO
    Eigen:                       YES (ver 3.4.0)
    Custom HAL:                  NO
    Protobuf:                    build (3.19.1)
    Flatbuffers:                 builtin/3rdparty (23.5.9)

  NVIDIA CUDA:                   YES (ver 11.8, CUFFT CUBLAS FAST_MATH)
    NVIDIA GPU arch:             86
    NVIDIA PTX archs:            90

  cuDNN:                         YES (ver 9.3.0)

  OpenCL:                        YES (no extra features)
    Include path:                /home/echo/Загрузки/opencv_cuda_86/opencv-4.10.0/3rdparty/include/opencl/1.2
    Link libraries:              Dynamic load

  Python 3:
    Interpreter:                 /usr/bin/python3 (ver 3.10.12)
    Libraries:                   /usr/lib/x86_64-linux-gnu/libpython3.10.so (ver 3.10.12)
    Limited API:                 NO
    numpy:                       /home/echo/.local/lib/python3.10/site-packages/numpy/core/include (ver 1.24.2)
    install path:                lib/python3.10/dist-packages/cv2/python-3.10

  Python (for build):            /usr/bin/python3

  Java:                          
    ant:                         NO
    Java:                        YES (ver 11.0.24)
    JNI:                         /usr/lib/jvm/default-java/include /usr/lib/jvm/default-java/include/linux /usr/lib/jvm/default-java/include
    Java wrappers:               YES (JAVA)
    Java tests:                  NO

  Install to:                    /usr/local
-----------------------------------------------------------------

Configuring done
Generating done
```

```console
General configuration for OpenCV 4.11.0 =====================================
  Version control:               unknown

  Extra modules:
    Location (extra):            /home/echo/work/lib/openVINO/opencv_contrib-4.11.0/modules
    Version control (extra):     unknown

  Platform:
    Timestamp:                   2025-02-05T13:41:05Z
    Host:                        Linux 6.8.0-52-generic x86_64
    CMake:                       3.31.5
    CMake generator:             Unix Makefiles
    CMake build tool:            /usr/bin/gmake
    Configuration:               Release
    Algorithm Hint:              ALGO_HINT_ACCURATE

  CPU/HW features:
    Baseline:                    SSE SSE2 SSE3
      requested:                 SSE3
    Dispatched code generation:  SSE4_1 SSE4_2 AVX FP16 AVX2 AVX512_SKX
      SSE4_1 (18 files):         + SSSE3 SSE4_1
      SSE4_2 (2 files):          + SSSE3 SSE4_1 POPCNT SSE4_2
      AVX (9 files):             + SSSE3 SSE4_1 POPCNT SSE4_2 AVX
      FP16 (1 files):            + SSSE3 SSE4_1 POPCNT SSE4_2 AVX FP16
      AVX2 (38 files):           + SSSE3 SSE4_1 POPCNT SSE4_2 AVX FP16 AVX2 FMA3
      AVX512_SKX (8 files):      + SSSE3 SSE4_1 POPCNT SSE4_2 AVX FP16 AVX2 FMA3 AVX_512F AVX512_COMMON AVX512_SKX

  C/C++:
    Built as dynamic libs?:      YES
    C++ standard:                11
    C++ Compiler:                /usr/bin/c++  (ver 11.4.0)
    C++ flags (Release):         -fsigned-char -W -Wall -Wreturn-type -Wnon-virtual-dtor -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -O3 -DNDEBUG  -DNDEBUG
    C++ flags (Debug):           -fsigned-char -W -Wall -Wreturn-type -Wnon-virtual-dtor -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
    C Compiler:                  /usr/bin/gcc-11
    C flags (Release):           -fsigned-char -W -Wall -Wreturn-type -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse3 -fvisibility=hidden -O3 -DNDEBUG  -DNDEBUG
    C flags (Debug):             -fsigned-char -W -Wall -Wreturn-type -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse3 -fvisibility=hidden -g  -O0 -DDEBUG -D_DEBUG
    Linker flags (Release):      -Wl,--exclude-libs,libippicv.a -Wl,--exclude-libs,libippiw.a   -Wl,--gc-sections -Wl,--as-needed -Wl,--no-undefined  
    Linker flags (Debug):        -Wl,--exclude-libs,libippicv.a -Wl,--exclude-libs,libippiw.a   -Wl,--gc-sections -Wl,--as-needed -Wl,--no-undefined  
    ccache:                      NO
    Precompiled headers:         NO
    Extra dependencies:          m pthread cudart_static dl rt nppc nppial nppicc nppidei nppif nppig nppim nppist nppisu nppitc npps cublas cudnn cufft -L/usr/local/cuda/lib64 -L/usr/lib/x86_64-linux-gnu
    3rdparty dependencies:

  OpenCV modules:
    To be built:                 alphamat aruco bgsegm bioinspired calib3d ccalib core cudaarithm cudabgsegm cudacodec cudafeatures2d cudafilters cudaimgproc cudalegacy cudaobjdetect cudaoptflow cudastereo cudawarping cudev cvv datasets dnn dnn_objdetect dnn_superres dpm face features2d flann freetype fuzzy gapi hdf hfs highgui img_hash imgcodecs imgproc intensity_transform java line_descriptor mcc ml objdetect optflow phase_unwrapping photo plot quality rapid reg rgbd saliency sfm shape signal stereo stitching structured_light superres surface_matching text tracking ts video videoio videostab viz wechat_qrcode xfeatures2d ximgproc xobjdetect xphoto
    Disabled:                    world
    Disabled by dependency:      -
    Unavailable:                 cannops fastcv julia matlab ovis python2 python3
    Applications:                tests perf_tests apps
    Documentation:               NO
    Non-free algorithms:         NO

  GUI:                           QT5
    QT:                          YES (ver 5.15.13 )
      QT OpenGL support:         NO
    GTK+:                        YES (ver 3.24.41)
    VTK support:                 YES (ver 9.1.0)

  Media I/O: 
    ZLib:                        /usr/lib/x86_64-linux-gnu/libz.so (ver 1.3)
    JPEG:                        /usr/lib/x86_64-linux-gnu/libjpeg.so (ver 80)
    WEBP:                        /usr/lib/x86_64-linux-gnu/libwebp.so (ver decoder: 0x0209, encoder: 0x020f, demux: 0x0107)
    AVIF:                        /home/echo/work/lib/anaconda3/lib/libavif.so.15.0.1 (ver 0.11.1)
    PNG:                         libpng (ver 1.6.43)
      SIMD Support Request:      YES
      SIMD Support:              YES (Intel SSE)
    TIFF:                        /usr/lib/x86_64-linux-gnu/libtiff.so (ver 42 / 4.5.1)
    JPEG 2000:                   build (ver 2.5.0)
    OpenEXR:                     build (ver 2.3.0)
    GIF:                         NO
    HDR:                         YES
    SUNRASTER:                   YES
    PXM:                         YES
    PFM:                         YES

  Video I/O:
    FFMPEG:                      YES
      avcodec:                   YES (60.31.102)
      avformat:                  YES (60.16.100)
      avutil:                    YES (58.29.100)
      swscale:                   YES (7.5.100)
      avresample:                NO
    GStreamer:                   YES (1.24.2)
    v4l/v4l2:                    YES (linux/videodev2.h)

  Parallel framework:            pthreads

  Trace:                         YES (with Intel ITT)

  Other third-party libraries:
    Intel IPP:                   2021.12.0 [2021.12.0]
           at:                   /home/echo/work/lib/openVINO/build-opencv-4.11.0/3rdparty/ippicv/ippicv_lnx/icv
    Intel IPP IW:                sources (2021.12.0)
              at:                /home/echo/work/lib/openVINO/build-opencv-4.11.0/3rdparty/ippicv/ippicv_lnx/iw
    VA:                          NO
    Lapack:                      NO
    OpenVINO:                    YES (2024.6.0)
    Eigen:                       YES (ver 3.4.0)
    Custom HAL:                  NO
    Protobuf:                    build (3.19.1)
    Flatbuffers:                 builtin/3rdparty (23.5.9)

  NVIDIA CUDA:                   YES (ver 11.8, CUFFT CUBLAS FAST_MATH)
    NVIDIA GPU arch:             86
    NVIDIA PTX archs:            90

  cuDNN:                         YES (ver 8.9.6)

  OpenCL:                        YES (no extra features)
    Include path:                /home/echo/work/lib/openVINO/opencv-4.11.0/3rdparty/include/opencl/1.2
    Link libraries:              Dynamic load

  ONNX:                          YES
    Include path:                /home/echo/work/lib/openVINO/onnxruntime-1.20.1/include
    Link libraries:              /home/echo/work/lib/openVINO/onnxruntime-1.20.1/lib/libonnxruntime.so

  Python (for build):            /home/echo/work/lib/anaconda3/bin/python3

  Java:                          
    ant:                         NO
    Java:                        YES (ver 21.0.6)
    JNI:                         /usr/lib/jvm/default-java/include /usr/lib/jvm/default-java/include/linux /usr/lib/jvm/default-java/include
    Java wrappers:               YES (JAVA)
    Java tests:                  NO

  Install to:                    /usr/local
-----------------------------------------------------------------
```





