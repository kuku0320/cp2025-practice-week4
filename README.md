# 计算物理实践 - 第四周作业

本仓库包含计算物理实践课程第四周的编程作业，涵盖多个物理模型的数值模拟与数据分析。

## 目录结构
```
cp2025-practice-week4/
├── data/                      # 数据文件目录
│   ├── g149novickA.txt        # 细菌生长实验数据
│   ├── g149novickB.txt        # 细菌生长实验数据
│   ├── HIVseries.csv          # HIV病毒载量数据
│   └── millikan.txt           # 光电效应实验数据
├── src/                       # 源代码目录（学生实现）
│   ├── bacteria_model_student.py  # 细菌生长模型
│   ├── hiv_model_student.py       # HIV病毒载量模型
│   ├── logistic_map.py            # Logistic映射模型
│   └── millikan_fit.py            # 光电效应数据分析
├── solutions/                 # 参考解答目录
│   ├── bacteria_model_solution.py
│   ├── hiv_model_solution.py
│   ├── logistic_map_solution.py
│   └── millikan_fit_solution.py
├── tests/                     # 测试文件目录
│   ├── test_bacteria_model.py
│   ├── test_hiv_model.py
│   ├── test_logistic.py
│   └── test_millikan.py
├── docs/                      # 文档目录
│   ├── Logistic映射与混沌系统研究.md
│   ├── 细菌生长模型研究.md
│   ├── HIV病毒载量模型研究.md
│   └── 光电效应实验数据分析.md
├── .github/                   # GitHub配置目录
│   └── workflows/             # GitHub Actions工作流
│       └── classroom.yml      # 自动评分配置
├── requirements.txt           # 项目依赖
└── README.md                  # 本文件
```

## 作业内容

本次作业包含四个独立的物理模型实现：

1. **Logistic映射与混沌系统研究**：实现Logistic映射模型，研究确定性混沌现象。
2. **细菌生长模型**：实现并分析细菌生长的数学模型。
3. **HIV病毒载量模型**：模拟HIV病毒在体内的动态变化。
4. **光电效应实验数据分析**：使用最小二乘法拟合光电效应实验数据，计算普朗克常量。

## 使用说明

### 环境配置

```bash
# 安装依赖
pip install -r requirements.txt
```

### 运行测试
```
# 运行所有测试
python -m pytest tests/

# 运行特定测试
python -m pytest tests/test_logistic.py -v
```
### 提交作业
1. 完成 src/ 目录下的所有实现文件
2. 确保所有测试通过
3. 提交到GitHub仓库

## 评分标准
每个模型实现占10分，总分40分。评分将通过自动测试完成，测试通过即得满分。

## 参考资料
- 《计算物理建模初学者指南》
- 课程讲义和示例代码
