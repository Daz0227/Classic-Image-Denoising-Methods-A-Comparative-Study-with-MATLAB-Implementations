# Classic-Image-Denoising-Methods-A-Comparative-Study-with-MATLAB-Implementations

图像去噪算法对比研究框架，提供10种经典去噪方法的完整MATLAB实现与系统化评估工具。


# 📚 方法清单

| 算法类别        | 包含方法                      | 关键特性                         |
|-----------------|-------------------------------|----------------------------------|
| 频域滤波        | Butterworth, Gaussian         | 频带可控/振铃抑制               |
| 空域滤波        | Average, Median, Bilateral    | 实时处理/边缘保持               |
| 形态学操作      | Open-Close, Close-Open        | 结构特征保持                     |
| 统计滤波        | Wiener, Adaptive Median       | 局部统计优化                     |
| 非局部方法      | Non-Local Means (NLM)         | 全局相似性匹配                   |

## 🛠️ 快速开始

### 环境要求
- MATLAB R2023a 或更高版本
- Image Processing Toolbox
- Wavelet Toolbox (仅小波去噪需要)

### 数据准备
1. 创建文件结构：
```bash
mkdir 原始图像
mkdir 乘性噪声
mkdir 高斯噪声
mkdir 椒盐噪声
```
2. 将测试图像（barbara.png, lena.png, peppers256.png）放入`原始图像`目录

### 运行示例
```matlab
% 配置核心参数
selectedMethod = 'butterworth';  % 可替换为gaussian/average等
```

## 📊 性能指标

### PSNR对比（dB）
| 方法          | 高斯噪声 | 椒盐噪声 | 散斑噪声 |
|---------------|----------|----------|----------|
| Butterworth   | 25.5     | 22.7     | 26.1     |
| Adaptive Median| 15.5    | **38.5** | 17.1     |
| NLM           | **26.7** | 26.1     | **26.7** |

## 📜 文献引用

若本项目对您的研究有帮助，请引用：
```bibtex
@software{OpenIDR,
  author = {Dou, Aozhe},
  title = {OpenIDR: Classical Image Denoising Framework},
  year = {2024},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/Daz0227/Classic-Image-Denoising-Methods-A-Comparative-Study-with-MATLAB-Implementations}}
}
```


## 许可证

本项目采用 [MIT License](LICENSE)

---

📧 学术合作联系: [aozhedou@gmail.com](mailto:aozhedou@gmail.com)  
🌐 项目维护: [窦奥喆 @中国石油大学（华东）](https://www.upc.edu.cn)
```
