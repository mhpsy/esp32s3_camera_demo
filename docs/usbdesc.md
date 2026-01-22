Information for device SPCA2650 PC Camera (VID=0x1BCF PID=0x0B15):

------------------------------
Connection Information:
------------------------------
Device current bus speed: HighSpeed
Device supports USB 1.1 specification
Device supports USB 2.0 specification
// 设备分配的地址
Device address: 0x0005
// 设备当前配置值 实际开发中需要设置为1才会启用
Current configuration value: 0x00
// 视频流的数量，数据管道都没有打开
Number of open pipes: 0


// 这个软件很牛逼啊，能够先连接1.1握手，然后在连接2.0 可以看到不同的信息
------------------------------
Device Descriptor:
------------------------------
// 描述符长度 (18字节)
0x12	bLength
// 描述符类型 (设备描述符)
0x01	bDescriptorType
// USB协议版本 (2.0)
0x0200	bcdUSB
// 设备类代码 (0xEF: 混合设备类)
// 混合设备就是一个物理设备实现了多个功能，不要只加载这一层驱动，要看接口关联描述符
// 或者具体接口描述符
0xEF	bDeviceClass      (Miscellaneous device)
// 设备子类代码 (0x02: 通用子类)
0x02	bDeviceSubClass   
// 设备协议代码 (0x01: 接口关联描述符协议 IAD)
0x01	bDeviceProtocol   
// 端点0最大包长 (64字节)
0x40	bMaxPacketSize0   (64 bytes)
// 厂商ID (VID)
0x1BCF	idVendor
// 产品ID (PID)
0x0B15	idProduct
// 设备版本号 (3.18)
0x0318	bcdDevice
// 厂商字符串索引
0x01	iManufacturer   "SunplusIT Inc"
// 产品字符串索引
0x02	iProduct        "SPCA2650 PC Camera"
// 序列号字符串索引
0x03	iSerialNumber   "01.00.00"
// 可能的配置数量
0x01	bNumConfigurations

Device Qualifier Descriptor:
------------------------------
// 描述符长度 (10字节)
0x0A	bLength
// 描述符类型 (设备限定描述符)
0x06	bDescriptorType
// USB协议版本 (2.0)
0x0200	bcdUSB
// 设备类代码
0xEF	bDeviceClass      (Miscellaneous device)
// 设备子类代码
0x02	bDeviceSubClass   
// 设备协议代码
0x01	bDeviceProtocol   
// 端点0最大包长 (64字节)
0x40	bMaxPacketSize0   (64 bytes)
// 其他速度下的配置数量
0x01	bNumConfigurations 
// 保留
0x00	bReserved 


-------------------------
// 配置描述符
Configuration Descriptor:
-------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (配置描述符)
0x02	bDescriptorType
// 此配置下返回的所有数据的总长度 (754字节)
0x02F2	wTotalLength   (754 bytes)
// 此配置所支持的接口数量 (2个接口: 控制接口 + 流接口)
0x02	bNumInterfaces
// 启用此配置所需的 set_configuration 值
0x01	bConfigurationValue
// 描述此配置的字符串索引
0x00	iConfiguration
// 供电特性 (0x80: 总线供电, 不支持远程唤醒)
0x80	bmAttributes   (Bus-powered Device)
// 最大功耗 (250 * 2mA = 500mA)
0xFA	bMaxPower      (500 mA)

// 接口关联描述符，就是上面提到的 IAD
Interface Association Descriptor:
------------------------------
// 描述符长度 (8字节)
0x08	bLength
// 描述符类型 (接口关联描述符 IAD)
0x0B	bDescriptorType
// 第一接口编号 (接口 0)
0x00	bFirstInterface
// 关联的接口数量 (2个接口)
0x02	bInterfaceCount
// 功能类代码 (视频设备类)
0x0E	bFunctionClass      (Video Device Class)
// 功能子类代码 (视频接口集合)
0x03	bFunctionSubClass   (Video SubInterface Collection)
// 功能协议代码 (未定义)
0x00	bFunctionProtocol   (undefined)
// 描述此功能的字符串索引
0x04	iFunction   "PC Camera"

// 接口描述符，控制接口
Interface Descriptor:
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 0)
0x00	bInterfaceNumber
// 备用设置编号 (0 - 默认)
0x00	bAlternateSetting
// 此接口使用的端点数量 (1个，不含端点0)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频控制接口 Video Control Interface)
0x01	bInterfaceSubClass   (Video Control Interface)
// 接口协议
0x00	bInterfaceProtocol   (undefined)
// 描述此接口的字符串索引
0x04	iInterface   "PC Camera"

// 
Video Control Interface Descriptor (Interface Header):
------------------------------
// 描述符长度 (13字节)
0x0D	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_Header - 视频控制头描述符)
0x01	bDescriptorSubtype   (VC_Header - VideoControl IF Descriptor Subtype Header)
// UVC 规范版本 (1.00)
0x0100	bcdUVC (1.0)
// 视频控制接口描述符集合的总长度 (109字节)
0x006D	wTotalLength (109 bytes)
// 设备时钟频率 (48MHz)
0x02DC6C00	dwClockFrequency (48000000 Hz)
// 属于此视频功能的流接口数量 (1个)
0x01	bInCollection
// 流接口编号列表 (接口 1)
0x01	aInterfaceNr[1]

Video Interface Descriptor (Input Terminal):
------------------------------
// 描述符长度 (18字节)
0x12	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_INPUT_TERMINAL - 输入终端描述符)
0x02	bDescriptorSubtype   (VC_INPUT_TERMINAL - VideoControl IF Descriptor Subtype Input Terminal)
// 终端ID (ID=1)
0x01	bTerminalID
// 终端类型 (摄像头传感器)
0x0201	wTerminalType (ITT_CAMERA - VideoClass Camera Input Terminal)
// 关联的终端/单元ID (无)
0x00	bAssocTerminal
// 描述终端的字符串索引
0x00	iTerminal
// 最小焦距 (不支持)
0x0000	wObjectiveFocalLengthMin (0)
// 最大焦距 (不支持)
0x0000	wObjectiveFocalLengthMax (0)
// 目镜焦距 (不支持)
0x0000	wOcularFocalLength (0)
// 控制位图大小 (3字节)
0x03	bControlSize (3)
// 支持的控制 (字节1)
// 支持: 自动曝光模式, 绝对曝光时间
0x0A	bmControls[1]
          Bit 1 (Auto-Exposure Mode)
          Bit 3 (Exposure Time (Absolute))
