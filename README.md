## 介绍
本仓库为面向**华中科技大学电子信息与通信学院WST实验室**自用 Typst 周报模板，因 word 模板不够灵活 + 本人偏爱使用 Typst 进行文档编写而诞生。

## 用法
#### 基础配置
1. git clone 到本地。
2. 使用 vscode + Tinymist 插件进行本地编写，或上传项目文件夹到 Typst webapp 进行编写。
#### 新增周报
1. 切入 reports 目录，新建空白typ文件。
2. 复制 reports/template.typ 内容至该空白 typ 文件。
3. 修改分别向 private-date、private-overview、private-details、private-plans 块填入当前周报日期、概述、详述、下周计划内容。在webapp中可选择对当前周报进行单独预览。
4. 修改 report_yxx_wxx 变量命名为对应周次。
5. 切入项目根目录，编辑 data.typ 文件，import对应新typ文件，并向reports列表加入对应 report_yxx_wxx 变量。
6. 将main.typ导出为pdf，新周报自动添加到末尾。

## 文件说明
- template.typ: 周报概述模板。
- utils.typ: 工具方法。
- main.typ: 周报概述主体。
- data.typ: 控制显示哪些周次的周报。
- reports/template.typ：单周周报模板。
- reports/report_yxxwxx.typ（或其他名称）：自建的单周周报。