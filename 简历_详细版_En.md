# Zheng Enci - Personal Resume

**Full-Stack AI Application Development**

---

## Contact Information

- **Email**: zheng_enci@qq.com
- **GitHub**: https://github.com/Zheng-Enci
- **Gitee**: https://gitee.com/zheng-enci050704
- **GitCode**: https://gitcode.com/ZhengEnCi
- **Juejin**: https://juejin.cn/user/2883382090934252
- **CSDN**: https://blog.csdn.net/2301_79239314

---

## Education Background

**2023.09 - 2027.06 (Expected)** | **Xiamen Institute of Technology, School of Artificial Intelligence** | Bachelor's Degree

- **Major**: Software Engineering (AI Direction)
- **Research Focus**: Full-stack AI application development, intelligent vision technology R&D, deep learning model design and optimization, multimodal large model application integration

---

## Core Skills

### Programming Languages
- **Python**: PyTorch, OpenCV, Flask
- **Java**: Spring Boot, Spring Security
- **JavaScript/TypeScript**: Vue3, Node.js

### Frontend Technologies
- **Frameworks**: Vue3 (Composition API), Element Plus
- **Visualization**: ECharts, Fabric.js, Canvas API

### Backend Technologies
- **Frameworks**: Spring Boot 3.x, Spring Security, Flask, Spring WebFlux
- **API Design**: RESTful API, JWT authentication, WebSocket

### AI/Machine Learning
- **Computer Vision**: YOLO, ResNet, object detection, behavior recognition, image stitching
- **Large Language Models**: Multimodal large model applications, Tongyi Qianwen, Zidong Taichu

### Database & Operations
- **Databases**: MySQL, PostgreSQL, Redis, SQL optimization, MinIO file storage
- **Deployment & Operations**: Docker, Nginx, Git, Linux/Ubuntu, intranet penetration, Spring Scheduler

---

## Internship Experience

### Xiamen Hongchen Network Technology Co., Ltd. | Full-Stack Developer | 2024.08

- **Rapidly built** the foundational framework for a human resource management information system, covering core modules including employee management, attendance clock-in, department management, and implementing dual-role permission systems for administrators and employees
- **Designed and implemented** JWT Token authentication mechanism to ensure system security; utilized Vue3 + Element Plus + Spring Boot + MyBatis + MySQL technology stack to complete basic system functionality development
- **Quickly mastered** enterprise-level technology stacks including Spring Boot, MyBatis, Vue3, and gained deep understanding of frontend-backend separation architecture and RESTful API design specifications through practical projects

---

## Project Experience

### Student Management System | 2025.09 - 2026.03

**Project Background**: Developed an integrated student management system for Xiamen Institute of Technology AI Creation Workshop to address issues such as irregular student information management, lack of time-based attendance restrictions, and absence of data visualization.

**Tech Stack**: Vue3 + Spring Boot 3.x + MySQL + Redis + Nginx

**Project Achievements**:
- **Independently completed full-stack development**: Responsible for frontend and backend architecture design and implementation, covering **7 core modules** including student information management, time-based attendance, data visualization
- **Security mechanism design**: Implemented triple security mechanism with JWT authentication + IP whitelist + CAPTCHA verification, **effectively preventing attendance fraud**
- **Performance optimization**: Optimized response time to **under 100ms** through Redis caching of attendance status; implemented on-demand component loading, **significantly reducing bundle size**
- **User experience optimization**: Redesigned attendance correction process as step-by-step workflow, supporting Chinese date picker, large screen adaptation, dark mode
- **System deployment**: Successfully deployed and launched, supporting multi-user concurrent access, **stable operation in production environment**
- **March 2026 feature expansion**: Added invitation code management system, data download functionality, verification code system refactoring, **further enhancing system security**
- **Project Link**: https://10257qh6684dd.vicp.fun/ | **Open Source Code**: GitHub/Gitee/GitCode (frontend open source)

---

### Hongxing Farm Corn Germination Monitoring System (Agricultural Academy Project) | 2025.10 - 2025.11

**Project Background**: Commissioned by the Agricultural Academy to develop a corn germination monitoring system for Beidahuang Group Beian Branch, addressing the difficulty of manual field inspection in timely identifying missing seedling areas.

**Tech Stack**: HTML5/CSS3 + Fabric.js + JavaScript + YOLO data parsing

