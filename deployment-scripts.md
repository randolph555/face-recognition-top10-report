# 🚀 人脸识别项目部署脚本集合

> **说明**: 本文档包含前5名人脸识别项目的详细部署脚本，支持多种部署方式。

## 📋 项目列表

1. [ageitgey/face_recognition](#1-ageitgeyface_recognition)
2. [serengil/deepface](#2-serengildeeface)  
3. [justadudewhohacks/face-api.js](#3-justadudewhohacksface-apijs)
4. [cmusatyalab/openface](#4-cmusatyalabopenface)
5. [davidsandberg/facenet](#5-davidsandbergfacenet)

---

## 1. ageitgey/face_recognition

### 🐍 Pip 安装方式
```bash
#!/bin/bash
# ageitgey/face_recognition - pip安装脚本
# 适用平台: macOS, Linux (推荐)

echo "🚀 开始安装 face_recognition..."

# 1. 更新系统包管理器
if [[ "$OSTYPE" == "linux-gnu"* ]]; then
    sudo apt-get update
    sudo apt-get install -y build-essential cmake libopenblas-dev liblapack-dev libx11-dev libgtk-3-dev python3-dev
elif [[ "$OSTYPE" == "darwin"* ]]; then
    brew install cmake
fi

# 2. 安装Python依赖
