# 训练集
## 1. 1106.xlsx
该文件存储目前的训练集原始数据，其中：question为自然语言问题，keyword为对应的focus关键词，table为对应的表格schema信息。

在训练时，目前会将question和schema组织为提示指令。如：

你是一个经验丰富的数据分析师。根据数据表结构(schema)，你需要将用户的数据查询描述(question)翻译成特定的DSL。\"\"\"schema\"\"\"为数据表结构，包括列名和列的属性，###question###为用户的查询描述。schema:\"\"\"{'部门ID': 'int', '部门名称': 'string', '创建时间': 'string', '排名': 'int', '预算额': 'double', '员工人数': 'double', '负责人ID': 'int', '姓名': 'string', '出生地区': 'string', '年龄': 'double', '临时代理': 'string'}\"\"\"\n---\nquestion:###领导中有多少人年龄大于56岁？###

对应的keyword标签为：
年龄>56   姓名去重后的数量

## 2. extract_keyword_qwen.json
该文件为1106.xlsx中数据被组织成Qwen官方微调格式后的json训练数据。

## 3. extract_keyword_chatglm3.json
该文件为1106.xlsx中数据被组织成chatglm3-6b官方微调格式后的jsonl训练数据。

# 测试集
## 1. benchmark_data.xlsx
该文件存储目前的测试集原始数据。其中，question为自然语言问题，schema为对应表格的模式信息。测试集的标签暂未放置在该文件中，目前根据执行的结果进行评估。