// 支持的控制 (字节2)
0x00	bmControls[2]
// 支持的控制 (字节3)
0x00	bmControls[3]

Video Processing Unit Descriptor (处理单元描述符):
------------------------------
// 描述符长度 (11字节)
0x0B	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_PROCESSING_UNIT - 处理单元描述符)
0x05	bDescriptorSubtype   (VC_PROCESSING_UNIT - VideoControl IF Descriptor Subtype Processing Unit)
// 单元ID (ID=2)
0x02	bUnitID
// 源ID (连接到输入终端 ID=1)
0x01	bSourceID
// 最大数字放大倍数 (163.84)
0x4000	wMaxMultiplier (163.84)
// 控制位图大小 (2字节)
0x02	bControlSize
// 支持的控制 (字节1)
// 支持: 亮度, 对比度, 色调, 饱和度, 清晰度, 伽马, 白平衡温度
0x7F	bmControls[1]
          Bit 0 (Brightness)
          Bit 1 (Contrast)
          Bit 2 (Hue)
          Bit 3 (Saturation)
          Bit 4 (Sharpness)
          Bit 5 (Gamma)
          Bit 6 (White Balance Temperature)
// 支持的控制 (字节2)
// 支持: 背光补偿, 电源线频率, 自动白平衡温度
0x15	bmControls[2]
          Bit 0 (Backlight Compensation)
          Bit 2 (Power Line Frequency)
          Bit 4 (White Balance Temperature, Auto)
// 处理单元字符串索引
0x00	iProcessing
INFO:   field bmVideoStandards is missing

Video Extension Unit Descriptor (扩展单元描述符):
------------------------------
// 描述符长度 (29字节)
0x1D	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_EXTENSION_UNIT - 扩展单元描述符)
0x06	bDescriptorSubtype   (VC_EXTENSION_UNIT - VideoControl IF Descriptor Subtype Extension Unit)
// 单元ID (ID=3)
0x03	bUnitID
// 扩展单元 GUID (厂商特定功能的唯一标识符)
D5C2F42C-1808-4D9F-BE56753E271C9244	guidExtensionCode
// 此单元支持的控制数量 (3个)
0x03	bNumControls
// 输入引脚数量 (1个)
0x01	bNrInPins
// 输入源ID (连接到处理单元 ID=2)
0x02	baSourceID[1]
// 控制位图大小 (4字节)
0x04	bControlSize
// 支持的控制 (厂商定义的用于扩展单元的控制位)
0x07	bmControls[1] (Vendor-specific)
0x00	bmControls[2] (Vendor-specific)
0x00	bmControls[3] (Vendor-specific)
0x00	bmControls[4] (Vendor-specific)
// 扩展单元字符串索引
0x00	iExtension

Video Extension Unit Descriptor (扩展单元描述符):
------------------------------
// 描述符长度 (29字节)
0x1D	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_EXTENSION_UNIT - 扩展单元描述符)
0x06	bDescriptorSubtype   (VC_EXTENSION_UNIT - VideoControl IF Descriptor Subtype Extension Unit)
// 单元ID (ID=4)
0x04	bUnitID
// 扩展单元 GUID
63610682-5070-49AB-B8CCB3855E8D221D	guidExtensionCode
// 此单元支持的控制数量 (25个)
0x19	bNumControls
// 输入引脚数量 (1个)
0x01	bNrInPins
// 输入源ID (连接到扩展单元 ID=3)
0x03	baSourceID[1]
// 控制位图大小 (4字节)
0x04	bControlSize
// 支持的控制 (厂商定义)
0xFF	bmControls[1] (Vendor-specific)
0xFF	bmControls[2] (Vendor-specific)
0x77	bmControls[3] (Vendor-specific)
0x07	bmControls[4] (Vendor-specific)
// 扩展单元字符串索引
0x00	iExtension

Video Output Terminal Descriptor (输出终端描述符):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_OUTPUT_TERMINAL - 输出终端描述符)
0x03	bDescriptorSubtype   (VC_OUTPUT_TERMINAL - VideoControl IF Descriptor Subtype Output Terminal)
// 终端ID (ID=5)
0x05	bTerminalID
// 终端类型 (USB流输出终端)
0x0101	wTerminalType (TT_STREAMING - VideoClass USB Streaming Terminal)
// 关联的终端ID (无)
0x00	bAssocTerminal
// 输入源ID (连接到扩展单元 ID=4)
0x04	bSourceID
// 终端字符串索引
0x00	iTerminal

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x87: 输入端点 7)
0x87	bEndpointAddress  (IN endpoint 7)
// 属性 (0x03: 中断传输)
0x03	bmAttributes      (Transfer: Interrupt / Synch: None / Usage: Data)
// 最大包长 (16字节)
0x0010	wMaxPacketSize    (1 x 16 bytes)
// 轮询间隔 (128微帧 = 16ms)
0x08	bInterval         (128 microframes)

Video Class-Specific Endpoint Descriptor (类特定视频端点描述符):
------------------------------
// 描述符长度 (5字节)
0x05	bLength
// 描述符类型 (CS_ENDPOINT - 类特定端点描述符)
0x25	bDescriptorType (CS_ENDPOINT)
// 描述符子类型 (EP_INTERRUPT - 中断端点)
0x03	bDescriptorSubType (EP_INTERRUPT)
// 最大传输大小 (1029字节)
0x0405	wMaxTransferSize (1029 bytes)

Interface Descriptor (接口描述符 - 流接口):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (0 - 默认, 通常用于带宽为0)
0x00	bAlternateSetting
// 端点数量 (0个)
0x00	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口 Video Streaming Interface)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Video Streaming Interface Input Header Descriptor (视频流输入头描述符):
------------------------------
// 描述符长度 (15字节)
0x0F	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_INPUT_HEADER - 输入头)
0x01	bDescriptorSubtype   (VS_INPUT_HEADER - VideoStreaming IF Input Header)
// 支持的视频格式数量 (2种: MJPEG, Uncompressed)
0x02	bNumFormats
// 视频流接口描述符集合的总长度 (422字节)
0x01A6	wTotalLength   (422 bytes)
// 用于流传输的端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress
// 信息位
0x00	bmInfo 
// 连接的终端ID (ID=5)
0x05	bTerminalLink
// 静态图像捕获方法 (方法2)
0x02	bStillCaptureMethod (Method 2)
// 硬件触发支持 (不支持)
0x00	bTriggerSupport (not supported)
// 触发用法
0x00	bTriggerUsage (Initiate still image capture)
// 控制大小 (1字节)
0x01	bControlSize
// 格式1 (MJPEG) 支持的控制 (支持压缩质量)
0x04	Format 1 bmaControls[1]
	  wCompQuality (supported)
