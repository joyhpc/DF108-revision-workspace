# Decision Summary

- **headline**: 原始工具输出有 40 个 ERROR，但在改版预审口径下被解释为 1 个工具问题、47 个边界/缺证项、0 个命名占位项、9 个封装/符号集成待办；当前不能据此判定原理图存在同等数量的设计错误。
- **interpreted_status**: evidence_open
- **technical_layer**: raw counts: ERROR 40, WARNING 197, INFO 275, skipped 2。解释后：已确认设计错误 0，工具问题 1，边界/缺证项 47，命名占位项 0，封装/符号集成待办 9。
- **decision_layer**: 当前应定义为证据未闭合/判断口径待补强，而不是设计已判错。优先处理 1 个工具问题、47 个边界/缺证项、0 个命名占位项、9 个封装/符号集成待办后复审。
- **raw_review_status**: fail
- **raw_headline**: 发现 40 个必须修复问题，建议在发板或发布前阻断闭环。
- **raw_risk_level**: critical
