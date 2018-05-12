# 基于`intoyun-wifi-mcu-sdk`开发的实例工程

通过该项目，我们将介绍如何使用`intoyun-wifi-mcu-sdk`进行从模式开发。

该项目工程使用intoyuniot开发工具开发。

## 目录和文件组成

```
+-- lib                       : 库目录
+-- keil                      : keil工程
+-- src                       : 源文件目录
    +-- sdk  : 从模式wifi MCU端SDK
    +-- mcu                   : MCU SDK库
    +-- user                  : 用户应用代码
+-- intoyuniot.ini            : intoyuniot配置文件
+-- README.md                 : 项目说明文件

```

## 下载工程

```
git clone --recursive https://github.com/IntoYun/intoyun-wifi-mcu-demo.git
```

## 项目实例开发

- [硬件平台:stm32f103rbx](#5-esp32硬件平台)

### 1 stm32f103rbx

#### 1.1 代码编写

用户可以把示例代码复制到工程中，具体如下：

复制`src/sdk/examples/smartLight/stm32f103rbx/`到`src/user/`中。

#### 1.2 程序编译

```
intoyuniot run -t clean              # 清除临时文件

intoyuniot run -e stm32f103rbx -t upload  # 编译和下载

```

