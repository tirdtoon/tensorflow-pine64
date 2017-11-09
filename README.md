# tensorflow-pine64

* build on PINE64/512/1G/2G

First of all you must do:
 - use more swap space. 

1. Follow this Blog -> http://zhiyisun.github.io/2017/02/15/Running-Google-Machine-Learning-Library-Tensorflow-On-ARM-64-bit-Platform.html
2. use bazel version 4.5.0
3. build by use this command: bazel build --verbose_failures tensorflow/tools/pip_package:build_pip_package
4. export LC_ALL=C
5. install by using this command: sudo python2.7 -m pip install /tmp/tensorflow_pkg/tensorflow-1.2.1-cp27-cp27mu-linux_aarch64.whl