// 格式2 (Uncompressed) 支持的控制 (无)
0x00	Format 2 bmaControls[1]

Format MJPEG Descriptor (MJPEG 格式描述符):
------------------------------
// 描述符长度 (11字节)
0x0B	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FORMAT_MJPEG - MJPEG 格式)
0x06	bDescriptorSubtype   (VS_FORMAT_MJPEG - VideoStreaming IF Format MJPEG)
// 格式索引 (1)
0x01	bFormatIndex
// 此格式下的帧描述符数量 (5种分辨率)
0x05	bNumFrameDescriptors (5)
// 标志 (固定样本大小)
0x01	bmFlags (FixedSizeSamples)
// 默认帧索引
0x01	bDefaultFrameIndex
// X轴纵横比 (0)
0x00	bAspectRatioX (0)
// Y轴纵横比 (0)
0x00	bAspectRatioY (0)
// 交错标志
0x00	bmInterlaceFlags
	  Interlaced stream   (No)
	  Fields per frame    (2)
	  Field 1 first       (No)
	  Reserved, don't use (0)
	  Fields pattern      (Random pattern of field 1 and 2)
// 拷贝保护 (无限制)
0x00	bCopyProtect (No restrictions)

Frame MJPEG Descriptor (MJPEG 帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_MJPEG - MJPEG 帧)
0x07	bDescriptorSubtype   (VS_FRAME_MJPEG - VideoStreaming IF Frame MJPEG)
// 帧索引 (1)
0x01	bFrameIndex
// 能力 (不支持静态图像, 动态帧率)
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (1280)
0x0500	wWidth  (1280)
// 高度 (720)
0x02D0	wHeight (720)
// 最小比特率
0x0D2F0000	dwMinBitRate (221184000 bps)
// 最大比特率
0x0D2F0000	dwMaxBitRate (221184000 bps)
// 最大视频帧缓冲区大小
0x001C2000	dwMaxVideoFrameBufferSize (1843200 bytes)
// 默认帧间隔 (66.6666ms = 15fps)
0x000A2C2A	dwDefaultFrameInterval (66.666600 mSec (15.00 Hz))
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (Discrete Frame Intervals)
// 支持的离散帧间隔 1 (15fps)
0x000A2C2A	dwFrameInterval[1] (66.666600 mSec (15.00 Hz))

Frame MJPEG Descriptor (MJPEG 帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_MJPEG - MJPEG 帧)
0x07	bDescriptorSubtype   (VS_FRAME_MJPEG - VideoStreaming IF Frame MJPEG)
// 帧索引 (2)
0x02	bFrameIndex
// 能力
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (1280)
0x0500	wWidth  (1280)
// 高度 (712)
0x02C8	wHeight (712)
// 最小比特率
0x0D098000	dwMinBitRate (218726400 bps)
// 最大比特率
0x0D098000	dwMaxBitRate (218726400 bps)
// 最大视频帧缓冲区大小
0x001BD000	dwMaxVideoFrameBufferSize (1822720 bytes)
// 默认帧间隔 (66.6666ms = 15fps)
0x000A2C2A	dwDefaultFrameInterval (66.666600 mSec (15.00 Hz))
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (Discrete Frame Intervals)
// 支持的离散帧间隔 1 (15fps)
0x000A2C2A	dwFrameInterval[1] (66.666600 mSec (15.00 Hz))

Frame MJPEG Descriptor (MJPEG 帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)

// 描述符子类型 (VS_FRAME_MJPEG - MJPEG 帧)
0x07	bDescriptorSubtype   (VS_FRAME_MJPEG - VideoStreaming IF Frame MJPEG)
// 帧索引 (3)
0x03	bFrameIndex
// 能力
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (1280)
0x0500	wWidth  (1280)
// 高度 (480)
0x01E0	wHeight (480)
// 最小比特率
0x0BB80000	dwMinBitRate (196608000 bps)
// 最大比特率
0x0BB80000	dwMaxBitRate (196608000 bps)
// 最大视频帧缓冲区大小
0x0012C000	dwMaxVideoFrameBufferSize (1228800 bytes)
// 默认帧间隔 (50.000ms = 20fps)
0x0007A120	dwDefaultFrameInterval (50.000 ms)
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (Discrete Frame Intervals)
// 支持的离散帧间隔 1 (20fps)
0x0007A120	dwFrameInterval[1] (50.000 ms)

Frame MJPEG Descriptor (MJPEG 帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_MJPEG - MJPEG 帧)
0x07	bDescriptorSubtype   (VS_FRAME_MJPEG - VideoStreaming IF Frame MJPEG)
// 帧索引 (4)
0x04	bFrameIndex
// 能力
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (640)
0x0280	wWidth  (640)
// 高度 (480)
0x01E0	wHeight (480)
// 最小比特率
0x08CA0000	dwMinBitRate (147456000 bps)
// 最大比特率
0x08CA0000	dwMaxBitRate (147456000 bps)
// 最大视频帧缓冲区大小
0x00096000	dwMaxVideoFrameBufferSize (614400 bytes)
// 默认帧间隔 (33.333ms = 30fps)
0x00051615	dwDefaultFrameInterval (33.333 ms)
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (Discrete Frame Intervals)
// 支持的离散帧间隔 1 (30fps)
0x00051615	dwFrameInterval[1] (33.333 ms)

Frame MJPEG Descriptor (MJPEG 帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_MJPEG - MJPEG 帧)
0x07	bDescriptorSubtype   (VS_FRAME_MJPEG - VideoStreaming IF Frame MJPEG)
// 帧索引 (5)
0x05	bFrameIndex
// 能力
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (640)
0x0280	wWidth  (640)
// 高度 (472)
0x01D8	wHeight (472)
// 最小比特率
0x08A48000	dwMinBitRate (144998400 bps)
// 最大比特率
0x08A48000	dwMaxBitRate (144998400 bps)
// 最大视频帧缓冲区大小
0x00093800	dwMaxVideoFrameBufferSize (604160 bytes)
// 默认帧间隔 (33.333ms = 30fps)
0x00051615	dwDefaultFrameInterval (33.333 ms)
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (Discrete Frame Intervals)
// 支持的离散帧间隔 1 (30fps)
0x00051615	dwFrameInterval[1] (33.333 ms)

