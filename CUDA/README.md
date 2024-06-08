# 一、安装CUDA

## 1、查看电脑支持的cuda版本

快捷键 win + R，然后输入 cmd

![1.0_cmd](images/1.0_cmd.png)

然后输入如下指令：

```
nvidia-smi
```

![1.0_nvida-smi](images/1.0_nvida-smi.png)

我这里最高支持12.2版本

## 2、下载安装包

在[CUDA官网](https://developer.nvidia.com/cuda-toolkit-archive)下载所需版本的CUDA

> https://developer.nvidia.com/cuda-toolkit-archive

![1.1_download](images/1.1_download.png)

![1.1_download_option](images/1.1_download_option.png)

我这里选择下载12.0.0版本

## 3、安装选项

找到下载好的安装包，双击运行

![1.2_double_clik](images/1.2_double_clik.png)

选择一个临时文件存储路径等待提取

![1.2.1_select_a_temp_path](images/1.2.1_select_a_temp_path.png)

![1.2.2_wait](images/1.2.2_wait.png)

同意许可协议

![1.2.3_agree](images/1.2.3_agree.png)

自定义安装

![1.2.4_C](images/1.2.4_C.png)

选择不安装驱动（之前已经安装过）

![1.2.5_config](images/1.2.5_config.png)

选择安装位置（我这里选择了默认）

![1.2.6_install_path](images/1.2.6_install_path.png)

选择I_undestand

![1.2.7_understand](images/1.2.7_understand.png)

安装成功

![1.2.8_success](images/1.2.8_success.png)

查看版本

```
nvcc_-V
```

![1.2.9_nvcc_-V](images/1.2.9_nvcc_-V.png)

# 二、安装cuDNN

## 1、下载安装包

首先安装对应的cuDNN

![2.1_download](images/2.1_download.png)

![2.1_download_option](images/2.1_download_option.png)

## 2、安装

找到下载的安装包，并解压

![2.1_extract](images/2.1_extract.png)

![2.2_replace](images/2.2_replace.png)

把解压后的三个文件夹复制到`C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.0`（自己的安装目录）

![2.2_replace_success](images/2.2_replace_success.png)

## 3、测试

在`C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.0\extras\demo_suite`文件下打开终端

分别输入

```
deviceQuery.exe
bandwidthTest.exe
```

![2.3_pass](images/2.3_pass.png)

![2.3_bandwithTest_pass](images/2.3_bandwithTest_pass.png)

显示Result = PASS即为安装成功

