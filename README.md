# Titanic 生存分析项目

## 项目介绍

本项目使用 Python 对 Titanic 数据集进行了基础数据分析，探索影响乘客生存率的关键因素。

通过数据清洗、缺失值处理和可视化分析，观察不同特征（如性别、舱位等级等）与生存率之间的关系。

这是我的第一个完整数据分析项目。

---

## 项目目标

本项目主要完成：

- 使用 Pandas 读取和处理数据
- 查看并处理缺失值
- 使用 Seaborn 进行数据可视化
- 分析不同特征对生存率的影响
- 使用 Git 和 GitHub 管理项目

---

## 使用技术

- Python
- Pandas
- Seaborn
- Matplotlib
- Jupyter Notebook
- Git
- GitHub

---

## 数据集来源

Titanic Dataset：

https://www.kaggle.com/competitions/titanic/data

---

## 项目结构

```text
titanic-analysis/
│
├── analysis.ipynb
├── train.csv
├── images/
│   └── survival_by_sex.png
└── README.md
```

---

## 数据分析内容

### 1. 数据读取

使用 Pandas 读取 Titanic CSV 数据：

```python
df = pd.read_csv("train.csv")
```

---

### 2. 数据结构查看

查看：

- 数据行数
- 字段类型
- 缺失值情况

```python
df.info()
```

---

### 3. 缺失值处理

对 Age 列缺失值进行中位数填充：

```python
df["Age"] = df["Age"].fillna(df["Age"].median())
```

---

### 4. 数据可视化

分析性别与生存率关系：

```python
sns.barplot(x="Sex", y="Survived", data=df)
```

---

## 分析结论

### 性别对生存率影响明显

女性乘客生存率明显高于男性乘客。

---

### 舱位等级影响生存率

头等舱乘客生存率更高。

说明社会等级和资源可能影响逃生概率。

---

## 可视化结果

![image](这里粘贴你的图片链接)

---

## 项目收获

通过这个项目，我学习了：

- Python 数据分析基础
- Pandas 数据处理
- 缺失值清洗
- 数据可视化
- Git/GitHub 项目管理
- Notebook 工作流

---

## 后续优化方向

未来计划继续优化：

- 增加更多特征分析
- 尝试机器学习预测
- 添加更多可视化图表
- 提高代码结构化程度

---

## 作者

GitHub：

https://github.com/Pity308