Video Streaming Still Image Frame Descriptor (静态图像帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_STILL_IMAGE_FRAME - 静态图像帧)
0x03	bDescriptorSubtype   (VS_STILL_IMAGE_FRAME - VideoStreaming IF Still Image Frame)
// 端点地址 (0x00: 使用默认控制端点)
0x00	bEndpointAddress
// 静态图像尺寸模式数量 (5种)
0x05	bNumImageSizePatterns
// 尺寸 1
0x500	wWidth_1  (1280)
0x2D0	wHeight_1 (720)
// 尺寸 2
0x500	wWidth_2  (1280)
0x2C8	wHeight_2 (712)
// 尺寸 3
0x500	wWidth_3  (1280)
0x1E0	wHeight_3 (480)
// 尺寸 4
0x280	wWidth_4  (640)
0x1E0	wHeight_4 (480)
// 尺寸 5
0x280	wWidth_5  (640)
0x1D8	wHeight_5 (472)
// 压缩模式数量 (4种)
0x04	bNumCompressionPattern
// 压缩比
0x01	bCompression[1]
0x05	bCompression[2]
0x0A	bCompression[3]
0x14	bCompression[4]

Video Streaming Color Format Descriptor (视频流颜色格式描述符):
------------------------------
// 描述符长度 (6字节)
0x06	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_COLORFORMAT - 颜色格式)
0x0D	bDescriptorSubtype   (VS_COLORFORMAT - VideoStreaming IF Format Color)
// 原色 (BT.709, sRGB)
0x01	bColorPrimaries (BT.709, sRGB (default))
// 传输特性 (BT.709)
0x01	bTransferCharacteristics (BT.709 (default))
// 矩阵系数 (SMPTE 170M)
0x04	bMatrixCoefficients (SMPTE 170M  (BT.601, default))

Uncompressed Video Format Descriptor (未压缩视频格式描述符):
------------------------------
// 描述符长度 (27字节)
0x1B	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FORMAT_UNCOMPRESSED - 未压缩格式)
0x04	bDescriptorSubtype   (VS_FORMAT_UNCOMPRESSED - VideoStreaming IF Uncompressed Format)
// 格式索引 (2)
0x02	bFormatIndex
// 此格式下的帧描述符数量 (5种分辨率)
0x05	bNumFrameDescriptors
// 格式 GUID (YUY2 格式)
32595559-0000-0010-800000AA00389B71	guidFormat
// 每像素位数 (16位)
0x10	bBitsPerPixel (16)
// 默认帧索引
0x01	bDefaultFrameIndex
// X轴纵横比 (0)
0x00	bAspectRatioX (0)
// Y轴纵横比 (0)
0x00	bAspectRatioY (0)
// 交错标志
0x00	bmInterlaceFlags
	  Interlaced stream   (No)
	  Fields per frame    (2)
	  Field 1 first       (No)
	  Reserved, don't use (0)
	  Fields pattern      (Field 1 only)
// 拷贝保护 (无限制)
0x00	bCopyProtect (No restrictions)

Uncompressed Video Frame Descriptor (未压缩视频帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_UNCOMPRESSED - 未压缩帧)
0x05	bDescriptorSubtype   (VS_FRAME_UNCOMPRESSED - VideoStreaming IF Uncompressed Frame)
// 帧索引 (1)
0x01	bFrameIndex
// 能力
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (1280)
0x0500	wWidth  (1280)
// 高度 (720)
0x02D0	wHeight (720)
// 最小比特率
0x08CA0000	dwMinBitRate (147456000 bps)
// 最大比特率
0x08CA0000	dwMaxBitRate (147456000 bps)
// 最大视频帧缓冲区大小
0x001C2000	dwMaxVideoFrameBufferSize (1843200 bytes)
// 默认帧间隔 (100.000ms = 10fps)
0x000F4240	dwDefaultFrameInterval (100.000 ms)
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (1 discrete frame interval)
// 支持的离散帧间隔 1 (10fps)
0x000F4240	dwFrameInterval[1] (100.000 ms)

Uncompressed Video Frame Descriptor (未压缩视频帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_UNCOMPRESSED - 未压缩帧)
0x05	bDescriptorSubtype   (VS_FRAME_UNCOMPRESSED - VideoStreaming IF Uncompressed Frame)
// 帧索引 (2)
0x02	bFrameIndex
// 能力
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (1280)
0x0500	wWidth  (1280)
// 高度 (712)
0x02C8	wHeight (712)
// 最小比特率
0x08B10000	dwMinBitRate (145817600 bps)
// 最大比特率
0x08B10000	dwMaxBitRate (145817600 bps)
// 最大视频帧缓冲区大小
0x001BD000	dwMaxVideoFrameBufferSize (1822720 bytes)
// 默认帧间隔 (100.000ms = 10fps)
0x000F4240	dwDefaultFrameInterval (100.000 ms)
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (1 discrete frame interval)
// 支持的离散帧间隔 1 (10fps)
0x000F4240	dwFrameInterval[1] (100.000 ms)

Uncompressed Video Frame Descriptor (未压缩视频帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_UNCOMPRESSED - 未压缩帧)
0x05	bDescriptorSubtype   (VS_FRAME_UNCOMPRESSED - VideoStreaming IF Uncompressed Frame)
// 帧索引 (3)
0x03	bFrameIndex
// 能力
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (1280)
0x0500	wWidth  (1280)
// 高度 (480)
0x01E0	wHeight (480)
// 最小比特率
0x05DC0000	dwMinBitRate (98304000 bps)
// 最大比特率
0x05DC0000	dwMaxBitRate (98304000 bps)
// 最大视频帧缓冲区大小
0x0012C000	dwMaxVideoFrameBufferSize (1228800 bytes)
// 默认帧间隔 (100.000ms = 10fps)
0x000F4240	dwDefaultFrameInterval (100.000 ms)
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (1 discrete frame interval)
// 支持的离散帧间隔 1 (10fps)
0x000F4240	dwFrameInterval[1] (100.000 ms)

