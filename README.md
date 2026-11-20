# My-Python-Learning-Journey
## 项目简介
本仓库用于存放Python课程练习代码，记录Python基础语法、pandas数据处理相关练习。本次练习实现两个小功能：一是使用pandas创建学生成绩数据表，实现结构化数据存储与打印；二是使用f-string格式化字符串，实现变量嵌入文本、简单数值计算输出，用来熟悉Python基础数据处理与字符串输出写法。

## 文件说明
- `python_homework.ipynb`：本次课堂练习Jupyter笔记本文件，包含2段练习代码，可直接运行查看输出结果。

## 代码说明
```python
# pandas部分：导入库，构造学生成绩表格，打印表格
import pandas as pd
df = pd.DataFrame({
    '语文':[110,105,109],
    '数学':[105,88,120],
    '英语':[99,115,130],
    '班级':'高一7班'
},index=[0,1,2])
print(df)
# f-string部分：格式化字符串，把变量和计算结果嵌入文本
name = "小明"
age = 25
msg = f"你好,{name}。你今年{age}岁。"
print(msg)
print(f"计算结果：{24 * 8 + 4}")
