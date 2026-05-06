# Decision Summary

- **project_id**: DF108
- **project_type**: board
- **status**: fail
- **risk_level**: critical
- **headline**: 发现 40 个必须修复问题，建议在发板或发布前阻断闭环。
- **technical_layer**: 本次运行 6 个引擎，ERROR 40 项，WARNING 197 项，INFO 275 项。
- **decision_layer**: 当前状态为 fail，存在必须修复项；不建议进入发板、发布或正式关闭。
- **must_fix_count**: 40
- **should_fix_count**: 197
- **manual_review_count**: 275
- **executed_engines**: ["power_tree", "rule_engine_v3", "semantic_v4", "board_review", "constraint_checker", "emc_checker"]
- **skipped_engines**: ["constraint_checker", "emc_checker"]