**Project Achievements**:
- Independently completed Canvas rendering, detection data parsing, interactive logic and UX optimization, parsed YOLO annotation files, aggregated seedling points by grid and generated heatmap views
- Implemented multi-parameter adjustment for grid size/rotation/translation, adapted to irregular field ridges, **row spacing error controlled within 5 pixels**
- Developed manual correction functionality, forming "algorithm detection + manual review" closed-loop, integrated germination rate calculation panel to assist farm owners in precise decision-making
- **Compressed drone collection→image stitching→detection→grid heatmap→manual review workflow to under 10 minutes, significantly improving field inspection efficiency**
- **Open Source Code**: GitHub/Gitee/GitCode

---

### Classroom Abnormal Behavior Detection System (EduBot) | 2025.03 - 2025.04

**Project Background**: School AI education reform project addressing the difficulty of real-time detection of behaviors such as lying on desks, using phones, standing, and looking up in classrooms.

**Tech Stack**: PyTorch + YOLOv8n + Flask + MySQL + Tongyi Qianwen/Zidong Taichu

**Project Achievements**:
- Used LabelImg to build **Xiamen Institute of Technology Classroom Personnel Detection Dataset** (YOLO format), compared multiple YOLO model versions, selected YOLOv8n for training specialized model
- Developed proprietary behavior binary classification model using PyTorch, innovatively implemented "YOLO person detection + proprietary model behavior judgment" detection logic, **model accuracy significantly better than generic models**, accurately identifying 4 target behavior types
- Independently completed full-stack development including frontend, backend, and model management three parts, integrated large language models for PPTX to mind map conversion, lesson plan generation and other functions
- Project received **National College Student Innovation and Entrepreneurship Training Program approval** (Project No.: 202513115006)
- Applied for **invention patent** (Third Inventor): Classroom behavior detection method based on multimodal large models (CN202510645941.9)
- **Open Source Code**: GitHub/Gitee/GitCode (frontend and backend open source)

---

### CAS Urban Environment High-altitude Camera Multi-image Stitching System | 2025.06 - 2025.07

**Project Background**: Commissioned by CAS Institute of Urban Environment to develop a deep learning-based image stitching system for high-altitude camera multi-video stream fusion needs, addressing the accuracy limitations of traditional image stitching methods in complex scenarios, achieving high-quality seamless stitching of multi-camera video streams.

**Tech Stack**: PyTorch + ResNet50 + OpenCV + CUDA GPU acceleration

**Project Achievements**:
- Conducted secondary development based on GitHub open source project, **extracted core code and optimized architecture**, refactored image stitching logic
- Designed **multi-image stitching algorithm**, expanded from original project's 2-image stitching capability to support 4-5 image stitching
- Optimized **dual-branch regression network**, separately predicting homography transformation parameters and TPS grid deformation parameters, achieving joint optimization of two transformations
- Implemented complete end-to-end image stitching workflow (preprocessing→feature extraction→transformation prediction→image transformation→image fusion→post-processing), **significantly improved stitching accuracy compared to traditional methods**, providing technical support for urban environment monitoring

---

### 3D Reconstruction Full-process File Management System | 2025.09 - 2025.11

**Project Background**: Addressing 3D reconstruction project full-process management needs, developed a complete full-process intelligent management system for step-by-step workflow coordination, file upload/download within processes, and process occupancy task coordination.

**Tech Stack**: Vue3 + TypeScript + Spring Boot 3.5.5 + PostgreSQL

**Project Achievements**:
- Independently completed frontend and backend architecture design, implemented **five-step process management** (data collection→frame extraction collection→reconstruction collection→Gaussian splatting→model polishing)
- Designed **hierarchical file storage architecture**, storing files in separate folders by process steps (Videos, Frames, Rebuild, 3dgs, plys)
- Implemented **task coordination mechanism** and **hierarchical permission management**, supporting process occupancy mechanism and exception appeal handling
- Integrated **unified authentication platform**, supported large file uploads (maximum 2GB), implemented complete task lifecycle management

---

### ROS Full-Stack Autonomous Control Car | 2025.04

**Project Background**: Aimed at implementing remote car camera viewing and control through relay server, building a complete ROS full-stack autonomous control solution to meet remote monitoring and car control requirements.

**Tech Stack**: Flask + ROS + OpenCV + Digua Robot + RDKx5 Development Board

**Project Achievements**:
- Implemented remote car monitoring and control functionality based on relay server, established full-link communication and control from client web page to car hardware
- Car end running on Ubuntu system, clients viewing car camera feed in real-time through web page and sending control commands
- Successfully integrated ROS system with web technology, implemented frontend and backend server code development and car control code

---

### Intelligent Monitoring System | 2025.09 - 2026.02

