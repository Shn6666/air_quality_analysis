# 城市空气质量分析 - 快速使用指南

##  一键运行

```bash
# 1. 安装依赖
pip install -r requirements.txt

# 2. 运行分析
python complete_analysis.py
```

## 📊 自动生成的文件

运行后自动生成：
- ✅ 2个数据文件（原始数据 + 清洗后数据）
- ✅ 6个可视化图表
- ✅ 1个分析报告

##  核心文件

只需一个文件：**complete_analysis.py**（26KB）

包含所有功能：
- 数据采集（真实API + 模拟数据）
- 数据清洗（缺失值 + 异常值处理）
- 数据可视化（6个专业图表）
- 数据分析（6条结论 + 5条建议）

##  切换数据源

编辑 `complete_analysis.py` 最后一行：

```python
# 使用真实数据（默认）
analyzer.run(use_real_data=True)

# 使用模拟数据
# analyzer.run(use_real_data=False)
```

##  项目结构

```
air_quality_analysis/
├── complete_analysis.py    ← 只需这个文件！
├── requirements.txt
├── README.md
├── data/                   ← 自动生成的数据
├── output/                 ← 自动生成的图表
└── reports/                ← 自动生成的报告
```

## 💡 特点

- ✅ 单文件运行，无需复杂配置
- ✅ 真实气象数据（Open-Meteo API）
- ✅ 自动备用方案（API失败时切换模拟数据）
- ✅ 完整的数据分析流程
- ✅ 6个专业可视化图表
- ✅ 详细分析报告

##  完成！

现在您只需运行一条命令即可获得完整的空气质量分析报告！
