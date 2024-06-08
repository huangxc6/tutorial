# 一、安装CUDA

## 1、查看电脑支持的cuda版本

快捷键 win + R，然后输入 cmd

![1.0_cmd](images/1.0_cmd.png)

然后输入如下指令：

```
nvidia-smi
```

![1.0 nvida-smi](images/1.0 nvida-smi.png)

我这里最高支持12.2版本

## 2、下载安装包

在[CUDA官网](https://developer.nvidia.com/cuda-toolkit-archive)下载所需版本的CUDA

> https://developer.nvidia.com/cuda-toolkit-archive

![1.1 download](images/1.1 download.png)

![1.1 download_option](images/1.1 download_option.png)

我这里选择下载12.0.0版本

## 3、安装选项

找到下载好的安装包，双击运行

![1.2 double clik](images/1.2 double clik.png)

选择一个临时文件存储路径等待提取

![1.2.1 select a temp path](images/1.2.1 select a temp path.png)

![1.2.2 wait](images/1.2.2 wait.png)

同意许可协议

![1.2.3 agree](images/1.2.3 agree.png)

自定义安装

![1.2.4 C](images/1.2.4 C.png)

选择不安装驱动（之前已经安装过）

![1.2.5 config](images/1.2.5 config.png)

选择安装位置（我这里选择了默认）

![1.2.6 install path](images/1.2.6 install path.png)

选择I undestand

![1.2.7 understand](images/1.2.7 understand.png)

安装成功

![1.2.8 success](images/1.2.8 success.png)

查看版本

```
nvcc -V
```

![1.2.9 nvcc -V](images/1.2.9 nvcc -V.png)

# 二、安装cuDNN

## 1、下载安装包

首先安装对应的cuDNN

![2.1 download](images/2.1 download.png)

![2.1 download_option](images/2.1 download_option.png)

## 2、安装

找到下载的安装包，并解压

![2.1 extract](images/2.1 extract.png)

![2.2 replace](images/2.2 replace.png)

把解压后的三个文件夹复制到`C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.0`（自己的安装目录）

![2.2 replace  success](images/2.2 replace  success.png)

## 3、测试

在`C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.0\extras\demo_suite`文件下打开终端

分别输入

```
deviceQuery.exe
bandwidthTest.exe
```

![2.3 pass](images/2.3 pass.png)

![2.3 bandwithTest pass](images/2.3 bandwithTest pass.png)

显示Result = PASS即为安装成功