**Project Background**: Xiamen Institute of Technology AI Creation Workshop required an intelligent monitoring system adapted to its scenario characteristics, addressing screen change detection and timeline storage needs.

**Tech Stack**: Python + OpenCV + imagehash

**Project Achievements**:
- Implemented screen change detection and timeline storage, achieved screen change detection through frame hash calculation
- Supported multi-threaded parallel monitoring of 3 Hikvision network cameras, stored by timeline path
- Implemented automatic disk space management (automatic image cleanup), automatic reconnection on disconnection, non-blocking startup and other fault tolerance mechanisms
- **Open Source Code**: GitHub/Gitee/GitCode

---

### IP Monitoring System | 2025.12

**Project Background**: Addressing IP conflict issues caused by manual IP address configuration in Xiamen Institute of Technology AI Creation Workshop network environment, independently developed IP monitoring system to implement data-driven IP allocation strategy.

**Tech Stack**: Flask + Python threading + HTML/CSS/JavaScript

**Project Achievements**:
- Implemented automatic network scanning, IP statistics visualization, interactive filtering and other functions
- Improved scanning efficiency through multi-threaded concurrent ping, visualized IP usage frequency using heatmaps
- Helped administrators understand IP usage frequency, prioritized assigning low-usage IP addresses to new devices to avoid IP conflicts
- **Open Source Code**: GitHub/Gitee/GitCode

---

## Awards & Honors

### Project Approval
- **2025.09** | **National College Student Innovation and Entrepreneurship Training Program** Approval | Project No.: 202513115006 | Project Name: EduBot - Creator of New Educational Forms

### Patent Achievements
- **2025.05** | **Invention Patent** (Third Inventor): Classroom behavior detection method based on multimodal large models
    - Application No.: CN202510645941.9 | Publication No.: CN120183048A
    - Technical Field: Multimodal large models, object detection, face recognition, behavior analysis
    - Personal Contribution: Participated in core algorithm design, technical solution and experimental verification

- **2025.09** | **Invention Patent** (Second Inventor): Student behavior detection system and method based on classroom monitoring
    - Application No.: CN202511244232.6 | Publication No.: CN121095547A
    - Technical Field: Computer vision, behavior detection, deep learning
    - Personal Contribution: Participated in overall system design, algorithm development and implementation

### Technical Community Achievements
- **2025.11** | **Juejin Quality Author Ranking 2nd Place** (2025 Issue 11)
    - 123 quality articles | 111 collections
    - Heat: 438, second only to JD Cloud official account

---

## Technical Highlights

1. **Full-stack development capability**: Independently completed frontend and backend architecture design and development, proficient in Vue3, Spring Boot, Flask and other technology stacks, completed multiple full-stack projects covering enterprise management systems, AI application systems and other fields

2. **AI model development**: Designed and trained specialized deep learning detection models, used PyTorch, YOLO and other frameworks, model accuracy better than generic models, successfully applied to practical scenarios such as classroom behavior detection, agricultural monitoring, received national innovation project approval and invention patents

3. **Performance optimization capability**: Optimized system performance through Redis caching, on-demand loading and other technologies, achieved real-time data dashboard update delay **<1 second**

4. **Project implementation capability**: Independently completed full process from requirements analysis, architecture design to deployment, multiple projects successfully launched and operating, including student management system, CAS image stitching system, agricultural academy monitoring system, etc.

5. **Problem-solving capability**: Designed and implemented JWT authentication + IP whitelist dual security mechanism, effectively preventing attendance fraud; solved performance bottlenecks in high-concurrency scenarios, optimized data loading efficiency through parallel loading strategies; independently solved image stitching accuracy issues, controlled row spacing error within 5 pixels

6. **UI/UX optimization capability**: Implemented enterprise-level UI component optimization (Chinese date picker, large screen standard adaptation), adopted card layout, gradient backgrounds, dark mode and other modern designs, improved user experience and interface aesthetics, followed enterprise development best practices

---

## Self-Evaluation

Possess the ability to **independently complete projects**, capable of independently handling the entire process from requirements analysis, architecture design to development and deployment, with good **problem-solving skills** and **technical optimization capabilities**. **Continuously learning new technologies**, able to quickly master and apply to practical projects, innovatively applying new technologies in projects, achieving results such as **national innovation project approval** and **invention patents**. Possess good **team collaboration skills** and **communication skills**, able to efficiently cooperate with team members to achieve project goals, with strong **stress resistance** and **adaptability**, able to maintain high productivity in fast-paced work environments.

---