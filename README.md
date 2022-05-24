# thesis_documentation
This is the documentation about the optimization of Neural Networks used for my Master Thesis 2022

### Jetson AGX Xavier configuration from scratch
- After setup, refer this [blog](https://jkjung-avt.github.io/setting-up-xavier-nx/) for installing `install_basics.sh` script and `install_protobuf_1.8.0.sh` scripts.
  - The protobuf script takes 30-45 mins to complete. So go for walk, grab a coffee! ;)
- After the above step, execute `sudo pip3 install onnx==1.9.0` and it will install without errors.

#### Installing pycuda inside pip
- Error regarding 
  ```
  xlocale.h: No such file or directory
  ```
  `sudo ln -s /usr/include/locale.h /usr/include/xlocale.h` <- tried this [fix](https://github.com/biobakery/homebrew-biobakery/issues/31) 
- Installed `numpy == 1.19.4`
- Finally just execute `pip install pycuda==2021.1`

#### Installing onnx inside pip
- `pip install onnx==1.9.0`