Uncompressed Video Frame Descriptor (未压缩视频帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_UNCOMPRESSED - 未压缩帧)
0x05	bDescriptorSubtype   (VS_FRAME_UNCOMPRESSED - VideoStreaming IF Uncompressed Frame)
// 帧索引 (4)
0x04	bFrameIndex
// 能力
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (640)
0x0280	wWidth  (640)
// 高度 (480)
0x01E0	wHeight (480)
// 最小比特率
0x08CA0000	dwMinBitRate (147456000 bps)
// 最大比特率
0x08CA0000	dwMaxBitRate (147456000 bps)
// 最大视频帧缓冲区大小
0x00096000	dwMaxVideoFrameBufferSize (614400 bytes)
// 默认帧间隔 (33.333ms = 30fps)
0x00051615	dwDefaultFrameInterval (33.333 ms)
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (1 discrete frame interval)
// 支持的离散帧间隔 1 (30fps)
0x00051615	dwFrameInterval[1] ( 33.333 ms)

Uncompressed Video Frame Descriptor (未压缩视频帧描述符):
------------------------------
// 描述符长度 (30字节)
0x1E	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_UNCOMPRESSED - 未压缩帧)
0x05	bDescriptorSubtype   (VS_FRAME_UNCOMPRESSED - VideoStreaming IF Uncompressed Frame)
// 帧索引 (5)
0x05	bFrameIndex
// 能力
0x00	bmCapabilities
	  Still image supported (No)
	  Fixed frame-rate      (Disabled)
// 宽度 (640)
0x0280	wWidth  (640)
// 高度 (472)
0x01D8	wHeight (472)
// 最小比特率
0x08A48000	dwMinBitRate (144998400 bps)
// 最大比特率
0x08A48000	dwMaxBitRate (144998400 bps)
// 最大视频帧缓冲区大小
0x00093800	dwMaxVideoFrameBufferSize (604160 bytes)
// 默认帧间隔 (33.333ms = 30fps)
0x00051615	dwDefaultFrameInterval (33.333 ms)
// 帧间隔类型 (1=离散)
0x01	bFrameIntervalType (1 discrete frame interval)
// 支持的离散帧间隔 1 (30fps)
0x00051615	dwFrameInterval[1] ( 33.333 ms)

Video Streaming Still Image Frame Descriptor (静态图像帧描述符):
------------------------------
// 描述符长度 (27字节)
0x1B	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_STILL_IMAGE_FRAME - 静态图像帧)
0x03	bDescriptorSubtype   (VS_STILL_IMAGE_FRAME - VideoStreaming IF Still Image Frame)
// 端点地址 (0x00: 使用默认控制端点)
0x00	bEndpointAddress
// 静态图像尺寸模式数量 (5种)
0x05	bNumImageSizePatterns
// 尺寸 1
0x500	wWidth_1  (1280)
0x2D0	wHeight_1 (720)
0x500	wWidth_2  (1280)
0x2C8	wHeight_2 (712)
0x500	wWidth_3  (1280)
0x1E0	wHeight_3 (480)
0x280	wWidth_4  (640)
0x1E0	wHeight_4 (480)
0x280	wWidth_5  (640)
0x1D8	wHeight_5 (472)
0x01	bNumCompressionPattern
0x01	bCompression[1]

Video Streaming Color Format Descriptor (视频流颜色格式描述符):
------------------------------
// 描述符长度 (6字节)
0x06	bLength
// 描述符类型 (CS_INTERFACE - 类特定接口描述符)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_COLORFORMAT - 颜色格式)
0x0D	bDescriptorSubtype   (VS_COLORFORMAT - VideoStreaming IF Format Color)
// 原色 (BT.709, sRGB)
0x01	bColorPrimaries (BT.709, sRGB (default))
// 传输特性 (BT.709)
0x01	bTransferCharacteristics (BT.709 (default))
// 矩阵系数 (SMPTE 170M)
0x04	bMatrixCoefficients (SMPTE 170M  (BT.601, default))

Interface Descriptor (接口描述符 - 备用设置 1):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (1)
0x01	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (192字节)
0x00C0	wMaxPacketSize    (1 x 192 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 2):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (2)
0x02	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (384字节)
0x0180	wMaxPacketSize    (1 x 384 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 3):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (3)
0x03	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (512字节)
0x0200	wMaxPacketSize    (1 x 512 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 4):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (4)
0x04	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (640字节)
0x0280	wMaxPacketSize    (1 x 640 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 5):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (5)
0x05	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (800字节)
0x0320	wMaxPacketSize    (1 x 800 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 6):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (6)
0x06	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (944字节)
0x03B0	wMaxPacketSize    (1 x 944 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 7):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (7)
0x07	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (2 x 640 = 1280字节) - 2次事务(High Bandwidth)
0x0A80	wMaxPacketSize    (2 x 640 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 8):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (8)
0x08	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (2 x 800 = 1600字节) - 2次事务(High Bandwidth)
0x0B20	wMaxPacketSize    (2 x 800 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 9):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (9)
0x09	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (2 x 992 = 1984字节) - 2次事务(High Bandwidth)
0x0BE0	wMaxPacketSize    (2 x 992 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 10):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (10)
0x0A	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (3 x 960 = 2880字节) - 3次事务(High Bandwidth)
0x13C0	wMaxPacketSize    (3 x 960 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)

Interface Descriptor (接口描述符 - 备用设置 11):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (11)
0x0B	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (3 x 1020 = 3060字节) - 3次事务(High Bandwidth)
0x13FC	wMaxPacketSize    (3 x 1020 bytes)
// 轮询间隔 (1微帧)
0x01	bInterval         (1 microframes)


-------------------------------------
Other Speed Configuration Descriptor (其它速率配置描述符):
-------------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (其它速率配置描述符)
0x07	bDescriptorType
// 总长度 (410字节)
0x019A	wTotalLength   (410 bytes)
// 接口数量 (2个)
0x02	bNumInterfaces
// 配置编号 (1)
0x01	bConfigurationValue
// 配置字符串索引
0x00	iConfiguration
// 属性 (总线供电)
0x80	bmAttributes   (Bus-powered Device)
// 最大功耗 (500 mA)
0xFA	bMaxPower      (500 mA)

Interface Association Descriptor (接口关联描述符):
------------------------------
// 描述符长度 (8字节)
0x08	bLength
// 描述符类型 (接口关联描述符)
0x0B	bDescriptorType
// 第一个接口编号 (0)
0x00	bFirstInterface
// 接口数量 (2)
0x02	bInterfaceCount
// 功能类 (视频设备类)
0x0E	bFunctionClass      (Video Device Class)
// 功能子类 (视频子接口集合)
0x03	bFunctionSubClass   (Video SubInterface Collection)
// 功能协议 (未定义)
0x00	bFunctionProtocol   (undefined)
// 功能字符串索引 "PC Camera"
0x04	iFunction   "PC Camera"

