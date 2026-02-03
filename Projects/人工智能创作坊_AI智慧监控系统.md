## 2025-9-3 | 开启人工智能创作坊・AI 智慧监控系统项目

### 项目背景
厦门工学院人工智能创作坊需配套一套适配其场景特性的智慧监控系统。当前，随着人工智能技术的持续迭代与深度应用，监控系统的功能边界不断拓展，对其智能化决策能力、精准化识别效率、高效化响应机制的要求也随之显著提升。

### 最初需求
有画面变化的时候存储，可以按时间轴效果展示存储内容，其他需求后续待定。

### 监控设备
两个海康威视 DS-2DE3Q140MY-T/GLSE 4mm 网络摄像机。

### 架构设计
项目分两个大部分：
1. 监控摄像保存：对有画面变化的图像进行存储，并按时间轴存储，技术上使用Python和opencv-python进行图像处理。
2. 智慧监控全栈系统（含前端与后端）：
   - 前端：Vue3、Element Plus、Vite、WebSocket、Pinia、Vue Router
   - 后端：Spring Boot 3.x、Spring WebFlux、MySQL + MinIO、Spring Security + JWT、Spring Scheduler

### 环境与依赖
- Python 3.13 + Anaconda 虚拟环境
- 依赖：tqdm==4.67.1、opencv-python==4.12.0.88、imagehash==4.3.2（清华源安装，多线程并行安装）

### 核心代码要点
- 配置类 `Config`：获取项目根目录；摄像头配置列表（RTSP地址、位置、哈希阈值）
- 摄像头处理类 `HikvisionDS2DE3Q140MYTGLSE4mmNetworkCamera`：帧哈希计算、秒级去重、画面变化按时间轴保存、日志记录
- 启动脚本：多线程运行双摄像头，按时间轴路径存储 `static/images/位置/年/月/日/时/分/秒.jpg`

### 现有功能覆盖
1. 画面变化存储：通过 `imagehash` 计算帧哈希值，差值大于阈值时保存
2. 时间轴存储：按时间路径层级保存
3. 双摄像头并行：多线程并行监控与存储
4. 日志记录：帧读取失败时记录时间+位置+错误

### Git初始化与推送
- 仓库：`https://gitee.com/zheng-enci050704/aismart-surveillance-system-project_-save_the_surveillance_image.git`
- 步骤：git init → git add . → git remote add origin … → git commit "First edition" → git push -u origin master

---

## 2025-9-5 （本科三年级）| 人工智能创作坊・AI 智慧监控系统项目代码优化

### 核心优化方向
针对海康威视摄像头数据采集稳定性、依赖安装效率及系统鲁棒性进行代码迭代。

### 关键优化
1. 连接与帧读取容错：断连自动重连；读取失败 sleep(1) 重试
2. 依赖安装脚本：线程锁 + 进度条同步；清华源可配置；自动创建 logs 目录
3. 参数与状态管理：记录 rtsp_url；初始哈希值有效赋值，避免计算异常

### 价值
提升系统稳定性、降低部署门槛、保障画面变化检测准确性。

### 地点
厦门工学院人工智能创作坊

---


## 2025-9-8 （本科三年级）| 人工智能创作坊・AI 智慧监控系统项目迭代（新增摄像头配置与版本控制优化）

### 项目背景
在既有智慧监控系统上新增1台海康摄像机并完成版本控制。

### 核心操作
1. 摄像头扩展：`camera_url_and_location` 增加 DS-2DE3Q140MY-T/GLSE 4mm（Outside_104，RTSP地址，哈希阈值2），实现3台并行监控
2. Git权限与身份：safe.directory 设置；git user.email/user.name 配置
3. 版本控制：两次提交与推送（新增摄像头配置；位置修正），推送至远程仓库

### 技术栈/工具
Python、Git、Windows PowerShell、海康威视网络摄像机

### 项目成果
监控设备扩展至3台（Hall、Inside_106、Outside_104）；解决权限与身份配置，保证迭代可追溯。

### 地点
厦门工学院人工智能创作坊

---
## 2026年2月2日 | 人工智能创作坊・AI 智慧监控系统项目优化（v1.0.0）

### 更新类型
代码优化

### 更新内容
1. **添加高质量代码注释**：为项目所有Python源代码文件添加详细中文注释，提升可读性与可维护性
2. **完善项目文档**：更新README.md，添加项目介绍、快速开始、配置说明、技术实现等内容
3. **项目开源**：将项目开源至Gitee平台，开源链接：`https://gitee.com/zheng-enci050704/aismart-surveillance-system-project_-save_the_surveillance_image`
4. **文件修改**：
   - `main.py`：添加模块文档、配置初始化、摄像头实例化、线程创建注释
   - `config.py`：添加模块、类、初始化方法文档及参数说明
   - `install_dependencies.py`：添加模块、安装函数注释及依赖用途说明
   - `models/cameras/hikvision_ds_2de3q140my_t_glse_4mm_camera.py`：添加模块、类、方法文档及感知哈希算法说明
   - `README.md`：完善项目文档结构与内容
   - `Note/UpdateLogs/2026/02/02.md`：创建更新日志文件

### 更新说明
- 统一使用中文注释，覆盖模块、类、方法及行内注释
- 保持原有代码逻辑不变，仅添加注释
- 完善的文档便于项目上手与维护
- 开源发布扩大项目影响力

### 地点
厦门工学院人工智能创作坊

---

## 2026年2月3日 | 人工智能创作坊・AI 智慧监控系统项目功能扩展（v1.1.0）

### 更新类型
功能扩展

### 更新内容
1. **实现图像自动清理功能**：当磁盘剩余空间不足时，自动删除最旧的监控图像，确保系统稳定运行
2. **添加磁盘空间配置**：在`config.py`中新增`min_disk_free_space`（默认50GB）和`check_disk_free_space_interval_seconds`（默认60秒）参数
3. **优化自动重连机制**：移除摄像头初始化时的严格连接检查，支持运行时自动重连
4. **标准化依赖管理**：添加`requirements.txt`文件，包含项目所有依赖包
5. **文件修改**：
   - `utils/image_cleaner.py`：实现`ImageCleaner`类，用于磁盘空间监控与旧图像清理
   - `main.py`：启动图像清理服务线程
   - `config.py`：添加磁盘空间配置参数
   - `models/cameras/hikvision_ds_2de3q140my_t_glse_4mm_camera.py`：优化自动重连机制
   - `requirements.txt`：添加项目依赖包列表
   - `README.md`：更新文档，添加图像清理功能与依赖管理说明

### 核心功能说明
- **ImageCleaner类**：定期检查磁盘空间，低于阈值时自动删除最旧图像，支持自定义参数
- **自动重连机制**：提高系统容错性，单个摄像头连接失败不影响其他摄像头运行
- **依赖管理**：通过`requirements.txt`快速安装项目环境

### 技术栈/工具
Python、OpenCV、ImageHash、Git、Gitee

### 项目成果
- 实现磁盘空间自动管理，避免因空间不足导致监控中断
- 提升系统稳定性与容错性，支持摄像头自动重连
- 标准化依赖管理，降低部署门槛

### 地点
厦门工学院人工智能创作坊

