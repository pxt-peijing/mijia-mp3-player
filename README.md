# MakerBit MP3

[![Build Status](https://travis-ci.org/1010Technologies/pxt-makerbit-mp3.svg?branch=master)](https://travis-ci.org/1010Technologies/pxt-makerbit-mp3)

米加智造micro:bit音乐播放器模块。

## 说明

米加盒子提供micro:bit所有周边产品，包括micr:bit主板、扩展板、传感器、显示设备、电机、舵机及输入输出附件。

米加智造micro:bit音乐播放器模块，配合micro:bit，可以制作一个MP3播放器，实现音乐播放的功能，包括播放、暂停、上一区、下一区、音量调节，并且可以与音箱相连接。

https://www.mijiahezi.com/microbit-mp3-player.html
                                |

## 功能说明

音乐模块需要配合micr SD卡使用，使用前请将SD卡格式化为FAT32，另外，文件夹及文件名请遵循如下的结构和标准：


- 文件夹必须是两位的数字, 例如： `01`。（不包括引号）
- 文件夹内的音频文件名称必须是3位数字开头，例如： `001.mp3`（不包括引号），支持mp3、wav两种文件格式。

最多支持99个文件夹，255个音频文件。

```
├── 01/
│   ├── 001.mp3
│   ├── 002 second track.mp3
│   └── 003 third track.mp3
├── 02/
│   ├── 001.mp3
│   └── 002.mp3
│
…
```

MP3音频播放模块根据字母顺序读取文件和文件夹，需要提前创建好文件夹，如：01、02、03等，并从001开始命名文件夹中的音频文件曲目，顺序中不能出现跳跃，一定要按照顺序，因为这些名称可以用在扩展中的功能调用中。

如果在播放过程中有问题，请检查全名是否有问题。

通过micro:bit技术支持社区提问，https://www.mijiahezi.com/community