Interface Descriptor (接口描述符 - 视频控制接口):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 0)
0x00	bInterfaceNumber
// 备用设置编号 (0)
0x00	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频控制接口)
0x01	bInterfaceSubClass   (Video Control Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引 "PC Camera"
0x04	iInterface   "PC Camera"

Video Control Interface Descriptor (Interface Header) (视频控制接口头描述符):
------------------------------
// 描述符长度 (13字节)
0x0D	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_HEADER)
0x01	bDescriptorSubtype   (VC_Header - VideoControl IF Descriptor Subtype Header)
// UVC 版本 (1.0)
0x0110	bcdUVC (1.0)
// 总长度 (110字节)
0x006E	wTotalLength (110 bytes)
// 时钟频率 (48MHz)
0x02DC6C00	dwClockFrequency (48000000 Hz)
// 接口集合数量 (1)
0x01	bInCollection
// 接口编号 (1)
0x01	aInterfaceNr[1]

Video Interface Descriptor (Input Terminal) (视频接口描述符 - 输入端点):
------------------------------
// 描述符长度 (18字节)
0x12	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_INPUT_TERMINAL)
0x02	bDescriptorSubtype   (VC_INPUT_TERMINAL - VideoControl IF Descriptor Subtype Input Terminal)
// 端点ID (1)
0x01	bTerminalID
// 端点类型 (摄像机)
0x0201	wTerminalType (ITT_CAMERA - VideoClass Camera Input Terminal)
// 关联端点 (0)
0x00	bAssocTerminal
// 端点字符串索引
0x00	iTerminal
// 最小焦距 (0)
0x0000	wObjectiveFocalLengthMin (0)
// 最大焦距 (0)
0x0000	wObjectiveFocalLengthMax (0)
// 目镜焦距 (0)
0x0000	wOcularFocalLength (0)
// 控制大小 (3字节)
0x03	bControlSize (3)
// 控制位图 1
0x0A	bmControls[1]
          Bit 1 (Auto-Exposure Mode)
          Bit 3 (Exposure Time (Absolute))
// 控制位图 2
0x00	bmControls[2]
// 控制位图 3
0x00	bmControls[3]

Video Interface Descriptor (Processing Unit) (视频接口描述符 - 处理单元):
------------------------------
// 描述符长度 (12字节)
0x0C	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_PROCESSING_UNIT)
0x05	bDescriptorSubtype   (VC_PROCESSING_UNIT - VideoControl IF Descriptor Subtype Processing Unit)
// 单元ID (2)
0x02	bUnitID
// 源ID (1)
0x01	bSourceID
// 最大倍率 (163.84)
0x4000	wMaxMultiplier (163.84)
// 控制大小 (2字节)
0x02	bControlSize
// 控制位图 1
0x7F	bmControls[1]
          Bit 0 (Brightness)
          Bit 1 (Contrast)
          Bit 2 (Hue)
          Bit 3 (Saturation)
          Bit 4 (Sharpness)
          Bit 5 (Gamma)
          Bit 6 (White Balance Temperature)
// 控制位图 2
0x15	bmControls[2]
          Bit 0 (Backlight Compensation)
          Bit 2 (Power Line Frequency)
          Bit 4 (White Balance Temperature, Auto)
// 处理单元字符串索引
0x00	iProcessing
// 视频标准位图
0x00	bmVideoStandards - bitmap should be ignored

Video Interface Descriptor (Extension Unit) (视频接口描述符 - 扩展单元):
------------------------------
// 描述符长度 (29字节)
0x1D	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_EXTENSION_UNIT)
0x06	bDescriptorSubtype   (VC_EXTENSION_UNIT - VideoControl IF Descriptor Subtype Extension Unit)
// 单元ID (3)
0x03	bUnitID
// GUID 扩展码
0FB885C3-68C2-4547-90F78F47579D95FC	guidExtensionCode
// 控制数量 (5)
0x05	bNumControls
// 输入引脚数量 (1)
0x01	bNrInPins
// 源ID (2)
0x02	baSourceID[1]
// 控制大小 (4字节)
0x04	bControlSize
// 控制位图 1 (厂商定义)
0x1F	bmControls[1] (Vendor-specific)
// 控制位图 2 (厂商定义)
0x00	bmControls[2] (Vendor-specific)
// 控制位图 3 (厂商定义)
0x00	bmControls[3] (Vendor-specific)
// 控制位图 4 (厂商定义)
0x00	bmControls[4] (Vendor-specific)
// 扩展单元字符串索引
0x00	iExtension

Video Interface Descriptor (Extension Unit) (视频接口描述符 - 扩展单元):
------------------------------
// 描述符长度 (29字节)
0x1D	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_EXTENSION_UNIT)
0x06	bDescriptorSubtype   (VC_EXTENSION_UNIT - VideoControl IF Descriptor Subtype Extension Unit)
// 单元ID (4)
0x04	bUnitID
// GUID 扩展码
63610682-5070-49AB-B8CCB3855E8D221D	guidExtensionCode
// 控制数量 (25)
0x19	bNumControls
// 输入引脚数量 (1)
0x01	bNrInPins
// 源ID (3)
0x03	baSourceID[1]
// 控制大小 (4字节)
0x04	bControlSize
// 控制位图 1 (厂商定义)
0xFF	bmControls[1] (Vendor-specific)
// 控制位图 2 (厂商定义)
0xFF	bmControls[2] (Vendor-specific)
// 控制位图 3 (厂商定义)
0x77	bmControls[3] (Vendor-specific)
// 控制位图 4 (厂商定义)
0x07	bmControls[4] (Vendor-specific)
// 扩展单元字符串索引
0x00	iExtension

Video Interface Descriptor (Output Terminal) (视频接口描述符 - 输出端点):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VC_OUTPUT_TERMINAL)
0x03	bDescriptorSubtype   (VC_OUTPUT_TERMINAL - VideoControl IF Descriptor Subtype Output Terminal)
// 端点ID (5)
0x05	bTerminalID
// 端点类型 (流传输)
0x0101	wTerminalType (TT_STREAMING - VideoClass USB Streaming Terminal)
// 关联端点 (0)
0x00	bAssocTerminal
// 源ID (4)
0x04	bSourceID
// 端点字符串索引
0x00	iTerminal

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x87: 输入端点 7)
0x87	bEndpointAddress  (IN endpoint 7)
// 属性 (中断，无同步，数据)
0x03	bmAttributes      (Transfer: Interrupt / Synch: None / Usage: Data)
// 最大包长 (16字节)
0x0010	wMaxPacketSize    (1 x 16 bytes)
// 轮询间隔 (8帧)
0x08	bInterval         (8 frames)

