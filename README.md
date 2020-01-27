[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![OpenCV](https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/opencv_badge.svg)](https://opencv.org/)
[![macOS](https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/mac_badge.svg)](https://www.apple.com)
[![CMake](https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/cmake_badge.svg)](https://cmake.org/)


# OpenCV Installation Instructions

The following instructions are based on the [Adrian Rosenbrock OpenCv Tutorial](https://www.pyimagesearch.com/2018/08/17/install-opencv-4-on-macos/ "Install OpenCV 4 on macOS")

Please do every step until "Compile OpenCV4 from source" section.

Compile OpenCV4 from source :desktop_computer:
===========================

If your compilation end up an error like below:

![alt text][configuration_error]

Do the following steps:

1. Set directories

![alt text][cmake_directories]

2. Configure the project

![alt text][configure]

3. Set build_type to release

![alt text][build_type]

4.Make sure install prefix is /usr/local

![alt text][install_prefix]

5. Set extra_modules path

![alt text][extra_modules]

6. Set Python3_executables path

![alt text][python_executables]

7. Make sure BUILD_opencv_python3 value is 1

![alt text][build_opencv_python3]

8. Make sure INSTALL_PYTHON_EXAMPLES value is 1

![alt text][python_examples]

9. Make sure INSTALL_C_EXAMPLES value is 0.

![alt text][c_examples]

10. Make sure OPENCV_ENABLE_NONFREE value is 1.

![alt text][enable_nonfree]

11. Make sure BUILD_EXAMPLES value is 1.

![alt text][build_examples]

12. Click on the configure button again.

![alt text][configure]

13. Click on the generate button.

![alt text][generate]

14. Activate the virtual environment. My virtual environment name is "vision"

```shell
workon vision
cd ~/opencv/build
```

15. make the OpenCV

```shell
make -j4
```

![alt text][make_result]

16. install the OpenCV

```shell
sudo make install
```

![alt text][install_result]

You have successfully installed the OpenCV, now you can return back to the [Adrian's tutorial](https://www.pyimagesearch.com/2018/08/17/install-opencv-4-on-macos/ "Step #6: Sym-link OpenCV 4 on macOS to your virtual environment site-packages")

Tesserract Error :bangbang:
================
![alt text][tesserract_error]

# Solution :thinking:
[Tesserract problem is a common problem](https://github.com/justadudewhohacks/opencv4nodejs/issues/179)

Change the library paths:
![alt text][tesserract_solution]


[configuration_error]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/configuration_error.png "Cmake Error"

[cmake_directories]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/cmake_directories.png "source code:opencv, binaries: opencv/build"

[configure]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/configure.png "Configure button"

[build_type]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/build_type.png

[install_prefix]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/install_prefix.png

[extra_modules]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/extra_modules.png

[python_executables]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/python_executables.png

[build_opencv_python3]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/build_opencv_python3.png

[python_examples]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/python_examples.png

[c_examples]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/c_examples.png

[enable_nonfree]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/enable_nonfree.png

[build_examples]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/build_examples.png

[generate]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/generate.png

[make_result]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/make_result.png

[install_result]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/install_result.png

[tesserract_error]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/tesserract_error.png

[tesserract_solution]: https://github.com/AhmetTavli/OpenCV-macOS-Installation-Instructions/blob/master/Images/tesseract_solution.png

## Contributing :thought_balloon:
Pull requests are welcome.

For major changes, please open an issue, then discuss what you would like to change.

 ## License :scroll:
[MIT](https://opensource.org/licenses/MIT)
