# 鼠标和键盘模拟项目

## 项目概述
基于USB Gadget HID协议的鼠标和键盘模拟项目，适用于RK3588等Linux开发板，提供RESTful API控制鼠标移动和键盘输入。

## 项目结构

### 核心模块
- **技术栈**：FastAPI + Flask + Python + USB Gadget HID
- **核心功能**：鼠标控制API、键盘服务、USB HID设备配置
- **详细信息**：查看 [开发日志](2026/03/README.md)

## 核心功能
- 鼠标任意方向移动（x、y坐标控制）
- 键盘短按/长按按键
- 字符串发送功能
- 统一API响应格式

## 开发历程
- **2026年3月**：项目初始化，实现鼠标API和键盘服务

## 项目链接
- **GitHub**: https://github.com/Zheng-Enci/mouse-and-keyboard-simulation
- **Gitee**: https://gitee.com/zheng-enci050704/mouse-and-keyboard-simulation
- **GitCode**: https://gitcode.com/ZhengEnCi/mouse-and-keyboard-simulation

## 硬件要求
- RK3588或其他支持USB Gadget的Linux开发板
- Ubuntu 20.04+或其他主流Linux发行版
- 支持USB Gadget HID功能的内核

## 快速开始
```bash
# 安装依赖
python install_requirements.py

# 配置HID设备
sudo bash Note/LinYuDong/setup_hid_gadget.sh

# 启动鼠标API
cd services/mouse_api && sudo python3 mouse_api.py

# 启动键盘服务
cd services/keyboard_service && python3 keyboard_service.py
```