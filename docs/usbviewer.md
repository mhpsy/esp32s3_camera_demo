[Port1]  :  USB Composite Device


Is Port User Connectable:         yes
Is Port Debug Capable:            no
Companion Port Number:            4
Companion Hub Symbolic Link Name: USB#ROOT_HUB30#5&a1c8184&0&0#{f18a0e88-c30c-11d0-8815-00a0c906bed8}
Protocols Supported:
 USB 1.1:                         yes
 USB 2.0:                         yes
 USB 3.0:                         no

Device Power State:               PowerDeviceD3


       ---===>USB4 Information<===---
Port is USB4 Capable:              No
Device is tunneled through USB4:   No

       ---===>Device Information<===---
English product name: "SPCA2650 PC Camera"

ConnectionStatus:                  
Current Config Value:              0x01  -> Device Bus Speed: High (is not SuperSpeed or higher capable)
Device Address:                    0x05
Open Pipes:                           1

          ===>Device Descriptor<===
bLength:                           0x12
bDescriptorType:                   0x01
bcdUSB:                          0x0200
bDeviceClass:                      0xEF  -> This is a Multi-interface Function Code Device
bDeviceSubClass:                   0x02  -> This is the Common Class Sub Class
bDeviceProtocol:                   0x01  -> This is the Interface Association Descriptor protocol
bMaxPacketSize0:                   0x40 = (64) Bytes
idVendor:                        0x1BCF = Sunplus Innovation Technology Inc.
idProduct:                       0x0B15
bcdDevice:                       0x0318
iManufacturer:                     0x01
     English (United States)  "SunplusIT Inc"
iProduct:                          0x02
     English (United States)  "SPCA2650 PC Camera"
iSerialNumber:                     0x03
     English (United States)  "01.00.00"
bNumConfigurations:                0x01

          ---===>Open Pipes<===---

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x87  -> Direction: IN - EndpointID: 7
bmAttributes:                      0x03  -> Interrupt Transfer Type
wMaxPacketSize:                  0x0010 = 1 transactions per microframe, 0x10 max bytes
bInterval:                         0x08

       ---===>Full Configuration Descriptor<===---

          ===>Configuration Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x02
wTotalLength:                    0x02F2  -> Validated
bNumInterfaces:                    0x02
bConfigurationValue:               0x01
iConfiguration:                    0x00
bmAttributes:                      0x80  -> Bus Powered
MaxPower:                          0xFA = 500 mA

          ===>IAD Descriptor<===
bLength:                           0x08
bDescriptorType:                   0x0B
bFirstInterface:                   0x00
bInterfaceCount:                   0x02
bFunctionClass:                    0x0E  -> Video Interface Class
bFunctionSubClass:                 0x03  -> Video Interface Collection
bFunctionProtocol:                 0x00  -> PC_PROTOCOL_UNDEFINED protocol
iFunction:                         0x04
     English (United States)  "PC Camera"

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x00
bAlternateSetting:                 0x00
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x01  -> Video Control Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x04
     English (United States)  "PC Camera"

          ===>Class-Specific Video Control Interface Header Descriptor<===
bLength:                           0x0D
bDescriptorType:                   0x24
bDescriptorSubtype:                0x01
bcdVDC:                          0x0100
wTotalLength:                    0x006D  -> Validated
dwClockFreq:                 0x02DC6C00 = (48000000) Hz
bInCollection:                     0x01
baInterfaceNr[1]:                  0x01
USB Video Class device: spec version 1.0

          ===>Video Control Input Terminal Descriptor<===