Video Endpoint Descriptor (视频端点描述符):
------------------------------
// 描述符长度 (5字节)
0x05	bLength
// 描述符类型 (CS_ENDPOINT)
0x25	bDescriptorType (CS_ENDPOINT)
// 描述符子类型 (EP_INTERRUPT)
0x03	bDescriptorSubType (EP_INTERRUPT)
// 最大传输大小 (1029字节)
0x0405	wMaxTransferSize (1029 bytes)

Interface Descriptor (接口描述符 - 视频流接口):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (0 - 默认空闲)
0x00	bAlternateSetting
// 端点数量 (0个)
0x00	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Video Streaming Interface Input Header Descriptor (视频流接口输入头描述符):
------------------------------
// 描述符长度 (15字节)
0x0F	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_INPUT_HEADER)
0x01	bDescriptorSubtype   (VS_INPUT_HEADER - VideoStreaming IF Input Header)
// 格式数量 (2个)
0x02	bNumFormats
// 总长度 (157字节)
0x009D	wTotalLength   (157 bytes)
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress
// 信息位图
0x00	bmInfo 
// 终端链接ID (5)
0x05	bTerminalLink
// 静态图像捕获方法 (方法 1)
0x01	bStillCaptureMethod (Method 1)
// 触发支持 (不支持)
0x00	bTriggerSupport (not supported)
// 触发用法 (启动静态图像捕获)
0x00	bTriggerUsage (Initiate still image capture)
// 控制大小 (1字节)
0x01	bControlSize
// 格式1控制
0x00	Format 1 bmaControls[1]
// 格式2控制
0x04	Format 2 bmaControls[1]
	  wCompQuality (supported)

Uncompressed Video Format Descriptor (非压缩视频格式描述符):
------------------------------
// 描述符长度 (27字节)
0x1B	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FORMAT_UNCOMPRESSED)
0x04	bDescriptorSubtype   (VS_FORMAT_UNCOMPRESSED - VideoStreaming IF Uncompressed Format)
// 格式索引 (1)
0x01	bFormatIndex
// 帧描述符数量 (1)
0x01	bNumFrameDescriptors
// 格式GUID (YUY2)
32595559-0000-0010-800000AA00389B71	guidFormat
// 每像素位数 (16)
0x10	bBitsPerPixel (16)
// 默认帧索引 (1)
0x01	bDefaultFrameIndex
// X轴纵横比 (0)
0x00	bAspectRatioX (0)
// Y轴纵横比 (0)
0x00	bAspectRatioY (0)
// 交错标志
0x00	bmInterlaceFlags
	  Interlaced stream   (No)
	  Fields per frame    (2)
	  Field 1 first       (No)
	  Reserved, don't use (0)
	  Fields pattern      (Field 1 only)
// 复制保护 (无限制)
0x00	bCopyProtect (No restrictions)

Uncompressed Video Frame Descriptor (非压缩视频帧描述符):
------------------------------
// 描述符长度 (46字节)
0x2E	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_UNCOMPRESSED)
0x05	bDescriptorSubtype   (VS_FRAME_UNCOMPRESSED - VideoStreaming IF Uncompressed Frame)
// 帧索引 (1)
0x01	bFrameIndex
// 功能特性 (支持静态图像)
0x01	bmCapabilities
	  Still image supported (Yes)
	  Fixed frame-rate      (Disabled)
// 宽度 (160)
0x00A0	wWidth  (160)
// 高度 (120)
0x0078	wHeight (120)
// 最小比特率 (1.536 Mbps)
0x00177000	dwMinBitRate (1536000 bps)
// 最大比特率 (1.536 Mbps)
0x008CA000	dwMaxBitRate (1536000 bps)
// 最大帧缓冲大小 (38400字节)
0x00009600	dwMaxVideoFrameBufferSize (38400 bytes)
// 默认帧间隔 (50ms - 20fps)
0x0007A120	dwDefaultFrameInterval (50.000 ms)
// 帧间隔类型 (5个离散值)
0x05	bFrameIntervalType (5 discrete frame intervals)
// 帧间隔 1 (50ms - 20fps)
0x0007A120	dwFrameInterval[1] ( 50.000 ms)
// 帧间隔 2 (66.667ms - 15fps)
0x000A2C2A	dwFrameInterval[2] ( 66.667 ms)
// 帧间隔 3 (100ms - 10fps)
0x000F4240	dwFrameInterval[3] (100.000 ms)
// 帧间隔 4 (133.333ms - 7.5fps)
0x00145855	dwFrameInterval[4] (133.333 ms)
// 帧间隔 5 (200ms - 5fps)
0x001E8480	dwFrameInterval[5] (200.000 ms)

Video Streaming Color Format Descriptor (视频流颜色格式描述符):
------------------------------
// 描述符长度 (6字节)
0x06	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_COLORFORMAT)
0x0D	bDescriptorSubtype   (VS_COLORFORMAT - VideoStreaming IF Format Color)
// 颜色原色 (sRGB)
0x01	bColorPrimaries (BT.709, sRGB (default))
// 传输特性 (BT.709)
0x01	bTransferCharacteristics (BT.709 (default))
// 矩阵系数 (BT.601)
0x04	bMatrixCoefficients (SMPTE 170M  (BT.601, default))

Format MJPEG Descriptor (MJPEG 格式描述符):
------------------------------
// 描述符长度 (11字节)
0x0B	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FORMAT_MJPEG)
0x06	bDescriptorSubtype   (VS_FORMAT_MJPEG - VideoStreaming IF Format MJPEG)
// 格式索引 (2)
0x02	bFormatIndex
// 帧描述符数量 (1)
0x01	bNumFrameDescriptors (1)
// 标志 (固定采样大小)
0x01	bmFlags (FixedSizeSamples)
// 默认帧索引 (1)
0x01	bDefaultFrameIndex
// X轴纵横比 (0)
0x00	bAspectRatioX (0)
// Y轴纵横比 (0)
0x00	bAspectRatioY (0)
// 交错标志
0x00	bmInterlaceFlags
	  Interlaced stream   (No)
	  Fields per frame    (2)
	  Field 1 first       (No)
	  Reserved, don't use (0)
	  Fields pattern      (Random pattern of field 1 and 2)
// 复制保护 (无限制)
0x00	bCopyProtect (No restrictions)

