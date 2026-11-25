# 科创企业研发与订单融资档案的动态复核

本项目用于整理相关业务资料。CSV 文件采用 UTF-8 编码，首行为字段名，日期使用 ISO 格式；空单元格表示来源未提供。样例记录为合成数据。

## 样例资料

- `rd_projects.csv` 包含样例字段 `project,company,period,rd_budget,spent,stage`。
- `orders.csv` 包含样例字段 `order,company,customer,value,state,delivery_due,acceptance_due`。
- `cash_plan.csv` 包含样例字段 `cash,order,kind,due,amount,certainty`。
- `credit.csv` 包含样例字段 `facility,bank,product,limit,months,security,source_ref`。

## 运行检查

需要 Python 3.11 或更高版本，无第三方依赖。

```bash
python3 -m unittest discover -s tests -v
python3 -m compileall -q tests
```