bLength:                           0x12
bDescriptorType:                   0x24
bDescriptorSubtype:                0x02
bTerminalID:                       0x01
wTerminalType:                   0x0201 = (ITT_CAMERA)
bAssocTerminal:                    0x00
iTerminal:                         0x00
===>Camera Input Terminal Data
wObjectiveFocalLengthMin:        0x0000
wObjectiveFocalLengthMax:        0x0000
wOcularFocalLength:              0x0000
bControlSize:                      0x03
bmControls : 0x0A 0x00 0x00 
     D00 = 0   no -  Scanning Mode
     D01 = 1  yes -  Auto-Exposure Mode
     D02 = 0   no -  Auto-Exposure Priority
     D03 = 1  yes -  Exposure Time (Absolute)
     D04 = 0   no -  Exposure Time (Relative)
     D05 = 0   no -  Focus (Absolute)
     D06 = 0   no -  Focus (Relative)
     D07 = 0   no -  Iris (Absolute)
     D08 = 0   no -  Iris (Relative)
     D09 = 0   no -  Zoom (Absolute)
     D10 = 0   no -  Zoom (Relative)
     D11 = 0   no -  PanTilt (Absolute)
     D12 = 0   no -  PanTilt (Relative)
     D13 = 0   no -  Roll (Absolute)
     D14 = 0   no -  Roll (Relative)
     D15 = 0   no -  Reserved
     D16 = 0   no -  Reserved
     D17 = 0   no -  Focus, Auto
     D18 = 0   no -  Privacy
     D19 = 0   no -  Focus, Simple
     D20 = 0   no -  Window
     D21 = 0   no -  Region of Interest
     D22 = 0   no -  Reserved
     D23 = 0   no -  Reserved

          ===>Video Control Processing Unit Descriptor<===
bLength:                           0x0B
bDescriptorType:                   0x24
bDescriptorSubtype:                0x05
bUnitID:                           0x02
bSourceID:                         0x01
wMaxMultiplier:                  0x4000
bControlSize:                      0x02
bmControls : 0x7F 0x15 
     D00 = 1  yes -  Brightness
     D01 = 1  yes -  Contrast
     D02 = 1  yes -  Hue
     D03 = 1  yes -  Saturation
     D04 = 1  yes -  Sharpness
     D05 = 1  yes -  Gamma
     D06 = 1  yes -  White Balance Temperature
     D07 = 0   no -  White Balance Component
     D08 = 1  yes -  Backlight Compensation
     D09 = 0   no -  Gain
     D10 = 1  yes -  Power Line Frequency
     D11 = 0   no -  Hue, Auto
     D12 = 1  yes -  White Balance Temperature, Auto
     D13 = 0   no -  White Balance Component, Auto
     D14 = 0   no -  Digital Multiplier
     D15 = 0   no -  Digital Multiplier Limit
iProcessing :                      0x00

          ===>Video Control Extension Unit Descriptor<===
bLength:                           0x1D
bDescriptorType:                   0x24
bDescriptorSubtype:                0x06
bUnitID:                           0x03
guidExtensionCode:                 {D5C2F42C-1808-4D9F-BE56-753E271C9244}
bNumControls:                      0x03
bNrInPins:                         0x01
===>List of Connected Units and Terminal ID's
baSourceID[1]:                     0x02
bControlSize:                      0x04
bmControls : 0x07 0x00 0x00 0x00 
     D00 = 1  yes -  Vendor-Specific (Optional)
     D01 = 1  yes -  Vendor-Specific (Optional)
     D02 = 1  yes -  Vendor-Specific (Optional)
     D03 = 0   no -  Vendor-Specific (Optional)
     D04 = 0   no -  Vendor-Specific (Optional)
     D05 = 0   no -  Vendor-Specific (Optional)
     D06 = 0   no -  Vendor-Specific (Optional)
     D07 = 0   no -  Vendor-Specific (Optional)
     D08 = 0   no -  Vendor-Specific (Optional)
     D09 = 0   no -  Vendor-Specific (Optional)
     D10 = 0   no -  Vendor-Specific (Optional)
     D11 = 0   no -  Vendor-Specific (Optional)
     D12 = 0   no -  Vendor-Specific (Optional)
     D13 = 0   no -  Vendor-Specific (Optional)
     D14 = 0   no -  Vendor-Specific (Optional)
     D15 = 0   no -  Vendor-Specific (Optional)
     D16 = 0   no -  Vendor-Specific (Optional)
     D17 = 0   no -  Vendor-Specific (Optional)
     D18 = 0   no -  Vendor-Specific (Optional)
     D19 = 0   no -  Vendor-Specific (Optional)
     D20 = 0   no -  Vendor-Specific (Optional)
     D21 = 0   no -  Vendor-Specific (Optional)
     D22 = 0   no -  Vendor-Specific (Optional)
     D23 = 0   no -  Vendor-Specific (Optional)
     D24 = 0   no -  Vendor-Specific (Optional)
     D25 = 0   no -  Vendor-Specific (Optional)
     D26 = 0   no -  Vendor-Specific (Optional)
     D27 = 0   no -  Vendor-Specific (Optional)
     D28 = 0   no -  Vendor-Specific (Optional)
     D29 = 0   no -  Vendor-Specific (Optional)
     D30 = 0   no -  Vendor-Specific (Optional)
     D31 = 0   no -  Vendor-Specific (Optional)