Frame MJPEG Descriptor (MJPEG 帧描述符):
------------------------------
// 描述符长度 (46字节)
0x2E	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_FRAME_MJPEG)
0x07	bDescriptorSubtype   (VS_FRAME_MJPEG - VideoStreaming IF Frame MJPEG)
// 帧索引 (1)
0x01	bFrameIndex
// 功能特性 (支持静态图像)
0x01	bmCapabilities
	  Still image supported (Yes)
	  Fixed frame-rate      (Disabled)
// 宽度 (160)
0x00A0	wWidth  (160)
// 高度 (120)
0x0078	wHeight (120)
// 最小比特率 (1.536 Mbps)
0x00177000	dwMinBitRate (1536000 bps)
// 最大比特率 (9.216 Mbps)
0x008CA000	dwMaxBitRate (9216000 bps)
// 最大帧缓冲大小 (38400字节)
0x00009600	dwMaxVideoFrameBufferSize (38400 bytes)
// 默认帧间隔 (50ms - 20fps)
0x0007A120	dwDefaultFrameInterval (50.000 ms)
// 帧间隔类型 (离散)
0x05	bFrameIntervalType (Discrete Frame Intervals)
// 帧间隔 1 (50ms - 20fps)
0x0007A120	dwFrameInterval[1] (50.000 ms)
// 帧间隔 2 (66.667ms - 15fps)
0x000A2C2A	dwFrameInterval[2] (66.667 ms)
// 帧间隔 3 (100ms - 10fps)
0x000F4240	dwFrameInterval[3] (100.000 ms)
// 帧间隔 4 (133.333ms - 7.5fps)
0x00145855	dwFrameInterval[4] (133.333 ms)
// 帧间隔 5 (200ms - 5fps)
0x001E8480	dwFrameInterval[5] (200.000 ms)

Video Streaming Color Format Descriptor (视频流颜色格式描述符):
------------------------------
// 描述符长度 (6字节)
0x06	bLength
// 描述符类型 (CS_INTERFACE)
0x24	bDescriptorType      (CS_INTERFACE - VideoClass Descriptor Type Interface)
// 描述符子类型 (VS_COLORFORMAT)
0x0D	bDescriptorSubtype   (VS_COLORFORMAT - VideoStreaming IF Format Color)
// 颜色原色 (sRGB)
0x01	bColorPrimaries (BT.709, sRGB (default))
// 传输特性 (BT.709)
0x01	bTransferCharacteristics (BT.709 (default))
// 矩阵系数 (BT.601)
0x04	bMatrixCoefficients (SMPTE 170M  (BT.601, default))

Interface Descriptor (接口描述符 - 备用设置 1):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (1)
0x01	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (192字节)
0x00C0	wMaxPacketSize    (1 x 192 bytes)
// 轮询间隔 (1帧 = 1ms)
0x01	bInterval         (1 frames)

Interface Descriptor (接口描述符 - 备用设置 2):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (2)
0x02	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (384字节)
0x0180	wMaxPacketSize    (1 x 384 bytes)
// 轮询间隔 (1帧 = 1ms)
0x01	bInterval         (1 frames)

Interface Descriptor (接口描述符 - 备用设置 3):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (3)
0x03	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (512字节)
0x0200	wMaxPacketSize    (1 x 512 bytes)
// 轮询间隔 (1帧 = 1ms)
0x01	bInterval         (1 frames)

Interface Descriptor (接口描述符 - 备用设置 4):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (4)
0x04	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (640字节)
0x0280	wMaxPacketSize    (1 x 640 bytes)
// 轮询间隔 (1帧 = 1ms)
0x01	bInterval         (1 frames)

Interface Descriptor (接口描述符 - 备用设置 5):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (5)
0x05	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (800字节)
0x0320	wMaxPacketSize    (1 x 800 bytes)
// 轮询间隔 (1帧 = 1ms)
0x01	bInterval         (1 frames)

Interface Descriptor (接口描述符 - 备用设置 6):
------------------------------
// 描述符长度 (9字节)
0x09	bLength
// 描述符类型 (接口描述符)
0x04	bDescriptorType
// 接口编号 (接口 1)
0x01	bInterfaceNumber
// 备用设置编号 (6)
0x06	bAlternateSetting
// 端点数量 (1个)
0x01	bNumEndPoints
// 接口类 (视频设备类)
0x0E	bInterfaceClass      (Video Device Class)
// 接口子类 (视频流接口)
0x02	bInterfaceSubClass   (Video Streaming Interface)
// 接口协议 (未定义)
0x00	bInterfaceProtocol   (undefined)
// 接口字符串索引
0x00	iInterface

Endpoint Descriptor (端点描述符):
------------------------------
// 描述符长度 (7字节)
0x07	bLength
// 描述符类型 (端点描述符)
0x05	bDescriptorType
// 端点地址 (0x81: 输入端点 1)
0x81	bEndpointAddress  (IN endpoint 1)
// 属性 (同步，异步，数据)
0x05	bmAttributes      (Transfer: Isochronous / Synch: Asynchronous / Usage: Data)
// 最大包长 (944字节)
0x03B0	wMaxPacketSize    (1 x 944 bytes)
// 轮询间隔 (1帧 = 1ms)
0x01	bInterval         (1 frames)

Microsoft OS Descriptor (微软 OS 描述符):
------------------------------
// 描述符长度 (18字节)
0x12	bLength
// 描述符类型 (字符串描述符)
0x03	bDescriptorType
// Hex dump: "MSFT100" string + Vendor Code
Hex dump: 
0x12 0x03 0x4D 0x00 0x53 0x00 0x46 0x00 0x54 0x00 
0x31 0x00 0x30 0x00 0x30 0x00 0x01 0x00 


--------------------------------
String Descriptor Table (字符串描述符表)
--------------------------------
// 索引  语言ID  字符串
Index  LANGID  String
// 语言支持 (英语 - 0x0409)
0x00   0x0000  0x0409 
// 制造商字符串
0x01   0x0409  "SunplusIT Inc"
// 产品字符串
0x02   0x0409  "SPCA2650 PC Camera"
// 序列号字符串
0x03   0x0409  "01.00.00"
// 接口/功能字符串
0x04   0x0409  "PC Camera"

------------------------------

Connection path for device: 
符合 USB xHCI 的主机控制器
Root Hub
SPCA2650 PC Camera (VID=0x1BCF PID=0x0B15) Port: 1

Running on: Windows 10 or greater (Build Version 26100)

Brought to you by TDD v2.19.0, Dec  5 2023, 12:08:38