iExtension:                        0x00

          ===>Video Control Extension Unit Descriptor<===
bLength:                           0x1D
bDescriptorType:                   0x24
bDescriptorSubtype:                0x06
bUnitID:                           0x04
guidExtensionCode:                 {63610682-5070-49AB-B8CC-B3855E8D221D}
bNumControls:                      0x19
bNrInPins:                         0x01
===>List of Connected Units and Terminal ID's
baSourceID[1]:                     0x03
bControlSize:                      0x04
bmControls : 0xFF 0xFF 0x77 0x07 
     D00 = 1  yes -  Vendor-Specific (Optional)
     D01 = 1  yes -  Vendor-Specific (Optional)
     D02 = 1  yes -  Vendor-Specific (Optional)
     D03 = 1  yes -  Vendor-Specific (Optional)
     D04 = 1  yes -  Vendor-Specific (Optional)
     D05 = 1  yes -  Vendor-Specific (Optional)
     D06 = 1  yes -  Vendor-Specific (Optional)
     D07 = 1  yes -  Vendor-Specific (Optional)
     D08 = 1  yes -  Vendor-Specific (Optional)
     D09 = 1  yes -  Vendor-Specific (Optional)
     D10 = 1  yes -  Vendor-Specific (Optional)
     D11 = 1  yes -  Vendor-Specific (Optional)
     D12 = 1  yes -  Vendor-Specific (Optional)
     D13 = 1  yes -  Vendor-Specific (Optional)
     D14 = 1  yes -  Vendor-Specific (Optional)
     D15 = 1  yes -  Vendor-Specific (Optional)
     D16 = 1  yes -  Vendor-Specific (Optional)
     D17 = 1  yes -  Vendor-Specific (Optional)
     D18 = 1  yes -  Vendor-Specific (Optional)
     D19 = 0   no -  Vendor-Specific (Optional)
     D20 = 1  yes -  Vendor-Specific (Optional)
     D21 = 1  yes -  Vendor-Specific (Optional)
     D22 = 1  yes -  Vendor-Specific (Optional)
     D23 = 0   no -  Vendor-Specific (Optional)
     D24 = 1  yes -  Vendor-Specific (Optional)
     D25 = 1  yes -  Vendor-Specific (Optional)
     D26 = 1  yes -  Vendor-Specific (Optional)
     D27 = 0   no -  Vendor-Specific (Optional)
     D28 = 0   no -  Vendor-Specific (Optional)
     D29 = 0   no -  Vendor-Specific (Optional)
     D30 = 0   no -  Vendor-Specific (Optional)
     D31 = 0   no -  Vendor-Specific (Optional)
iExtension:                        0x00

          ===>Video Control Output Terminal Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x24
bDescriptorSubtype:                0x03
bTerminalID:                       0x05
wTerminalType:                   0x0101 = (TT_STREAMING)
bAssocTerminal:                    0x00
bSourceID:                         0x04
iTerminal:                         0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x87  -> Direction: IN - EndpointID: 7
bmAttributes:                      0x03  -> Interrupt Transfer Type
wMaxPacketSize:                  0x0010 = 1 transactions per microframe, 0x10 max bytes
bInterval:                         0x08

          ===>Class-specific VC Interrupt Endpoint Descriptor<===
bLength:                           0x05 
bDescriptorType:                   0x25
bDescriptorSubtype:                0x03
wMaxTransferSize:                0x0405 = (1029) Bytes

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x00
bNumEndpoints:                     0x00
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Video Class-Specific VS Video Input Header Descriptor<===
bLength:                           0x0F
bDescriptorType:                   0x24
bDescriptorSubtype:                0x01
bNumFormats:                       0x02
wTotalLength:                    0x01A6  -> Validated
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmInfo:                            0x00  -> Dynamic Format Change not Supported
bTerminalLink:                     0x05
bStillCaptureMethod:               0x02  -> Still Capture Method 2
bTriggerSupport:                   0x00  -> No Hardware Triggering Support
bTriggerUsage:                     0x00
bControlSize:                      0x01
Video Payload Format 1             0x04 
     D00 = 0   no -  Key Frame Rate
     D01 = 0   no -  P Frame Rate
     D02 = 1  yes -  Compression Quality
     D03 = 0   no -  Compression Window Size
     D04 = 0   no -  Generate Key Frame
     D05 = 0   no -  Update Frame Segment
     D06 = 0   no -  Reserved
     D07 = 0   no -  Reserved
Video Payload Format 2             0x00 
     D00 = 0   no -  Key Frame Rate
     D01 = 0   no -  P Frame Rate
     D02 = 0   no -  Compression Quality
     D03 = 0   no -  Compression Window Size
     D04 = 0   no -  Generate Key Frame
     D05 = 0   no -  Update Frame Segment
     D06 = 0   no -  Reserved
     D07 = 0   no -  Reserved

          ===>Video Streaming MJPEG Format Type Descriptor<===
bLength:                           0x0B
bDescriptorType:                   0x24
bDescriptorSubtype:                0x06
bFormatIndex:                      0x01
bNumFrameDescriptors:              0x05
bmFlags:                           0x01  -> Sample Size is Fixed
bDefaultFrameIndex:                0x01
bAspectRatioX:                     0x00
bAspectRatioY:                     0x00
bmInterlaceFlags:                  0x00
     D00   = 0  non-Interlaced stream or variable
     D01   = 0  2 fields per frame
     D02   = 0  Field 1 not first
     D03   = 0  Reserved
     D4..5 = 0  Field patterns  -> Field 1 only
     D6..7 = 0  Display Mode  -> Bob only
bCopyProtect:                      0x00  -> Duplication Unrestricted

          ===>Video Streaming MJPEG Frame Type Descriptor<===
          --->This is the Default (optimum) Frame index
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x07
bFrameIndex:                       0x01
bmCapabilities:                    0x00
wWidth:                          0x0500 = 1280
wHeight:                         0x02D0 = 720
dwMinBitRate:                0x0D2F0000
dwMaxBitRate:                0x0D2F0000
dwMaxVideoFrameBufferSize:   0x001C2000
dwDefaultFrameInterval:      0x000A2C2A = 66.666600 mSec (15.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame TypeData
dwFrameInterval[1]:          0x000A2C2A = 66.666600 mSec (15.00 Hz)

          ===>Video Streaming MJPEG Frame Type Descriptor<===
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x07
bFrameIndex:                       0x02
bmCapabilities:                    0x00
wWidth:                          0x0500 = 1280
wHeight:                         0x02C8 = 712
dwMinBitRate:                0x0D098000
dwMaxBitRate:                0x0D098000
dwMaxVideoFrameBufferSize:   0x001BD000
dwDefaultFrameInterval:      0x000A2C2A = 66.666600 mSec (15.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame TypeData
dwFrameInterval[1]:          0x000A2C2A = 66.666600 mSec (15.00 Hz)

          ===>Video Streaming MJPEG Frame Type Descriptor<===
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x07
bFrameIndex:                       0x03
bmCapabilities:                    0x00
wWidth:                          0x0500 = 1280
wHeight:                         0x01E0 = 480
dwMinBitRate:                0x0BB80000
dwMaxBitRate:                0x0BB80000
dwMaxVideoFrameBufferSize:   0x0012C000
dwDefaultFrameInterval:      0x0007A120 = 50.000000 mSec (20.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame TypeData
dwFrameInterval[1]:          0x0007A120 = 50.000000 mSec (20.00 Hz)

          ===>Video Streaming MJPEG Frame Type Descriptor<===
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x07
bFrameIndex:                       0x04
bmCapabilities:                    0x00
wWidth:                          0x0280 = 640
wHeight:                         0x01E0 = 480
dwMinBitRate:                0x08CA0000
dwMaxBitRate:                0x08CA0000
dwMaxVideoFrameBufferSize:   0x00096000
dwDefaultFrameInterval:      0x00051615 = 33.333300 mSec (30.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame TypeData
dwFrameInterval[1]:          0x00051615 = 33.333300 mSec (30.00 Hz)

          ===>Video Streaming MJPEG Frame Type Descriptor<===
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x07
bFrameIndex:                       0x05
bmCapabilities:                    0x00
wWidth:                          0x0280 = 640
wHeight:                         0x01D8 = 472
dwMinBitRate:                0x08A48000
dwMaxBitRate:                0x08A48000
dwMaxVideoFrameBufferSize:   0x00093800
dwDefaultFrameInterval:      0x00051615 = 33.333300 mSec (30.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame TypeData
dwFrameInterval[1]:          0x00051615 = 33.333300 mSec (30.00 Hz)

          ===>Still Image Frame Type Descriptor<===
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x03
bEndpointAddress:                  0x00
bNumImageSizePatterns:             0x05
wWidth[1]:                       0x0500
wHeight[1]:                      0x02D0
wWidth[2]:                       0x0500
wHeight[2]:                      0x02C8
wWidth[3]:                       0x0500
wHeight[3]:                      0x01E0
wWidth[4]:                       0x0280
wHeight[4]:                      0x01E0
wWidth[5]:                       0x0280
wHeight[5]:                      0x01D8
bNumCompressionPattern:            0x04
bCompression[1]:                   0x01
bCompression[2]:                   0x05
bCompression[3]:                   0x0A
bCompression[4]:                   0x14


          ===>Color Matching Descriptor<===
bLength:                           0x06
bDescriptorType:                   0x24
bDescriptorSubtype:                0x0D
bColorPrimaries:                   0x01
bTransferCharacteristics:          0x01
bMatrixCoefficients:               0x04

          ===>Video Streaming Uncompressed Format Type Descriptor<===
bLength:                           0x1B
bDescriptorType:                   0x24
bDescriptorSubtype:                0x04
bFormatIndex:                      0x02
bNumFrameDescriptors:              0x05
guidFormat:                        {32595559-0000-0010-8000-00AA00389B71} = YUY2 Format
bBitsPerPixel:                     0x10
bDefaultFrameIndex:                0x01
bAspectRatioX:                     0x00
bAspectRatioY:                     0x00
bmInterlaceFlags:                  0x00
     D0    = 0x00 Interlaced stream or variable: No
     D1    = 0x00 Fields per frame: 2 fields
     D2    = 0x00 Field 1 first: No
     D3    = 0x00 Reserved
     D4..5 = 0x00 Field patterns  -> Field 1 only
     D6..7 = 0x00 Display Mode  -> Bob only
bCopyProtect:                      0x00  -> Duplication Unrestricted

          ===>Video Streaming Uncompressed Frame Type Descriptor<===
          --->This is the Default (optimum) Frame index
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x05
bFrameIndex:                       0x01
bmCapabilities:                    0x00
wWidth:                          0x0500 = 1280
wHeight:                         0x02D0 = 720
dwMinBitRate:                0x08CA0000
dwMaxBitRate:                0x08CA0000
dwMaxVideoFrameBufferSize:   0x001C2000
dwDefaultFrameInterval:      0x000F4240 = 100.000000 mSec (10.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame Type Data
dwFrameInterval[1]:          0x000F4240 = 100.000000 mSec (10.00 Hz)

          ===>Video Streaming Uncompressed Frame Type Descriptor<===
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x05
bFrameIndex:                       0x02
bmCapabilities:                    0x00
wWidth:                          0x0500 = 1280
wHeight:                         0x02C8 = 712
dwMinBitRate:                0x08B10000
dwMaxBitRate:                0x08B10000
dwMaxVideoFrameBufferSize:   0x001BD000
dwDefaultFrameInterval:      0x000F4240 = 100.000000 mSec (10.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame Type Data
dwFrameInterval[1]:          0x000F4240 = 100.000000 mSec (10.00 Hz)

          ===>Video Streaming Uncompressed Frame Type Descriptor<===
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x05
bFrameIndex:                       0x03
bmCapabilities:                    0x00
wWidth:                          0x0500 = 1280
wHeight:                         0x01E0 = 480
dwMinBitRate:                0x05DC0000
dwMaxBitRate:                0x05DC0000
dwMaxVideoFrameBufferSize:   0x0012C000
dwDefaultFrameInterval:      0x000F4240 = 100.000000 mSec (10.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame Type Data
dwFrameInterval[1]:          0x000F4240 = 100.000000 mSec (10.00 Hz)

          ===>Video Streaming Uncompressed Frame Type Descriptor<===
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x05
bFrameIndex:                       0x04
bmCapabilities:                    0x00
wWidth:                          0x0280 = 640
wHeight:                         0x01E0 = 480
dwMinBitRate:                0x08CA0000
dwMaxBitRate:                0x08CA0000
dwMaxVideoFrameBufferSize:   0x00096000
dwDefaultFrameInterval:      0x00051615 = 33.333300 mSec (30.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame Type Data
dwFrameInterval[1]:          0x00051615 = 33.333300 mSec (30.00 Hz)

          ===>Video Streaming Uncompressed Frame Type Descriptor<===
bLength:                           0x1E
bDescriptorType:                   0x24
bDescriptorSubtype:                0x05
bFrameIndex:                       0x05
bmCapabilities:                    0x00
wWidth:                          0x0280 = 640
wHeight:                         0x01D8 = 472
dwMinBitRate:                0x08A48000
dwMaxBitRate:                0x08A48000
dwMaxVideoFrameBufferSize:   0x00093800
dwDefaultFrameInterval:      0x00051615 = 33.333300 mSec (30.00 Hz)
bFrameIntervalType:                0x01
===>Additional Discrete Frame Type Data
dwFrameInterval[1]:          0x00051615 = 33.333300 mSec (30.00 Hz)

          ===>Still Image Frame Type Descriptor<===
bLength:                           0x1B
bDescriptorType:                   0x24
bDescriptorSubtype:                0x03
bEndpointAddress:                  0x00
bNumImageSizePatterns:             0x05
wWidth[1]:                       0x0500
wHeight[1]:                      0x02D0
wWidth[2]:                       0x0500
wHeight[2]:                      0x02C8
wWidth[3]:                       0x0500
wHeight[3]:                      0x01E0
wWidth[4]:                       0x0280
wHeight[4]:                      0x01E0
wWidth[5]:                       0x0280
wHeight[5]:                      0x01D8
bNumCompressionPattern:            0x01
bCompression[1]:                   0x01


          ===>Color Matching Descriptor<===
bLength:                           0x06
bDescriptorType:                   0x24
bDescriptorSubtype:                0x0D
bColorPrimaries:                   0x01
bTransferCharacteristics:          0x01
bMatrixCoefficients:               0x04

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x01
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x00C0 = 1 transactions per microframe, 0xC0 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x02
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x0180 = 1 transactions per microframe, 0x180 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x03
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x0200 = 1 transactions per microframe, 0x200 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x04
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x0280 = 1 transactions per microframe, 0x280 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x05
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x0320 = 1 transactions per microframe, 0x320 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x06
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x03B0 = 1 transactions per microframe, 0x3B0 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x07
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x0A80 = 2 transactions per microframe, 0x280 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x08
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x0B20 = 2 transactions per microframe, 0x320 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x09
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x0BE0 = 2 transactions per microframe, 0x3E0 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x0A
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x13C0 = 3 transactions per microframe, 0x3C0 max bytes
bInterval:                         0x01

          ===>Interface Descriptor<===
bLength:                           0x09
bDescriptorType:                   0x04
bInterfaceNumber:                  0x01
bAlternateSetting:                 0x0B
bNumEndpoints:                     0x01
bInterfaceClass:                   0x0E  -> Video Interface Class
bInterfaceSubClass:                0x02  -> Video Streaming Interface SubClass
bInterfaceProtocol:                0x00
iInterface:                        0x00

          ===>Endpoint Descriptor<===
bLength:                           0x07
bDescriptorType:                   0x05
bEndpointAddress:                  0x81  -> Direction: IN - EndpointID: 1
bmAttributes:                      0x05  -> Isochronous Transfer Type, Synchronization Type = Asynchronous, Usage Type = Data Endpoint
wMaxPacketSize:                  0x13FC = 3 transactions per microframe, 0x3FC max bytes
bInterval:                         0x01

          ===>Additional Error Checking<===
PASS: number of uncompressed-frame frame descriptors (5) == number of frame descriptors (5) specified in uncompressed format descriptor(s)
PASS: number of MJPEG frame descriptors (5) == number of frame descriptors (5) specified in MJPEG format descriptor(s)

