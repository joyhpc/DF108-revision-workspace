# Engineering Actions

## 1. Board review failed: 'DiffPairCheck' object has no attribute 'pair_name'
- **action_id**: ACT-001
- **priority**: P0
- **action_type**: must_fix
- **source**: board_review
- **rule_id**: ENGINE-ERROR
- **category**: SYSTEM
- **location**: 
- **title**: Board review failed: 'DiffPairCheck' object has no attribute 'pair_name'
- **recommended_action**: 修复后重新运行 sch-review，并确认该项关闭。
- **decision_impact**: SYSTEM 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-001-board_review-ENGINE-ERROR

## 2. 上游未闭合 / 缺测试点 / 外部依赖: A_DC_PWR (0.0V)
- **action_id**: ACT-002
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: A_DC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: A_DC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-002-power_tree-PWR-RISK

## 3. 上游未闭合 / 缺测试点 / 外部依赖: A_POC_PWR (0.0V)
- **action_id**: ACT-003
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: A_POC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: A_POC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-003-power_tree-PWR-RISK

## 4. 上游未闭合 / 缺测试点 / 外部依赖: B_DC_PWR (0.0V)
- **action_id**: ACT-004
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: B_DC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: B_DC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-004-power_tree-PWR-RISK

## 5. 上游未闭合 / 缺测试点 / 外部依赖: B_POC_PWR (0.0V)
- **action_id**: ACT-005
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: B_POC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: B_POC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-005-power_tree-PWR-RISK

## 6. 上游未闭合 / 缺测试点 / 外部依赖: C_DC_PWR (0.0V)
- **action_id**: ACT-006
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: C_DC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: C_DC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-006-power_tree-PWR-RISK

## 7. 上游未闭合 / 缺测试点 / 外部依赖: C_POC_PWR (0.0V)
- **action_id**: ACT-007
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: C_POC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: C_POC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-007-power_tree-PWR-RISK

## 8. 上游未闭合 / 缺测试点 / 外部依赖: D_DC_PWR (0.0V)
- **action_id**: ACT-008
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: D_DC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: D_DC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-008-power_tree-PWR-RISK

## 9. 上游未闭合 / 缺测试点 / 外部依赖: D_POC_PWR (0.0V)
- **action_id**: ACT-009
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: D_POC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: D_POC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-009-power_tree-PWR-RISK

## 10. 上游未闭合 / 缺测试点: EX_IO1_1V8 (1.8V)
- **action_id**: ACT-010
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: EX_IO1_1V8
- **title**: 上游未闭合 / 缺测试点: EX_IO1_1V8 (1.8V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-010-power_tree-PWR-RISK

## 11. 上游未闭合 / 缺测试点: EX_IO2_1V8 (1.8V)
- **action_id**: ACT-011
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: EX_IO2_1V8
- **title**: 上游未闭合 / 缺测试点: EX_IO2_1V8 (1.8V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-011-power_tree-PWR-RISK

## 12. 上游未闭合 / 缺测试点 / 外部依赖: EX_POC_PWR (0.0V)
- **action_id**: ACT-012
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: EX_POC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: EX_POC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-012-power_tree-PWR-RISK

## 13. 上游未闭合 / 缺测试点 / 外部依赖: E_DC_PWR (0.0V)
- **action_id**: ACT-013
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: E_DC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: E_DC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-013-power_tree-PWR-RISK

## 14. 上游未闭合 / 缺测试点 / 外部依赖: E_POC_PWR (0.0V)
- **action_id**: ACT-014
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: E_POC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: E_POC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-014-power_tree-PWR-RISK

## 15. 上游未闭合 / 缺测试点 / 外部依赖: FAN_12V (12.0V)
- **action_id**: ACT-015
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: FAN_12V
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: FAN_12V (12.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-015-power_tree-PWR-RISK

## 16. 上游未闭合 / 缺测试点: FPGA_1V8 (1.8V)
- **action_id**: ACT-016
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: FPGA_1V8
- **title**: 上游未闭合 / 缺测试点: FPGA_1V8 (1.8V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-016-power_tree-PWR-RISK

## 17. 上游未闭合 / 缺测试点 / 外部依赖: F_DC_PWR (0.0V)
- **action_id**: ACT-017
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: F_DC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: F_DC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-017-power_tree-PWR-RISK

## 18. 上游未闭合 / 缺测试点 / 外部依赖: F_POC_PWR (0.0V)
- **action_id**: ACT-018
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: F_POC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: F_POC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-018-power_tree-PWR-RISK

## 19. 上游未闭合 / 缺测试点 / 外部依赖: G_DC_PWR (0.0V)
- **action_id**: ACT-019
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: G_DC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: G_DC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-019-power_tree-PWR-RISK

## 20. 上游未闭合 / 缺测试点 / 外部依赖: G_POC_PWR (0.0V)
- **action_id**: ACT-020
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: G_POC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: G_POC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-020-power_tree-PWR-RISK

## 21. 上游未闭合 / 缺测试点 / 外部依赖: H_DC_PWR (0.0V)
- **action_id**: ACT-021
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: H_DC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: H_DC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-021-power_tree-PWR-RISK

## 22. 上游未闭合 / 缺测试点 / 外部依赖: H_POC_PWR (0.0V)
- **action_id**: ACT-022
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: H_POC_PWR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: H_POC_PWR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-022-power_tree-PWR-RISK

## 23. 上游未闭合: M1V8 (1.8V)
- **action_id**: ACT-023
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: M1V8
- **title**: 上游未闭合: M1V8 (1.8V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-023-power_tree-PWR-RISK

## 24. 上游未闭合: M24V (24.0V)
- **action_id**: ACT-024
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: M24V
- **title**: 上游未闭合: M24V (24.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-024-power_tree-PWR-RISK

## 25. 上游未闭合 / 缺测试点: MGTVCCAUX_R (0.0V)
- **action_id**: ACT-025
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: MGTVCCAUX_R
- **title**: 上游未闭合 / 缺测试点: MGTVCCAUX_R (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-025-power_tree-PWR-RISK

## 26. 上游未闭合 / 缺测试点: UART_RX_F/EX_IO3_1V8 (1.8V)
- **action_id**: ACT-026
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: UART_RX_F/EX_IO3_1V8
- **title**: 上游未闭合 / 缺测试点: UART_RX_F/EX_IO3_1V8 (1.8V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-026-power_tree-PWR-RISK

## 27. 上游未闭合 / 缺测试点: UART_TX_F/EX_IO4_1V8 (1.8V)
- **action_id**: ACT-027
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: UART_TX_F/EX_IO4_1V8
- **title**: 上游未闭合 / 缺测试点: UART_TX_F/EX_IO4_1V8 (1.8V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-027-power_tree-PWR-RISK

## 28. 上游未闭合 / 缺测试点 / 外部依赖: VCC1 (1.0V)
- **action_id**: ACT-028
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: VCC1
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: VCC1 (1.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-028-power_tree-PWR-RISK

## 29. 上游未闭合 / 缺测试点: VCCAUX (0.0V)
- **action_id**: ACT-029
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: VCCAUX
- **title**: 上游未闭合 / 缺测试点: VCCAUX (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-029-power_tree-PWR-RISK

## 30. 上游未闭合 / 缺测试点 / 外部依赖: VCCR (0.0V)
- **action_id**: ACT-030
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: VCCR
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: VCCR (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-030-power_tree-PWR-RISK

## 31. 上游未闭合 / 缺测试点 / 外部依赖: VCCT (0.0V)
- **action_id**: ACT-031
- **priority**: P0
- **action_type**: must_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: VCCT
- **title**: 上游未闭合 / 缺测试点 / 外部依赖: VCCT (0.0V)
- **recommended_action**: 检查电源链路完整性
- **decision_impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-031-power_tree-PWR-RISK

## 32. U9 没有连接到 GND
- **action_id**: ACT-032
- **priority**: P0
- **action_type**: must_fix
- **source**: rule_engine_v3
- **rule_id**: PI.ic_grounding
- **category**: PI
- **location**: 
- **title**: U9 没有连接到 GND
- **recommended_action**: 连接的网络: ['NC']
- **decision_impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-032-rule_engine_v3-PI.ic_grounding

## 33. U122 没有连接到任何电源网络
- **action_id**: ACT-033
- **priority**: P0
- **action_type**: must_fix
- **source**: rule_engine_v3
- **rule_id**: PI.ic_power_supply
- **category**: PI
- **location**: 
- **title**: U122 没有连接到任何电源网络
- **recommended_action**: 连接的网络: ['N20359018', 'N20359112', 'NC', 'S3V3']
- **decision_impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-033-rule_engine_v3-PI.ic_power_supply

## 34. U123 没有连接到任何电源网络
- **action_id**: ACT-034
- **priority**: P0
- **action_type**: must_fix
- **source**: rule_engine_v3
- **rule_id**: PI.ic_power_supply
- **category**: PI
- **location**: 
- **title**: U123 没有连接到任何电源网络
- **recommended_action**: 连接的网络: ['N20361029', 'N20361040', 'N20361064', 'NC']
- **decision_impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-034-rule_engine_v3-PI.ic_power_supply

## 35. U124 没有连接到任何电源网络
- **action_id**: ACT-035
- **priority**: P0
- **action_type**: must_fix
- **source**: rule_engine_v3
- **rule_id**: PI.ic_power_supply
- **category**: PI
- **location**: 
- **title**: U124 没有连接到任何电源网络
- **recommended_action**: 连接的网络: ['N20360328', 'N20360401', 'N20360576', 'POW_EN', 'S3V3']
- **decision_impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-035-rule_engine_v3-PI.ic_power_supply

## 36. U125 没有连接到任何电源网络
- **action_id**: ACT-036
- **priority**: P0
- **action_type**: must_fix
- **source**: rule_engine_v3
- **rule_id**: PI.ic_power_supply
- **category**: PI
- **location**: 
- **title**: U125 没有连接到任何电源网络
- **recommended_action**: 连接的网络: ['POW_EN', 'POW_EN1', 'POW_EN2', 'POW_EN3', 'S3V3']
- **decision_impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-036-rule_engine_v3-PI.ic_power_supply

## 37. U260 没有连接到任何电源网络
- **action_id**: ACT-037
- **priority**: P0
- **action_type**: must_fix
- **source**: rule_engine_v3
- **rule_id**: PI.ic_power_supply
- **category**: PI
- **location**: 
- **title**: U260 没有连接到任何电源网络
- **recommended_action**: 连接的网络: ['EX_POC_VOLTAGE_TEST', 'N25616805', 'N25642853', 'NC']
- **decision_impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-037-rule_engine_v3-PI.ic_power_supply

## 38. U1 没有连接到任何电源网络
- **action_id**: ACT-038
- **priority**: P0
- **action_type**: must_fix
- **source**: rule_engine_v3
- **rule_id**: PI.ic_power_supply
- **category**: PI
- **location**: 
- **title**: U1 没有连接到任何电源网络
- **recommended_action**: 连接的网络: ['N20357505', 'N20357507']
- **decision_impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-038-rule_engine_v3-PI.ic_power_supply

## 39. U154 没有连接到任何电源网络
- **action_id**: ACT-039
- **priority**: P0
- **action_type**: must_fix
- **source**: rule_engine_v3
- **rule_id**: PI.ic_power_supply
- **category**: PI
- **location**: 
- **title**: U154 没有连接到任何电源网络
- **recommended_action**: 连接的网络: ['EX_POC_AMP_SCL', 'EX_POC_AMP_SDA', 'N25558477', 'N25582134']
- **decision_impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-039-rule_engine_v3-PI.ic_power_supply

## 40. U9 没有连接到任何电源网络
- **action_id**: ACT-040
- **priority**: P0
- **action_type**: must_fix
- **source**: rule_engine_v3
- **rule_id**: PI.ic_power_supply
- **category**: PI
- **location**: 
- **title**: U9 没有连接到任何电源网络
- **recommended_action**: 连接的网络: ['NC']
- **decision_impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **evidence_id**: EVID-040-rule_engine_v3-PI.ic_power_supply

## 41. 缺测试点 / 外部依赖: 24_VIN (24.0V)
- **action_id**: ACT-041
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: 24_VIN
- **title**: 缺测试点 / 外部依赖: 24_VIN (24.0V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-041-power_tree-PWR-RISK

## 42. 缺测试点: DDR4_VDD (1.2V)
- **action_id**: ACT-042
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: DDR4_VDD
- **title**: 缺测试点: DDR4_VDD (1.2V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-042-power_tree-PWR-RISK

## 43. 缺测试点: FPGA_1V2 (1.2V)
- **action_id**: ACT-043
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: FPGA_1V2
- **title**: 缺测试点: FPGA_1V2 (1.2V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-043-power_tree-PWR-RISK

## 44. 缺测试点: FPGA_3V3 (3.3V)
- **action_id**: ACT-044
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: FPGA_3V3
- **title**: 缺测试点: FPGA_3V3 (3.3V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-044-power_tree-PWR-RISK

## 45. 缺测试点: M3V3 (3.3V)
- **action_id**: ACT-045
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: M3V3
- **title**: 缺测试点: M3V3 (3.3V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-045-power_tree-PWR-RISK

## 46. 缺测试点: M5V (5.0V)
- **action_id**: ACT-046
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: M5V
- **title**: 缺测试点: M5V (5.0V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-046-power_tree-PWR-RISK

## 47. 缺测试点: M5V_A-D (5.0V)
- **action_id**: ACT-047
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: M5V_A-D
- **title**: 缺测试点: M5V_A-D (5.0V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-047-power_tree-PWR-RISK

## 48. 缺测试点: M5V_E-H (5.0V)
- **action_id**: ACT-048
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: M5V_E-H
- **title**: 缺测试点: M5V_E-H (5.0V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-048-power_tree-PWR-RISK

## 49. 缺测试点: MGTAVCC_L (1.0V)
- **action_id**: ACT-049
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: MGTAVCC_L
- **title**: 缺测试点: MGTAVCC_L (1.0V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-049-power_tree-PWR-RISK

## 50. 缺测试点: MGTAVCC_R (1.0V)
- **action_id**: ACT-050
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: MGTAVCC_R
- **title**: 缺测试点: MGTAVCC_R (1.0V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-050-power_tree-PWR-RISK

## 51. 缺测试点: PMU1_VDDIO (3.3V)
- **action_id**: ACT-051
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: PMU1_VDDIO
- **title**: 缺测试点: PMU1_VDDIO (3.3V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-051-power_tree-PWR-RISK

## 52. 缺测试点: PMU2_VDDIO (3.3V)
- **action_id**: ACT-052
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: PMU2_VDDIO
- **title**: 缺测试点: PMU2_VDDIO (3.3V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-052-power_tree-PWR-RISK

## 53. 缺测试点: VCCINT (0.95V)
- **action_id**: ACT-053
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: VCCINT
- **title**: 缺测试点: VCCINT (0.95V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-053-power_tree-PWR-RISK

## 54. 缺测试点: VDDIO_A-D (3.3V)
- **action_id**: ACT-054
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: VDDIO_A-D
- **title**: 缺测试点: VDDIO_A-D (3.3V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-054-power_tree-PWR-RISK

## 55. 缺测试点: VDDIO_B6465 (3.3V)
- **action_id**: ACT-055
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: VDDIO_B6465
- **title**: 缺测试点: VDDIO_B6465 (3.3V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-055-power_tree-PWR-RISK

## 56. 缺测试点: VDDIO_E-H (3.3V)
- **action_id**: ACT-056
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: VDDIO_E-H
- **title**: 缺测试点: VDDIO_E-H (3.3V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-056-power_tree-PWR-RISK

## 57. 缺测试点: VDDIO_OUT (3.3V)
- **action_id**: ACT-057
- **priority**: P1
- **action_type**: should_fix
- **source**: power_tree
- **rule_id**: PWR-RISK
- **category**: POWER
- **location**: VDDIO_OUT
- **title**: 缺测试点: VDDIO_OUT (3.3V)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-057-power_tree-PWR-RISK

## 58. 电路有 34 个独立分量（可能有断开的子电路）
- **action_id**: ACT-058
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.connected_components
- **category**: CONN
- **location**: 
- **title**: 电路有 34 个独立分量（可能有断开的子电路）
- **recommended_action**: 分量大小: [2630, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-058-rule_engine_v3-CONN.connected_components

## 59. U14.IO_L12P_T1U_N10_GC_A08_D24_65/H: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-059
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U14.IO_L12P_T1U_N10_GC_A08_D24_65/H: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-059-rule_engine_v3-CONN.device_id_pins

## 60. U14.IO_T0U_N12_A28_65/HR: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-060
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U14.IO_T0U_N12_A28_65/HR: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-060-rule_engine_v3-CONN.device_id_pins

## 61. U44.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-061
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U44.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-061-rule_engine_v3-CONN.device_id_pins

## 62. U44.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-062
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U44.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-062-rule_engine_v3-CONN.device_id_pins

## 63. U36.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-063
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U36.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-063-rule_engine_v3-CONN.device_id_pins

## 64. U36.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-064
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U36.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-064-rule_engine_v3-CONN.device_id_pins

## 65. U105.A2: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-065
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U105.A2: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-065-rule_engine_v3-CONN.device_id_pins

## 66. U56.A0+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-066
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U56.A0+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-066-rule_engine_v3-CONN.device_id_pins

## 67. U56.A0-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-067
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U56.A0-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-067-rule_engine_v3-CONN.device_id_pins

## 68. U16.A2: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-068
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U16.A2: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-068-rule_engine_v3-CONN.device_id_pins

## 69. U18.A2: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-069
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U18.A2: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-069-rule_engine_v3-CONN.device_id_pins

## 70. U69.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-070
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U69.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-070-rule_engine_v3-CONN.device_id_pins

## 71. U69.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-071
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U69.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-071-rule_engine_v3-CONN.device_id_pins

## 72. U37.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-072
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U37.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-072-rule_engine_v3-CONN.device_id_pins

## 73. U37.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-073
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U37.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-073-rule_engine_v3-CONN.device_id_pins

## 74. U62.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-074
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U62.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-074-rule_engine_v3-CONN.device_id_pins

## 75. U62.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-075
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U62.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-075-rule_engine_v3-CONN.device_id_pins

## 76. U91.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-076
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U91.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-076-rule_engine_v3-CONN.device_id_pins

## 77. U91.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-077
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U91.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-077-rule_engine_v3-CONN.device_id_pins

## 78. U58.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-078
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U58.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-078-rule_engine_v3-CONN.device_id_pins

## 79. U58.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-079
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U58.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-079-rule_engine_v3-CONN.device_id_pins

## 80. U32.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-080
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U32.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-080-rule_engine_v3-CONN.device_id_pins

## 81. U32.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-081
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U32.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-081-rule_engine_v3-CONN.device_id_pins

## 82. U63.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-082
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U63.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-082-rule_engine_v3-CONN.device_id_pins

## 83. U63.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-083
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U63.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-083-rule_engine_v3-CONN.device_id_pins

## 84. U53.A1+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-084
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U53.A1+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-084-rule_engine_v3-CONN.device_id_pins

## 85. U53.A1-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-085
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U53.A1-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-085-rule_engine_v3-CONN.device_id_pins

## 86. U93.A0+: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-086
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U93.A0+: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-086-rule_engine_v3-CONN.device_id_pins

## 87. U93.A0-: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-087
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U93.A0-: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-087-rule_engine_v3-CONN.device_id_pins

## 88. U9.APROBE_GTSL1A_CH3,BA107: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-088
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.APROBE_GTSL1A_CH3,BA107: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-088-rule_engine_v3-CONN.device_id_pins

## 89. U9.APROBE_GTSR4A_CH3,BA29: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-089
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.APROBE_GTSR4A_CH3,BA29: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-089-rule_engine_v3-CONN.device_id_pins

## 90. U9.DNU,BA104: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-090
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.DNU,BA104: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-090-rule_engine_v3-CONN.device_id_pins

## 91. U9.GND,A103: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-091
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,A103: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-091-rule_engine_v3-CONN.device_id_pins

## 92. U9.GND,A119: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-092
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,A119: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-092-rule_engine_v3-CONN.device_id_pins

## 93. U9.GND,A132: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-093
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,A132: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-093-rule_engine_v3-CONN.device_id_pins

## 94. U9.GND,A134: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-094
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,A134: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-094-rule_engine_v3-CONN.device_id_pins

## 95. U9.GND,A26: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-095
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,A26: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-095-rule_engine_v3-CONN.device_id_pins

## 96. U9.GND,AA134: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-096
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,AA134: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-096-rule_engine_v3-CONN.device_id_pins

## 97. U9.GND,AA2: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-097
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,AA2: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-097-rule_engine_v3-CONN.device_id_pins

## 98. U9.GND,BA1: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-098
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA1: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-098-rule_engine_v3-CONN.device_id_pins

## 99. U9.GND,BA100: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-099
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA100: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-099-rule_engine_v3-CONN.device_id_pins

## 100. U9.GND,BA111: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-100
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA111: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-100-rule_engine_v3-CONN.device_id_pins

## 101. U9.GND,BA115: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-101
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA115: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-101-rule_engine_v3-CONN.device_id_pins

## 102. U9.GND,BA120: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-102
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA120: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-102-rule_engine_v3-CONN.device_id_pins

## 103. U9.GND,BA123: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-103
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA123: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-103-rule_engine_v3-CONN.device_id_pins

## 104. U9.GND,BA13: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-104
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA13: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-104-rule_engine_v3-CONN.device_id_pins

## 105. U9.GND,BA131: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-105
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA131: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-105-rule_engine_v3-CONN.device_id_pins

## 106. U9.GND,BA133: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-106
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA133: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-106-rule_engine_v3-CONN.device_id_pins

## 107. U9.GND,BA135: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-107
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA135: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-107-rule_engine_v3-CONN.device_id_pins

## 108. U9.GND,BA16: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-108
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA16: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-108-rule_engine_v3-CONN.device_id_pins

## 109. U9.GND,BA21: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-109
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA21: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-109-rule_engine_v3-CONN.device_id_pins

## 110. U9.GND,BA25: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-110
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,BA25: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-110-rule_engine_v3-CONN.device_id_pins

## 111. U9.GND,CA19: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-111
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,CA19: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-111-rule_engine_v3-CONN.device_id_pins

## 112. U9.GND,CA28: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-112
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GND,CA28: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-112-rule_engine_v3-CONN.device_id_pins

## 113. U9.GTSL1B_TX_CH2N,BA126: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-113
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GTSL1B_TX_CH2N,BA126: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-113-rule_engine_v3-CONN.device_id_pins

## 114. U9.GTSL1B_TX_CH2P,BA129: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-114
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GTSL1B_TX_CH2P,BA129: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-114-rule_engine_v3-CONN.device_id_pins

## 115. U9.GTSR4B_TX_CH2N,BA10: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-115
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.GTSR4B_TX_CH2N,BA10: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-115-rule_engine_v3-CONN.device_id_pins

## 116. U9.NC,AA1: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-116
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.NC,AA1: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-116-rule_engine_v3-CONN.device_id_pins

## 117. U9.NC,AA135: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-117
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.NC,AA135: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-117-rule_engine_v3-CONN.device_id_pins

## 118. U9.SDM_IO1,AVSTX8_DATA2,AS_DATA1: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-118
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.SDM_IO1,AVSTX8_DATA2,AS_DATA1: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-118-rule_engine_v3-CONN.device_id_pins

## 119. U9.SDM_IO11,AVSTX8_VALID,PWRMGT_SD: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-119
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.SDM_IO11,AVSTX8_VALID,PWRMGT_SD: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-119-rule_engine_v3-CONN.device_id_pins

## 120. U9.SDM_IO2,AVSTX8_DATA0,AS_CLK: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-120
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.SDM_IO2,AVSTX8_DATA0,AS_CLK: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-120-rule_engine_v3-CONN.device_id_pins

## 121. U9.SDM_IO3,AVSTX8_DATA3,AS_DATA2: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-121
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.SDM_IO3,AVSTX8_DATA3,AS_DATA2: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-121-rule_engine_v3-CONN.device_id_pins

## 122. U9.SDM_IO4,AVSTX8_DATA1,AS_DATA0: 地址/ID 引脚未连接 (NC)
- **action_id**: ACT-122
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.device_id_pins
- **category**: CONN
- **location**: 
- **title**: U9.SDM_IO4,AVSTX8_DATA1,AS_DATA0: 地址/ID 引脚未连接 (NC)
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-122-rule_engine_v3-CONN.device_id_pins

## 123. J20 只连接到 GND（可能未连接）
- **action_id**: ACT-123
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J20 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-123-rule_engine_v3-CONN.isolated_devices

## 124. J21 只连接到 GND（可能未连接）
- **action_id**: ACT-124
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J21 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-124-rule_engine_v3-CONN.isolated_devices

## 125. J22 只连接到 GND（可能未连接）
- **action_id**: ACT-125
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J22 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-125-rule_engine_v3-CONN.isolated_devices

## 126. J23 只连接到 GND（可能未连接）
- **action_id**: ACT-126
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J23 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-126-rule_engine_v3-CONN.isolated_devices

## 127. J24 只连接到 GND（可能未连接）
- **action_id**: ACT-127
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J24 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-127-rule_engine_v3-CONN.isolated_devices

## 128. J25 只连接到 GND（可能未连接）
- **action_id**: ACT-128
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J25 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-128-rule_engine_v3-CONN.isolated_devices

## 129. J26 只连接到 GND（可能未连接）
- **action_id**: ACT-129
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J26 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-129-rule_engine_v3-CONN.isolated_devices

## 130. J27 只连接到 GND（可能未连接）
- **action_id**: ACT-130
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J27 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-130-rule_engine_v3-CONN.isolated_devices

## 131. J28 只连接到 GND（可能未连接）
- **action_id**: ACT-131
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J28 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-131-rule_engine_v3-CONN.isolated_devices

## 132. J16 只连接到 GND（可能未连接）
- **action_id**: ACT-132
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J16 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-132-rule_engine_v3-CONN.isolated_devices

## 133. J17 只连接到 GND（可能未连接）
- **action_id**: ACT-133
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: J17 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-133-rule_engine_v3-CONN.isolated_devices

## 134. P1 只连接到 GND（可能未连接）
- **action_id**: ACT-134
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: P1 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-134-rule_engine_v3-CONN.isolated_devices

## 135. P2 只连接到 GND（可能未连接）
- **action_id**: ACT-135
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.isolated_devices
- **category**: CONN
- **location**: 
- **title**: P2 只连接到 GND（可能未连接）
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-135-rule_engine_v3-CONN.isolated_devices

## 136. 网络 DDR4_DQS_P2: 多个输出引脚冲突 — U14.IO_L16P_T2U_N6_QBC_AD3P_44/HP, U5.LDQS_T
- **action_id**: ACT-136
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 DDR4_DQS_P2: 多个输出引脚冲突 — U14.IO_L16P_T2U_N6_QBC_AD3P_44/HP, U5.LDQS_T
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-136-rule_engine_v3-CONN.output_conflict

## 137. 网络 DDR4_DQS_N2: 多个输出引脚冲突 — U14.IO_L16N_T2U_N7_QBC_AD3N_44/HP, U5.LDQS_C
- **action_id**: ACT-137
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 DDR4_DQS_N2: 多个输出引脚冲突 — U14.IO_L16N_T2U_N7_QBC_AD3N_44/HP, U5.LDQS_C
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-137-rule_engine_v3-CONN.output_conflict

## 138. 网络 MA_BF_D_D3_HS_P: 多个输出引脚冲突 — U14.IO_L10P_T1U_N6_QBC_AD4P_48/HP, U25.OUT+
- **action_id**: ACT-138
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 MA_BF_D_D3_HS_P: 多个输出引脚冲突 — U14.IO_L10P_T1U_N6_QBC_AD4P_48/HP, U25.OUT+
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-138-rule_engine_v3-CONN.output_conflict

## 139. 网络 DDR4_DQS_P1: 多个输出引脚冲突 — U14.IO_L10P_T1U_N6_QBC_AD4P_44/HP, U6.UDQS_T
- **action_id**: ACT-139
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 DDR4_DQS_P1: 多个输出引脚冲突 — U14.IO_L10P_T1U_N6_QBC_AD4P_44/HP, U6.UDQS_T
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-139-rule_engine_v3-CONN.output_conflict

## 140. 网络 DDR4_DQS_N1: 多个输出引脚冲突 — U14.IO_L10N_T1U_N7_QBC_AD4N_44/HP, U6.UDQS_C
- **action_id**: ACT-140
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 DDR4_DQS_N1: 多个输出引脚冲突 — U14.IO_L10N_T1U_N7_QBC_AD4N_44/HP, U6.UDQS_C
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-140-rule_engine_v3-CONN.output_conflict

## 141. 网络 DDR4_DQS_P5: 多个输出引脚冲突 — U14.IO_L10P_T1U_N6_QBC_AD4P_46/HP, U4.UDQS_T
- **action_id**: ACT-141
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 DDR4_DQS_P5: 多个输出引脚冲突 — U14.IO_L10P_T1U_N6_QBC_AD4P_46/HP, U4.UDQS_T
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-141-rule_engine_v3-CONN.output_conflict

## 142. 网络 DDR4_DQS_N5: 多个输出引脚冲突 — U14.IO_L10N_T1U_N7_QBC_AD4N_46/HP, U4.UDQS_C
- **action_id**: ACT-142
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 DDR4_DQS_N5: 多个输出引脚冲突 — U14.IO_L10N_T1U_N7_QBC_AD4N_46/HP, U4.UDQS_C
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-142-rule_engine_v3-CONN.output_conflict

## 143. 网络 MA_BF_D_D3_HS_N: 多个输出引脚冲突 — U14.IO_L10N_T1U_N7_QBC_AD4N_48/HP, U25.OUT-
- **action_id**: ACT-143
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 MA_BF_D_D3_HS_N: 多个输出引脚冲突 — U14.IO_L10N_T1U_N7_QBC_AD4N_48/HP, U25.OUT-
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-143-rule_engine_v3-CONN.output_conflict

## 144. 网络 DDR4_DQS_P6: 多个输出引脚冲突 — U14.IO_L16P_T2U_N6_QBC_AD3P_46/HP, U3.LDQS_T
- **action_id**: ACT-144
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 DDR4_DQS_P6: 多个输出引脚冲突 — U14.IO_L16P_T2U_N6_QBC_AD3P_46/HP, U3.LDQS_T
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-144-rule_engine_v3-CONN.output_conflict

## 145. 网络 DDR4_DQS_N6: 多个输出引脚冲突 — U14.IO_L16N_T2U_N7_QBC_AD3N_46/HP, U3.LDQS_C
- **action_id**: ACT-145
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.output_conflict
- **category**: CONN
- **location**: 
- **title**: 网络 DDR4_DQS_N6: 多个输出引脚冲突 — U14.IO_L16N_T2U_N7_QBC_AD3N_46/HP, U3.LDQS_C
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-145-rule_engine_v3-CONN.output_conflict

## 146. 网络 ME_SERDES_D3_HS_N: 输入引脚 U14.MGTHRXN2_228/GTH 可能无驱动源
- **action_id**: ACT-146
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 ME_SERDES_D3_HS_N: 输入引脚 U14.MGTHRXN2_228/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-146-rule_engine_v3-CONN.undriven_inputs

## 147. 网络 ME_SERDES_D0_HS_P: 输入引脚 U14.MGTHRXP1_228/GTH 可能无驱动源
- **action_id**: ACT-147
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 ME_SERDES_D0_HS_P: 输入引脚 U14.MGTHRXP1_228/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-147-rule_engine_v3-CONN.undriven_inputs

## 148. 网络 ME_SERDES_D0_HS_N: 输入引脚 U14.MGTHRXN1_228/GTH 可能无驱动源
- **action_id**: ACT-148
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 ME_SERDES_D0_HS_N: 输入引脚 U14.MGTHRXN1_228/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-148-rule_engine_v3-CONN.undriven_inputs

## 149. 网络 ME_SERDES_D2_HS_P: 输入引脚 U14.MGTHRXP3_228/GTH 可能无驱动源
- **action_id**: ACT-149
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 ME_SERDES_D2_HS_P: 输入引脚 U14.MGTHRXP3_228/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-149-rule_engine_v3-CONN.undriven_inputs

## 150. 网络 ME_SERDES_D2_HS_N: 输入引脚 U14.MGTHRXN3_228/GTH 可能无驱动源
- **action_id**: ACT-150
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 ME_SERDES_D2_HS_N: 输入引脚 U14.MGTHRXN3_228/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-150-rule_engine_v3-CONN.undriven_inputs

## 151. 网络 MF_SERDES_D0_HS_P: 输入引脚 U14.MGTHRXP3_227/GTH 可能无驱动源
- **action_id**: ACT-151
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 MF_SERDES_D0_HS_P: 输入引脚 U14.MGTHRXP3_227/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-151-rule_engine_v3-CONN.undriven_inputs

## 152. 网络 MF_SERDES_D0_HS_N: 输入引脚 U14.MGTHRXN3_227/GTH 可能无驱动源
- **action_id**: ACT-152
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 MF_SERDES_D0_HS_N: 输入引脚 U14.MGTHRXN3_227/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-152-rule_engine_v3-CONN.undriven_inputs

## 153. 网络 MF_SERDES_D2_HS_P: 输入引脚 U14.MGTHRXP1_227/GTH 可能无驱动源
- **action_id**: ACT-153
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 MF_SERDES_D2_HS_P: 输入引脚 U14.MGTHRXP1_227/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-153-rule_engine_v3-CONN.undriven_inputs

## 154. 网络 MF_SERDES_D2_HS_N: 输入引脚 U14.MGTHRXN1_227/GTH 可能无驱动源
- **action_id**: ACT-154
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 MF_SERDES_D2_HS_N: 输入引脚 U14.MGTHRXN1_227/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-154-rule_engine_v3-CONN.undriven_inputs

## 155. 网络 MG_SERDES_D1_HS_N: 输入引脚 U14.MGTHRXN3_225/GTH 可能无驱动源
- **action_id**: ACT-155
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: CONN.undriven_inputs
- **category**: CONN
- **location**: 
- **title**: 网络 MG_SERDES_D1_HS_N: 输入引脚 U14.MGTHRXN3_225/GTH 可能无驱动源
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-155-rule_engine_v3-CONN.undriven_inputs

## 156. U122: MCU/FPGA 无调试接口
- **action_id**: ACT-156
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: DBG.debug_interface
- **category**: DBG
- **location**: 
- **title**: U122: MCU/FPGA 无调试接口
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: DBG 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-156-rule_engine_v3-DBG.debug_interface

## 157. A-D_DECODER_5V_EN: 有 1 个 IC 负载但无去耦电容
- **action_id**: ACT-157
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.decoupling_caps
- **category**: PI
- **location**: 
- **title**: A-D_DECODER_5V_EN: 有 1 个 IC 负载但无去耦电容
- **recommended_action**: IC: ['U14']
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-157-rule_engine_v3-PI.decoupling_caps

## 158. A-D_DECODER_VDDIO_EN: 有 1 个 IC 负载但无去耦电容
- **action_id**: ACT-158
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.decoupling_caps
- **category**: PI
- **location**: 
- **title**: A-D_DECODER_VDDIO_EN: 有 1 个 IC 负载但无去耦电容
- **recommended_action**: IC: ['U14']
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-158-rule_engine_v3-PI.decoupling_caps

## 159. E-H_DECODER_5V_EN: 有 1 个 IC 负载但无去耦电容
- **action_id**: ACT-159
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.decoupling_caps
- **category**: PI
- **location**: 
- **title**: E-H_DECODER_5V_EN: 有 1 个 IC 负载但无去耦电容
- **recommended_action**: IC: ['U14']
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-159-rule_engine_v3-PI.decoupling_caps

## 160. E-H__DECODER_VDDIO_EN: 有 1 个 IC 负载但无去耦电容
- **action_id**: ACT-160
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.decoupling_caps
- **category**: PI
- **location**: 
- **title**: E-H__DECODER_VDDIO_EN: 有 1 个 IC 负载但无去耦电容
- **recommended_action**: IC: ['U14']
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-160-rule_engine_v3-PI.decoupling_caps

## 161. EX_IO1_1V8: 有 1 个 IC 负载但无去耦电容
- **action_id**: ACT-161
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.decoupling_caps
- **category**: PI
- **location**: 
- **title**: EX_IO1_1V8: 有 1 个 IC 负载但无去耦电容
- **recommended_action**: IC: ['U14']
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-161-rule_engine_v3-PI.decoupling_caps

## 162. EX_IO2_1V8: 有 1 个 IC 负载但无去耦电容
- **action_id**: ACT-162
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.decoupling_caps
- **category**: PI
- **location**: 
- **title**: EX_IO2_1V8: 有 1 个 IC 负载但无去耦电容
- **recommended_action**: IC: ['U14']
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-162-rule_engine_v3-PI.decoupling_caps

## 163. UART_RX_F/EX_IO3_1V8: 有 2 个 IC 负载但无去耦电容
- **action_id**: ACT-163
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.decoupling_caps
- **category**: PI
- **location**: 
- **title**: UART_RX_F/EX_IO3_1V8: 有 2 个 IC 负载但无去耦电容
- **recommended_action**: IC: ['U14', 'U18']
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-163-rule_engine_v3-PI.decoupling_caps

## 164. UART_TX_F/EX_IO4_1V8: 有 2 个 IC 负载但无去耦电容
- **action_id**: ACT-164
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.decoupling_caps
- **category**: PI
- **location**: 
- **title**: UART_TX_F/EX_IO4_1V8: 有 2 个 IC 负载但无去耦电容
- **recommended_action**: IC: ['U14', 'U16']
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-164-rule_engine_v3-PI.decoupling_caps

## 165. EN 信号 POW_EN2: 连接 3 个 IC 但无滤波电容
- **action_id**: ACT-165
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.enable_pin_filter
- **category**: PI
- **location**: 
- **title**: EN 信号 POW_EN2: 连接 3 个 IC 但无滤波电容
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-165-rule_engine_v3-PI.enable_pin_filter

## 166. EN 信号 POW_EN1: 连接 3 个 IC 但无滤波电容
- **action_id**: ACT-166
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: PI.enable_pin_filter
- **category**: PI
- **location**: 
- **title**: EN 信号 POW_EN1: 连接 3 个 IC 但无滤波电容
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-166-rule_engine_v3-PI.enable_pin_filter

## 167. I2C 网络 A_I2C1_SDA: 未检测到上拉电阻
- **action_id**: ACT-167
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 A_I2C1_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN32', 'RN5']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-167-rule_engine_v3-SI.i2c_pullup

## 168. I2C 网络 A_I2C2_SCL: 未检测到上拉电阻
- **action_id**: ACT-168
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 A_I2C2_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN32', 'RN5']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-168-rule_engine_v3-SI.i2c_pullup

## 169. I2C 网络 A_I2C2_SDA: 未检测到上拉电阻
- **action_id**: ACT-169
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 A_I2C2_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN32', 'RN5']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-169-rule_engine_v3-SI.i2c_pullup

## 170. I2C 网络 H_I2C1_SDA_: 未检测到上拉电阻
- **action_id**: ACT-170
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 H_I2C1_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN41']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-170-rule_engine_v3-SI.i2c_pullup

## 171. I2C 网络 H_I2C1_SCL_: 未检测到上拉电阻
- **action_id**: ACT-171
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 H_I2C1_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN41']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-171-rule_engine_v3-SI.i2c_pullup

## 172. I2C 网络 H_I2C2_SDA_: 未检测到上拉电阻
- **action_id**: ACT-172
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 H_I2C2_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN41']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-172-rule_engine_v3-SI.i2c_pullup

## 173. I2C 网络 H_I2C2_SCL_: 未检测到上拉电阻
- **action_id**: ACT-173
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 H_I2C2_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN41']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-173-rule_engine_v3-SI.i2c_pullup

## 174. I2C 网络 C_I2C1_SCL: 未检测到上拉电阻
- **action_id**: ACT-174
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 C_I2C1_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN33', 'RN34']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-174-rule_engine_v3-SI.i2c_pullup

## 175. I2C 网络 C_I2C1_SDA: 未检测到上拉电阻
- **action_id**: ACT-175
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 C_I2C1_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN33', 'RN34']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-175-rule_engine_v3-SI.i2c_pullup

## 176. I2C 网络 H_I2C2_SDA: 未检测到上拉电阻
- **action_id**: ACT-176
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 H_I2C2_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN36', 'RN41']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-176-rule_engine_v3-SI.i2c_pullup

## 177. I2C 网络 E_I2C1_SCL: 未检测到上拉电阻
- **action_id**: ACT-177
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 E_I2C1_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN31', 'RN35']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-177-rule_engine_v3-SI.i2c_pullup

## 178. I2C 网络 H_I2C2_SCL: 未检测到上拉电阻
- **action_id**: ACT-178
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 H_I2C2_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN36', 'RN41']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-178-rule_engine_v3-SI.i2c_pullup

## 179. I2C 网络 B_I2C1_SDA: 未检测到上拉电阻
- **action_id**: ACT-179
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 B_I2C1_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN37', 'RN38']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-179-rule_engine_v3-SI.i2c_pullup

## 180. I2C 网络 E_I2C1_SDA: 未检测到上拉电阻
- **action_id**: ACT-180
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 E_I2C1_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN31', 'RN35']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-180-rule_engine_v3-SI.i2c_pullup

## 181. I2C 网络 B_I2C1_SCL: 未检测到上拉电阻
- **action_id**: ACT-181
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 B_I2C1_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN37', 'RN38']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-181-rule_engine_v3-SI.i2c_pullup

## 182. I2C 网络 G_I2C1_SDA: 未检测到上拉电阻
- **action_id**: ACT-182
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 G_I2C1_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN30', 'RN4']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-182-rule_engine_v3-SI.i2c_pullup

## 183. I2C 网络 G_I2C1_SCL: 未检测到上拉电阻
- **action_id**: ACT-183
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 G_I2C1_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN30', 'RN4']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-183-rule_engine_v3-SI.i2c_pullup

## 184. I2C 网络 G_I2C2_SCL_: 未检测到上拉电阻
- **action_id**: ACT-184
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 G_I2C2_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN30']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-184-rule_engine_v3-SI.i2c_pullup

## 185. I2C 网络 F_I2C1_SDA_: 未检测到上拉电阻
- **action_id**: ACT-185
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 F_I2C1_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN18']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-185-rule_engine_v3-SI.i2c_pullup

## 186. I2C 网络 F_I2C1_SCL: 未检测到上拉电阻
- **action_id**: ACT-186
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 F_I2C1_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN18', 'RN21']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-186-rule_engine_v3-SI.i2c_pullup

## 187. I2C 网络 F_I2C1_SDA: 未检测到上拉电阻
- **action_id**: ACT-187
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 F_I2C1_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN18', 'RN21']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-187-rule_engine_v3-SI.i2c_pullup

## 188. I2C 网络 F_I2C2_SCL: 未检测到上拉电阻
- **action_id**: ACT-188
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 F_I2C2_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN18', 'RN21']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-188-rule_engine_v3-SI.i2c_pullup

## 189. I2C 网络 F_I2C2_SDA: 未检测到上拉电阻
- **action_id**: ACT-189
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 F_I2C2_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN18', 'RN21']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-189-rule_engine_v3-SI.i2c_pullup

## 190. I2C 网络 G_I2C1_SCL_: 未检测到上拉电阻
- **action_id**: ACT-190
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 G_I2C1_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN30']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-190-rule_engine_v3-SI.i2c_pullup

## 191. I2C 网络 A_I2C1_SCL_: 未检测到上拉电阻
- **action_id**: ACT-191
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 A_I2C1_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN32']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-191-rule_engine_v3-SI.i2c_pullup

## 192. I2C 网络 A_I2C2_SCL_: 未检测到上拉电阻
- **action_id**: ACT-192
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 A_I2C2_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN32']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-192-rule_engine_v3-SI.i2c_pullup

## 193. I2C 网络 D_I2C1_SCL: 未检测到上拉电阻
- **action_id**: ACT-193
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 D_I2C1_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN14', 'RN15']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-193-rule_engine_v3-SI.i2c_pullup

## 194. I2C 网络 H_I2C1_SDA: 未检测到上拉电阻
- **action_id**: ACT-194
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 H_I2C1_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN36', 'RN41']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-194-rule_engine_v3-SI.i2c_pullup

## 195. I2C 网络 D_I2C1_SDA: 未检测到上拉电阻
- **action_id**: ACT-195
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 D_I2C1_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN14', 'RN15']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-195-rule_engine_v3-SI.i2c_pullup

## 196. I2C 网络 H_I2C1_SCL: 未检测到上拉电阻
- **action_id**: ACT-196
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 H_I2C1_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN36', 'RN41']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-196-rule_engine_v3-SI.i2c_pullup

## 197. I2C 网络 B_I2C1_SCL_: 未检测到上拉电阻
- **action_id**: ACT-197
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 B_I2C1_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN38']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-197-rule_engine_v3-SI.i2c_pullup

## 198. I2C 网络 A_I2C1_SDA_: 未检测到上拉电阻
- **action_id**: ACT-198
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 A_I2C1_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN32']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-198-rule_engine_v3-SI.i2c_pullup

## 199. I2C 网络 C_I2C2_SDA: 未检测到上拉电阻
- **action_id**: ACT-199
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 C_I2C2_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN33', 'RN34']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-199-rule_engine_v3-SI.i2c_pullup

## 200. I2C 网络 G_I2C2_SDA_: 未检测到上拉电阻
- **action_id**: ACT-200
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 G_I2C2_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN30']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-200-rule_engine_v3-SI.i2c_pullup

## 201. I2C 网络 C_I2C2_SCL: 未检测到上拉电阻
- **action_id**: ACT-201
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 C_I2C2_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN33', 'RN34']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-201-rule_engine_v3-SI.i2c_pullup

## 202. I2C 网络 D_I2C2_SDA_: 未检测到上拉电阻
- **action_id**: ACT-202
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 D_I2C2_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN15']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-202-rule_engine_v3-SI.i2c_pullup

## 203. I2C 网络 E_I2C1_SCL_: 未检测到上拉电阻
- **action_id**: ACT-203
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 E_I2C1_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN31']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-203-rule_engine_v3-SI.i2c_pullup

## 204. I2C 网络 F_I2C1_SCL_: 未检测到上拉电阻
- **action_id**: ACT-204
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 F_I2C1_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN18']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-204-rule_engine_v3-SI.i2c_pullup

## 205. I2C 网络 F_I2C2_SCL_: 未检测到上拉电阻
- **action_id**: ACT-205
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 F_I2C2_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN18']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-205-rule_engine_v3-SI.i2c_pullup

## 206. I2C 网络 F_I2C2_SDA_: 未检测到上拉电阻
- **action_id**: ACT-206
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 F_I2C2_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN18']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-206-rule_engine_v3-SI.i2c_pullup

## 207. I2C 网络 G_I2C1_SDA_: 未检测到上拉电阻
- **action_id**: ACT-207
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 G_I2C1_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN30']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-207-rule_engine_v3-SI.i2c_pullup

## 208. I2C 网络 B_I2C2_SCL_: 未检测到上拉电阻
- **action_id**: ACT-208
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 B_I2C2_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN38']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-208-rule_engine_v3-SI.i2c_pullup

## 209. I2C 网络 E_I2C2_SCL_: 未检测到上拉电阻
- **action_id**: ACT-209
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 E_I2C2_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN31']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-209-rule_engine_v3-SI.i2c_pullup

## 210. I2C 网络 B_I2C2_SDA_: 未检测到上拉电阻
- **action_id**: ACT-210
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 B_I2C2_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN38']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-210-rule_engine_v3-SI.i2c_pullup

## 211. I2C 网络 B_I2C2_SDA: 未检测到上拉电阻
- **action_id**: ACT-211
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 B_I2C2_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN37', 'RN38']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-211-rule_engine_v3-SI.i2c_pullup

## 212. I2C 网络 C_I2C2_SDA_: 未检测到上拉电阻
- **action_id**: ACT-212
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 C_I2C2_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN33']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-212-rule_engine_v3-SI.i2c_pullup

## 213. I2C 网络 B_I2C2_SCL: 未检测到上拉电阻
- **action_id**: ACT-213
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 B_I2C2_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN37', 'RN38']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-213-rule_engine_v3-SI.i2c_pullup

## 214. I2C 网络 E_I2C2_SDA_: 未检测到上拉电阻
- **action_id**: ACT-214
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 E_I2C2_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN31']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-214-rule_engine_v3-SI.i2c_pullup

## 215. I2C 网络 E_I2C1_SDA_: 未检测到上拉电阻
- **action_id**: ACT-215
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 E_I2C1_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN31']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-215-rule_engine_v3-SI.i2c_pullup

## 216. I2C 网络 D_I2C2_SDA: 未检测到上拉电阻
- **action_id**: ACT-216
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 D_I2C2_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN14', 'RN15']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-216-rule_engine_v3-SI.i2c_pullup

## 217. I2C 网络 B_I2C1_SDA_: 未检测到上拉电阻
- **action_id**: ACT-217
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 B_I2C1_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN38']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-217-rule_engine_v3-SI.i2c_pullup

## 218. I2C 网络 D_I2C2_SCL: 未检测到上拉电阻
- **action_id**: ACT-218
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 D_I2C2_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN14', 'RN15']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-218-rule_engine_v3-SI.i2c_pullup

## 219. I2C 网络 E_I2C2_SDA: 未检测到上拉电阻
- **action_id**: ACT-219
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 E_I2C2_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN31', 'RN35']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-219-rule_engine_v3-SI.i2c_pullup

## 220. I2C 网络 E_I2C2_SCL: 未检测到上拉电阻
- **action_id**: ACT-220
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 E_I2C2_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN31', 'RN35']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-220-rule_engine_v3-SI.i2c_pullup

## 221. I2C 网络 G_I2C2_SDA: 未检测到上拉电阻
- **action_id**: ACT-221
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 G_I2C2_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN30', 'RN4']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-221-rule_engine_v3-SI.i2c_pullup

## 222. I2C 网络 G_I2C2_SCL: 未检测到上拉电阻
- **action_id**: ACT-222
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 G_I2C2_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN30', 'RN4']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-222-rule_engine_v3-SI.i2c_pullup

## 223. I2C 网络 C_I2C2_SCL_: 未检测到上拉电阻
- **action_id**: ACT-223
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 C_I2C2_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN33']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-223-rule_engine_v3-SI.i2c_pullup

## 224. I2C 网络 C_I2C1_SCL_: 未检测到上拉电阻
- **action_id**: ACT-224
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 C_I2C1_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN33']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-224-rule_engine_v3-SI.i2c_pullup

## 225. I2C 网络 QSFP_SDA: 未检测到上拉电阻
- **action_id**: ACT-225
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 QSFP_SDA: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN44']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-225-rule_engine_v3-SI.i2c_pullup

## 226. I2C 网络 QSFP_SCL: 未检测到上拉电阻
- **action_id**: ACT-226
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 QSFP_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN44']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-226-rule_engine_v3-SI.i2c_pullup

## 227. I2C 网络 D_I2C2_SCL_: 未检测到上拉电阻
- **action_id**: ACT-227
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 D_I2C2_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN15']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-227-rule_engine_v3-SI.i2c_pullup

## 228. I2C 网络 C_I2C1_SDA_: 未检测到上拉电阻
- **action_id**: ACT-228
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 C_I2C1_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN33']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-228-rule_engine_v3-SI.i2c_pullup

## 229. I2C 网络 D_I2C1_SDA_: 未检测到上拉电阻
- **action_id**: ACT-229
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 D_I2C1_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN15']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-229-rule_engine_v3-SI.i2c_pullup

## 230. I2C 网络 D_I2C1_SCL_: 未检测到上拉电阻
- **action_id**: ACT-230
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 D_I2C1_SCL_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN15']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-230-rule_engine_v3-SI.i2c_pullup

## 231. I2C 网络 A_I2C2_SDA_: 未检测到上拉电阻
- **action_id**: ACT-231
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 A_I2C2_SDA_: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN32']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-231-rule_engine_v3-SI.i2c_pullup

## 232. I2C 网络 A_I2C1_SCL: 未检测到上拉电阻
- **action_id**: ACT-232
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 A_I2C1_SCL: 未检测到上拉电阻
- **recommended_action**: 网络上的器件: ['RN32', 'RN5']
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-232-rule_engine_v3-SI.i2c_pullup

## 233. 复位网络 /CLK_DIVIDE_RST_: 无上拉/下拉电阻
- **action_id**: ACT-233
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 /CLK_DIVIDE_RST_: 无上拉/下拉电阻
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-233-rule_engine_v3-SI.reset_bias

## 234. 复位网络 PMUBOARD_RST1_: 无上拉/下拉电阻
- **action_id**: ACT-234
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 PMUBOARD_RST1_: 无上拉/下拉电阻
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-234-rule_engine_v3-SI.reset_bias

## 235. 复位网络 PMUBOARD_RST2_: 无上拉/下拉电阻
- **action_id**: ACT-235
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 PMUBOARD_RST2_: 无上拉/下拉电阻
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-235-rule_engine_v3-SI.reset_bias

## 236. 复位网络 WD_POW_RESET: 无上拉/下拉电阻
- **action_id**: ACT-236
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 WD_POW_RESET: 无上拉/下拉电阻
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-236-rule_engine_v3-SI.reset_bias

## 237. 复位网络 QSFP_RESETL_: 无上拉/下拉电阻
- **action_id**: ACT-237
- **priority**: P1
- **action_type**: should_fix
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 QSFP_RESETL_: 无上拉/下拉电阻
- **recommended_action**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **decision_impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **evidence_id**: EVID-237-rule_engine_v3-SI.reset_bias

## 238. 未找到可检查的设计约束，约束冲突检查已跳过。提供 requirements.yaml 或 pipeline_result.design_constraints 后会启用。
- **action_id**: ACT-238
- **priority**: P2
- **action_type**: manual_review
- **source**: constraint_checker
- **rule_id**: CONSTRAINT-NO-INPUT
- **category**: CONSTRAINT
- **location**: /home/ubuntu/hardware-projects/prj/DF108/revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-20260507-judgment-v2/runtime_repo/data/DF108
- **title**: 未找到可检查的设计约束，约束冲突检查已跳过。提供 requirements.yaml 或 pipeline_result.design_constraints 后会启用。
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: CONSTRAINT 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-238-constraint_checker-CONSTRAINT-NO-INPUT

## 239. 未找到 requirements.yaml，跳过 EMC 预评估
- **action_id**: ACT-239
- **priority**: P2
- **action_type**: manual_review
- **source**: emc_checker
- **rule_id**: EMC-NO-REQ
- **category**: EMC
- **location**: 
- **title**: 未找到 requirements.yaml，跳过 EMC 预评估
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: EMC 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-239-emc_checker-EMC-NO-REQ

## 240. R176: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-240
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R176: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-240-rule_engine_v3-COMP.abnormal_values

## 241. R310: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-241
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R310: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-241-rule_engine_v3-COMP.abnormal_values

## 242. R222: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-242
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R222: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-242-rule_engine_v3-COMP.abnormal_values

## 243. R236: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-243
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R236: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-243-rule_engine_v3-COMP.abnormal_values

## 244. R234: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-244
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R234: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-244-rule_engine_v3-COMP.abnormal_values

## 245. R229: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-245
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R229: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-245-rule_engine_v3-COMP.abnormal_values

## 246. R248: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-246
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R248: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-246-rule_engine_v3-COMP.abnormal_values

## 247. R240: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-247
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R240: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-247-rule_engine_v3-COMP.abnormal_values

## 248. R200: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-248
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R200: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-248-rule_engine_v3-COMP.abnormal_values

## 249. R209: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-249
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R209: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-249-rule_engine_v3-COMP.abnormal_values

## 250. R221: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-250
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R221: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-250-rule_engine_v3-COMP.abnormal_values

## 251. R213: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-251
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R213: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-251-rule_engine_v3-COMP.abnormal_values

## 252. R48: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-252
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R48: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-252-rule_engine_v3-COMP.abnormal_values

## 253. R46: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-253
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R46: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-253-rule_engine_v3-COMP.abnormal_values

## 254. R47: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-254
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R47: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-254-rule_engine_v3-COMP.abnormal_values

## 255. R178: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-255
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R178: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-255-rule_engine_v3-COMP.abnormal_values

## 256. R183: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-256
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R183: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-256-rule_engine_v3-COMP.abnormal_values

## 257. R56: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-257
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R56: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-257-rule_engine_v3-COMP.abnormal_values

## 258. R55: 0R 电阻在电源路径上（确认是否为设计意图）
- **action_id**: ACT-258
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.abnormal_values
- **category**: COMP
- **location**: 
- **title**: R55: 0R 电阻在电源路径上（确认是否为设计意图）
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-258-rule_engine_v3-COMP.abnormal_values

## 259. BOM 与网表 Refdes 完全一致
- **action_id**: ACT-259
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.bom_netlist_coverage
- **category**: COMP
- **location**: 
- **title**: BOM 与网表 Refdes 完全一致
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-259-rule_engine_v3-COMP.bom_netlist_coverage

## 260. BOM Value/Description 一致性良好
- **action_id**: ACT-260
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.bom_value_consistency
- **category**: COMP
- **location**: 
- **title**: BOM Value/Description 一致性良好
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-260-rule_engine_v3-COMP.bom_value_consistency

## 261. 物料封装一致，无需整合
- **action_id**: ACT-261
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.consolidation
- **category**: COMP
- **location**: 
- **title**: 物料封装一致，无需整合
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-261-rule_engine_v3-COMP.consolidation

## 262. 封装一致性良好
- **action_id**: ACT-262
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: COMP.package_consistency
- **category**: COMP
- **location**: 
- **title**: 封装一致性良好
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-262-rule_engine_v3-COMP.package_consistency

## 263. 无悬空网络
- **action_id**: ACT-263
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: CONN.dangling_nets
- **category**: CONN
- **location**: 
- **title**: 无悬空网络
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: CONN 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-263-rule_engine_v3-CONN.dangling_nets

## 264. 无单引脚网络
- **action_id**: ACT-264
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: CONN.single_pin_nets
- **category**: CONN
- **location**: 
- **title**: 无单引脚网络
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: CONN 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-264-rule_engine_v3-CONN.single_pin_nets

## 265. 电容降额检查通过
- **action_id**: ACT-265
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: CONST.cap_derating
- **category**: CONST
- **location**: 
- **title**: 电容降额检查通过
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: CONST 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-265-rule_engine_v3-CONST.cap_derating

## 266. 协议合规检查通过
- **action_id**: ACT-266
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: CONST.protocol_compliance
- **category**: CONST
- **location**: 
- **title**: 协议合规检查通过
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: CONST 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-266-rule_engine_v3-CONST.protocol_compliance

## 267. VIN 绝对最大值检查通过
- **action_id**: ACT-267
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: CONST.voltage_abs_max
- **category**: CONST
- **location**: 
- **title**: VIN 绝对最大值检查通过
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: CONST 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-267-rule_engine_v3-CONST.voltage_abs_max

## 268. 未找到 VCC/VCCIO 电源网络
- **action_id**: ACT-268
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: CONST.voltage_ripple
- **category**: CONST
- **location**: 
- **title**: 未找到 VCC/VCCIO 电源网络
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: CONST 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-268-rule_engine_v3-CONST.voltage_ripple

## 269. 未找到 DRC 文件，跳过交叉引用检查
- **action_id**: ACT-269
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: DRC.drc_cross_reference
- **category**: DRC
- **location**: 
- **title**: 未找到 DRC 文件，跳过交叉引用检查
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: DRC 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-269-rule_engine_v3-DRC.drc_cross_reference

## 270. 未找到 DRC 文件，跳过 DRC 检查
- **action_id**: ACT-270
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: DRC.drc_summary
- **category**: DRC
- **location**: 
- **title**: 未找到 DRC 文件，跳过 DRC 检查
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: DRC 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-270-rule_engine_v3-DRC.drc_summary

## 271. 未发现 FPGA 器件
- **action_id**: ACT-271
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.bank_voltage
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-271-rule_engine_v3-FPGA.bank_voltage

## 272. 未发现 FPGA 器件
- **action_id**: ACT-272
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.cfgbvs
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-272-rule_engine_v3-FPGA.cfgbvs

## 273. 未发现 FPGA 器件
- **action_id**: ACT-273
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.config_design_guide
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-273-rule_engine_v3-FPGA.config_design_guide

## 274. 未发现 FPGA 器件
- **action_id**: ACT-274
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.design_guide_clocking
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-274-rule_engine_v3-FPGA.design_guide_clocking

## 275. 未发现 FPGA 器件
- **action_id**: ACT-275
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.design_guide_io_signaling
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-275-rule_engine_v3-FPGA.design_guide_io_signaling

## 276. 未发现 FPGA 器件
- **action_id**: ACT-276
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.design_guide_power_integrity
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-276-rule_engine_v3-FPGA.design_guide_power_integrity

## 277. 未发现 FPGA 器件
- **action_id**: ACT-277
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.done_pullup
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-277-rule_engine_v3-FPGA.done_pullup

## 278. 未发现 FPGA 器件
- **action_id**: ACT-278
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.mode_strap
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-278-rule_engine_v3-FPGA.mode_strap

## 279. 未发现 FPGA 器件
- **action_id**: ACT-279
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.pudc_static
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-279-rule_engine_v3-FPGA.pudc_static

## 280. 未发现 FPGA 器件
- **action_id**: ACT-280
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.reconfig_n_bias
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-280-rule_engine_v3-FPGA.reconfig_n_bias

## 281. 未发现 FPGA 器件
- **action_id**: ACT-281
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.serdes_ac_coupling
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-281-rule_engine_v3-FPGA.serdes_ac_coupling

## 282. 未发现 FPGA 器件
- **action_id**: ACT-282
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: FPGA.sspi_pin_swap
- **category**: FPGA
- **location**: 
- **title**: 未发现 FPGA 器件
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-282-rule_engine_v3-FPGA.sspi_pin_swap

## 283. 电容耐压降额检查通过
- **action_id**: ACT-283
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.cap_voltage_derating
- **category**: PI
- **location**: 
- **title**: 电容耐压降额检查通过
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-283-rule_engine_v3-PI.cap_voltage_derating

## 284. 未发现 SerDes/MIPI 电源网络
- **action_id**: ACT-284
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.ferrite_isolation
- **category**: PI
- **location**: 
- **title**: 未发现 SerDes/MIPI 电源网络
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-284-rule_engine_v3-PI.ferrite_isolation

## 285. R176: 0R 电阻在电源路径上 (M1V8 ↔ VCCAUX)
- **action_id**: ACT-285
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R176: 0R 电阻在电源路径上 (M1V8 ↔ VCCAUX)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-285-rule_engine_v3-PI.zero_ohm_on_power

## 286. R310: 0R 电阻在电源路径上 (M1V8 ↔ VCCAUX)
- **action_id**: ACT-286
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R310: 0R 电阻在电源路径上 (M1V8 ↔ VCCAUX)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-286-rule_engine_v3-PI.zero_ohm_on_power

## 287. R222: 0R 电阻在电源路径上 (5V ↔ M5V)
- **action_id**: ACT-287
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R222: 0R 电阻在电源路径上 (5V ↔ M5V)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-287-rule_engine_v3-PI.zero_ohm_on_power

## 288. R236: 0R 电阻在电源路径上 (5V ↔ M5V)
- **action_id**: ACT-288
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R236: 0R 电阻在电源路径上 (5V ↔ M5V)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-288-rule_engine_v3-PI.zero_ohm_on_power

## 289. R234: 0R 电阻在电源路径上 (5V ↔ M5V)
- **action_id**: ACT-289
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R234: 0R 电阻在电源路径上 (5V ↔ M5V)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-289-rule_engine_v3-PI.zero_ohm_on_power

## 290. R229: 0R 电阻在电源路径上 (5V ↔ M5V)
- **action_id**: ACT-290
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R229: 0R 电阻在电源路径上 (5V ↔ M5V)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-290-rule_engine_v3-PI.zero_ohm_on_power

## 291. R248: 0R 电阻在电源路径上 (DDR4_VDD ↔ M1V2)
- **action_id**: ACT-291
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R248: 0R 电阻在电源路径上 (DDR4_VDD ↔ M1V2)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-291-rule_engine_v3-PI.zero_ohm_on_power

## 292. R240: 0R 电阻在电源路径上 (DDR4_VDD ↔ M1V2)
- **action_id**: ACT-292
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R240: 0R 电阻在电源路径上 (DDR4_VDD ↔ M1V2)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-292-rule_engine_v3-PI.zero_ohm_on_power

## 293. R200: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **action_id**: ACT-293
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R200: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-293-rule_engine_v3-PI.zero_ohm_on_power

## 294. R209: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **action_id**: ACT-294
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R209: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-294-rule_engine_v3-PI.zero_ohm_on_power

## 295. R221: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **action_id**: ACT-295
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R221: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-295-rule_engine_v3-PI.zero_ohm_on_power

## 296. R213: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **action_id**: ACT-296
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R213: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-296-rule_engine_v3-PI.zero_ohm_on_power

## 297. R48: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **action_id**: ACT-297
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R48: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-297-rule_engine_v3-PI.zero_ohm_on_power

## 298. R46: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **action_id**: ACT-298
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R46: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-298-rule_engine_v3-PI.zero_ohm_on_power

## 299. R47: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **action_id**: ACT-299
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R47: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-299-rule_engine_v3-PI.zero_ohm_on_power

## 300. R178: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **action_id**: ACT-300
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R178: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-300-rule_engine_v3-PI.zero_ohm_on_power

## 301. R183: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **action_id**: ACT-301
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R183: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-301-rule_engine_v3-PI.zero_ohm_on_power

## 302. R56: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_L)
- **action_id**: ACT-302
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R56: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_L)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-302-rule_engine_v3-PI.zero_ohm_on_power

## 303. R55: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_L)
- **action_id**: ACT-303
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: PI.zero_ohm_on_power
- **category**: PI
- **location**: 
- **title**: R55: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_L)
- **recommended_action**: 确认是否为设计意图，大电流场景需评估压降
- **decision_impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-303-rule_engine_v3-PI.zero_ohm_on_power

## 304. 发现 112 对确认差分对, 72 对疑似
- **action_id**: ACT-304
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 发现 112 对确认差分对, 72 对疑似
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-304-rule_engine_v3-SI.diff_pair_symmetry

## 305. 差分对 DDR4_CLK_P/DDR4_CLK_N (置信度100%): 对称 ✓
- **action_id**: ACT-305
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 DDR4_CLK_P/DDR4_CLK_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-305-rule_engine_v3-SI.diff_pair_symmetry

## 306. 疑似差分对 DDR4_DQS_P0/DDR4_DQS_N0 (置信度50%): 请人工确认
- **action_id**: ACT-306
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 DDR4_DQS_P0/DDR4_DQS_N0 (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-306-rule_engine_v3-SI.diff_pair_symmetry

## 307. 疑似差分对 DDR4_DQS_P1/DDR4_DQS_N1 (置信度50%): 请人工确认
- **action_id**: ACT-307
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 DDR4_DQS_P1/DDR4_DQS_N1 (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-307-rule_engine_v3-SI.diff_pair_symmetry

## 308. 疑似差分对 DDR4_DQS_P2/DDR4_DQS_N2 (置信度50%): 请人工确认
- **action_id**: ACT-308
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 DDR4_DQS_P2/DDR4_DQS_N2 (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-308-rule_engine_v3-SI.diff_pair_symmetry

## 309. 疑似差分对 DDR4_DQS_P3/DDR4_DQS_N3 (置信度50%): 请人工确认
- **action_id**: ACT-309
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 DDR4_DQS_P3/DDR4_DQS_N3 (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-309-rule_engine_v3-SI.diff_pair_symmetry

## 310. 疑似差分对 DDR4_DQS_P4/DDR4_DQS_N4 (置信度50%): 请人工确认
- **action_id**: ACT-310
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 DDR4_DQS_P4/DDR4_DQS_N4 (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-310-rule_engine_v3-SI.diff_pair_symmetry

## 311. 疑似差分对 DDR4_DQS_P5/DDR4_DQS_N5 (置信度50%): 请人工确认
- **action_id**: ACT-311
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 DDR4_DQS_P5/DDR4_DQS_N5 (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-311-rule_engine_v3-SI.diff_pair_symmetry

## 312. 疑似差分对 DDR4_DQS_P6/DDR4_DQS_N6 (置信度50%): 请人工确认
- **action_id**: ACT-312
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 DDR4_DQS_P6/DDR4_DQS_N6 (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-312-rule_engine_v3-SI.diff_pair_symmetry

## 313. 疑似差分对 DDR4_DQS_P7/DDR4_DQS_N7 (置信度50%): 请人工确认
- **action_id**: ACT-313
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 DDR4_DQS_P7/DDR4_DQS_N7 (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-313-rule_engine_v3-SI.diff_pair_symmetry

## 314. 差分对 DDR4_VREF_CLK_P/DDR4_VREF_CLK_N (置信度100%): 对称 ✓
- **action_id**: ACT-314
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 DDR4_VREF_CLK_P/DDR4_VREF_CLK_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-314-rule_engine_v3-SI.diff_pair_symmetry

## 315. 差分对 MA_BF_D_CLK_HS_P/MA_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-315
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MA_BF_D_CLK_HS_P/MA_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-315-rule_engine_v3-SI.diff_pair_symmetry

## 316. 差分对 MA_BF_D_D0_HS_P/MA_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-316
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MA_BF_D_D0_HS_P/MA_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-316-rule_engine_v3-SI.diff_pair_symmetry

## 317. 差分对 MA_BF_D_D1_HS_P/MA_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-317
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MA_BF_D_D1_HS_P/MA_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-317-rule_engine_v3-SI.diff_pair_symmetry

## 318. 差分对 MA_BF_D_D2_HS_P/MA_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-318
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MA_BF_D_D2_HS_P/MA_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-318-rule_engine_v3-SI.diff_pair_symmetry

## 319. 差分对 MA_BF_D_D3_HS_P/MA_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-319
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MA_BF_D_D3_HS_P/MA_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-319-rule_engine_v3-SI.diff_pair_symmetry

## 320. 差分对 MB_BF_D_CLK_HS_P/MB_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-320
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MB_BF_D_CLK_HS_P/MB_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-320-rule_engine_v3-SI.diff_pair_symmetry

## 321. 差分对 MB_BF_D_D0_HS_P/MB_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-321
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MB_BF_D_D0_HS_P/MB_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-321-rule_engine_v3-SI.diff_pair_symmetry

## 322. 差分对 MB_BF_D_D1_HS_P/MB_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-322
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MB_BF_D_D1_HS_P/MB_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-322-rule_engine_v3-SI.diff_pair_symmetry

## 323. 差分对 MB_BF_D_D2_HS_P/MB_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-323
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MB_BF_D_D2_HS_P/MB_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-323-rule_engine_v3-SI.diff_pair_symmetry

## 324. 差分对 MB_BF_D_D3_HS_P/MB_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-324
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MB_BF_D_D3_HS_P/MB_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-324-rule_engine_v3-SI.diff_pair_symmetry

## 325. 疑似差分对 MC_BF_D_CLK_HS_P/MC_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-325
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MC_BF_D_CLK_HS_P/MC_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-325-rule_engine_v3-SI.diff_pair_symmetry

## 326. 疑似差分对 MC_BF_D_D0_HS_P/MC_BF_D_D0_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-326
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MC_BF_D_D0_HS_P/MC_BF_D_D0_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-326-rule_engine_v3-SI.diff_pair_symmetry

## 327. 疑似差分对 MC_BF_D_D1_HS_P/MC_BF_D_D1_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-327
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MC_BF_D_D1_HS_P/MC_BF_D_D1_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-327-rule_engine_v3-SI.diff_pair_symmetry

## 328. 疑似差分对 MC_BF_D_D2_HS_P/MC_BF_D_D2_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-328
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MC_BF_D_D2_HS_P/MC_BF_D_D2_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-328-rule_engine_v3-SI.diff_pair_symmetry

## 329. 疑似差分对 MC_BF_D_D3_HS_P/MC_BF_D_D3_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-329
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MC_BF_D_D3_HS_P/MC_BF_D_D3_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-329-rule_engine_v3-SI.diff_pair_symmetry

## 330. 疑似差分对 MD_BF_D_CLK_HS_P/MD_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-330
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MD_BF_D_CLK_HS_P/MD_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-330-rule_engine_v3-SI.diff_pair_symmetry

## 331. 疑似差分对 MD_BF_D_D0_HS_P/MD_BF_D_D0_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-331
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MD_BF_D_D0_HS_P/MD_BF_D_D0_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-331-rule_engine_v3-SI.diff_pair_symmetry

## 332. 疑似差分对 MD_BF_D_D1_HS_P/MD_BF_D_D1_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-332
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MD_BF_D_D1_HS_P/MD_BF_D_D1_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-332-rule_engine_v3-SI.diff_pair_symmetry

## 333. 疑似差分对 MD_BF_D_D2_HS_P/MD_BF_D_D2_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-333
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MD_BF_D_D2_HS_P/MD_BF_D_D2_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-333-rule_engine_v3-SI.diff_pair_symmetry

## 334. 疑似差分对 MD_BF_D_D3_HS_P/MD_BF_D_D3_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-334
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MD_BF_D_D3_HS_P/MD_BF_D_D3_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-334-rule_engine_v3-SI.diff_pair_symmetry

## 335. 差分对 ME_BF_D_CLK_HS_P/ME_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-335
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_BF_D_CLK_HS_P/ME_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-335-rule_engine_v3-SI.diff_pair_symmetry

## 336. 差分对 ME_BF_D_D0_HS_P/ME_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-336
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_BF_D_D0_HS_P/ME_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-336-rule_engine_v3-SI.diff_pair_symmetry

## 337. 差分对 ME_BF_D_D1_HS_P/ME_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-337
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_BF_D_D1_HS_P/ME_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-337-rule_engine_v3-SI.diff_pair_symmetry

## 338. 差分对 ME_BF_D_D2_HS_P/ME_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-338
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_BF_D_D2_HS_P/ME_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-338-rule_engine_v3-SI.diff_pair_symmetry

## 339. 差分对 ME_BF_D_D3_HS_P/ME_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-339
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_BF_D_D3_HS_P/ME_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-339-rule_engine_v3-SI.diff_pair_symmetry

## 340. 差分对 ME_DIVIDE_CLK_HS_P/ME_DIVIDE_CLK_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-340
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_DIVIDE_CLK_HS_P/ME_DIVIDE_CLK_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-340-rule_engine_v3-SI.diff_pair_symmetry

## 341. 差分对 ME_D_CLK_HS_P/ME_D_CLK_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-341
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_D_CLK_HS_P/ME_D_CLK_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-341-rule_engine_v3-SI.diff_pair_symmetry

## 342. 差分对 ME_D_D0_HS_P/ME_D_D0_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-342
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_D_D0_HS_P/ME_D_D0_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-342-rule_engine_v3-SI.diff_pair_symmetry

## 343. 差分对 ME_D_D1_HS_P/ME_D_D1_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-343
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_D_D1_HS_P/ME_D_D1_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-343-rule_engine_v3-SI.diff_pair_symmetry

## 344. 差分对 ME_D_D2_HS_P/ME_D_D2_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-344
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_D_D2_HS_P/ME_D_D2_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-344-rule_engine_v3-SI.diff_pair_symmetry

## 345. 差分对 ME_D_D3_HS_P/ME_D_D3_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-345
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_D_D3_HS_P/ME_D_D3_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-345-rule_engine_v3-SI.diff_pair_symmetry

## 346. 差分对 ME_SERDES_CLK_HS_P/ME_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **action_id**: ACT-346
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_SERDES_CLK_HS_P/ME_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-346-rule_engine_v3-SI.diff_pair_symmetry

## 347. 差分对 ME_SERDES_D0_HS_P/ME_SERDES_D0_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-347
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_SERDES_D0_HS_P/ME_SERDES_D0_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-347-rule_engine_v3-SI.diff_pair_symmetry

## 348. 差分对 ME_SERDES_D1_HS_P/ME_SERDES_D1_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-348
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_SERDES_D1_HS_P/ME_SERDES_D1_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-348-rule_engine_v3-SI.diff_pair_symmetry

## 349. 差分对 ME_SERDES_D2_HS_P/ME_SERDES_D2_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-349
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_SERDES_D2_HS_P/ME_SERDES_D2_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-349-rule_engine_v3-SI.diff_pair_symmetry

## 350. 差分对 ME_SERDES_D3_HS_P/ME_SERDES_D3_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-350
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 ME_SERDES_D3_HS_P/ME_SERDES_D3_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-350-rule_engine_v3-SI.diff_pair_symmetry

## 351. 差分对 MF_BF_D_CLK_HS_P/MF_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-351
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_BF_D_CLK_HS_P/MF_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-351-rule_engine_v3-SI.diff_pair_symmetry

## 352. 差分对 MF_BF_D_D0_HS_P/MF_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-352
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_BF_D_D0_HS_P/MF_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-352-rule_engine_v3-SI.diff_pair_symmetry

## 353. 差分对 MF_BF_D_D1_HS_P/MF_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-353
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_BF_D_D1_HS_P/MF_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-353-rule_engine_v3-SI.diff_pair_symmetry

## 354. 差分对 MF_BF_D_D2_HS_P/MF_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-354
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_BF_D_D2_HS_P/MF_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-354-rule_engine_v3-SI.diff_pair_symmetry

## 355. 差分对 MF_BF_D_D3_HS_P/MF_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-355
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_BF_D_D3_HS_P/MF_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-355-rule_engine_v3-SI.diff_pair_symmetry

## 356. 差分对 MF_DIVIDE_CLK_HS_P/MF_DIVIDE_CLK_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-356
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_DIVIDE_CLK_HS_P/MF_DIVIDE_CLK_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-356-rule_engine_v3-SI.diff_pair_symmetry

## 357. 差分对 MF_D_CLK_HS_P/MF_D_CLK_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-357
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_D_CLK_HS_P/MF_D_CLK_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-357-rule_engine_v3-SI.diff_pair_symmetry

## 358. 差分对 MF_D_D0_HS_P/MF_D_D0_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-358
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_D_D0_HS_P/MF_D_D0_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-358-rule_engine_v3-SI.diff_pair_symmetry

## 359. 差分对 MF_D_D1_HS_P/MF_D_D1_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-359
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_D_D1_HS_P/MF_D_D1_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-359-rule_engine_v3-SI.diff_pair_symmetry

## 360. 差分对 MF_D_D2_HS_P/MF_D_D2_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-360
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_D_D2_HS_P/MF_D_D2_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-360-rule_engine_v3-SI.diff_pair_symmetry

## 361. 差分对 MF_D_D3_HS_P/MF_D_D3_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-361
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_D_D3_HS_P/MF_D_D3_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-361-rule_engine_v3-SI.diff_pair_symmetry

## 362. 差分对 MF_SERDES_CLK_HS_P/MF_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **action_id**: ACT-362
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_SERDES_CLK_HS_P/MF_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-362-rule_engine_v3-SI.diff_pair_symmetry

## 363. 差分对 MF_SERDES_D0_HS_P/MF_SERDES_D0_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-363
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_SERDES_D0_HS_P/MF_SERDES_D0_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-363-rule_engine_v3-SI.diff_pair_symmetry

## 364. 差分对 MF_SERDES_D1_HS_P/MF_SERDES_D1_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-364
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_SERDES_D1_HS_P/MF_SERDES_D1_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-364-rule_engine_v3-SI.diff_pair_symmetry

## 365. 差分对 MF_SERDES_D2_HS_P/MF_SERDES_D2_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-365
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_SERDES_D2_HS_P/MF_SERDES_D2_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-365-rule_engine_v3-SI.diff_pair_symmetry

## 366. 差分对 MF_SERDES_D3_HS_P/MF_SERDES_D3_HS_N (置信度90%): 对称 ✓
- **action_id**: ACT-366
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MF_SERDES_D3_HS_P/MF_SERDES_D3_HS_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-366-rule_engine_v3-SI.diff_pair_symmetry

## 367. 疑似差分对 MG_BF_D_CLK_HS_P/MG_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-367
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_BF_D_CLK_HS_P/MG_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-367-rule_engine_v3-SI.diff_pair_symmetry

## 368. 疑似差分对 MG_BF_D_D0_HS_P/MG_BF_D_D0_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-368
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_BF_D_D0_HS_P/MG_BF_D_D0_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-368-rule_engine_v3-SI.diff_pair_symmetry

## 369. 疑似差分对 MG_BF_D_D1_HS_P/MG_BF_D_D1_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-369
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_BF_D_D1_HS_P/MG_BF_D_D1_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-369-rule_engine_v3-SI.diff_pair_symmetry

## 370. 疑似差分对 MG_BF_D_D2_HS_P/MG_BF_D_D2_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-370
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_BF_D_D2_HS_P/MG_BF_D_D2_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-370-rule_engine_v3-SI.diff_pair_symmetry

## 371. 疑似差分对 MG_BF_D_D3_HS_P/MG_BF_D_D3_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-371
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_BF_D_D3_HS_P/MG_BF_D_D3_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-371-rule_engine_v3-SI.diff_pair_symmetry

## 372. 疑似差分对 MG_DIVIDE_CLK_HS_P/MG_DIVIDE_CLK_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-372
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_DIVIDE_CLK_HS_P/MG_DIVIDE_CLK_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-372-rule_engine_v3-SI.diff_pair_symmetry

## 373. 疑似差分对 MG_D_CLK_HS_P/MG_D_CLK_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-373
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_D_CLK_HS_P/MG_D_CLK_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-373-rule_engine_v3-SI.diff_pair_symmetry

## 374. 疑似差分对 MG_D_D0_HS_P/MG_D_D0_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-374
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_D_D0_HS_P/MG_D_D0_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-374-rule_engine_v3-SI.diff_pair_symmetry

## 375. 疑似差分对 MG_D_D1_HS_P/MG_D_D1_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-375
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_D_D1_HS_P/MG_D_D1_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-375-rule_engine_v3-SI.diff_pair_symmetry

## 376. 疑似差分对 MG_D_D2_HS_P/MG_D_D2_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-376
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_D_D2_HS_P/MG_D_D2_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-376-rule_engine_v3-SI.diff_pair_symmetry

## 377. 疑似差分对 MG_D_D3_HS_P/MG_D_D3_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-377
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_D_D3_HS_P/MG_D_D3_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-377-rule_engine_v3-SI.diff_pair_symmetry

## 378. 差分对 MG_SERDES_CLK_HS_P/MG_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **action_id**: ACT-378
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MG_SERDES_CLK_HS_P/MG_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-378-rule_engine_v3-SI.diff_pair_symmetry

## 379. 疑似差分对 MG_SERDES_D0_HS_P/MG_SERDES_D0_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-379
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_SERDES_D0_HS_P/MG_SERDES_D0_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-379-rule_engine_v3-SI.diff_pair_symmetry

## 380. 疑似差分对 MG_SERDES_D1_HS_P/MG_SERDES_D1_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-380
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_SERDES_D1_HS_P/MG_SERDES_D1_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-380-rule_engine_v3-SI.diff_pair_symmetry

## 381. 疑似差分对 MG_SERDES_D2_HS_P/MG_SERDES_D2_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-381
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_SERDES_D2_HS_P/MG_SERDES_D2_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-381-rule_engine_v3-SI.diff_pair_symmetry

## 382. 疑似差分对 MG_SERDES_D3_HS_P/MG_SERDES_D3_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-382
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MG_SERDES_D3_HS_P/MG_SERDES_D3_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-382-rule_engine_v3-SI.diff_pair_symmetry

## 383. 疑似差分对 MH_BF_D_CLK_HS_P/MH_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-383
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_BF_D_CLK_HS_P/MH_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-383-rule_engine_v3-SI.diff_pair_symmetry

## 384. 疑似差分对 MH_BF_D_D0_HS_P/MH_BF_D_D0_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-384
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_BF_D_D0_HS_P/MH_BF_D_D0_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-384-rule_engine_v3-SI.diff_pair_symmetry

## 385. 疑似差分对 MH_BF_D_D1_HS_P/MH_BF_D_D1_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-385
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_BF_D_D1_HS_P/MH_BF_D_D1_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-385-rule_engine_v3-SI.diff_pair_symmetry

## 386. 疑似差分对 MH_BF_D_D2_HS_P/MH_BF_D_D2_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-386
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_BF_D_D2_HS_P/MH_BF_D_D2_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-386-rule_engine_v3-SI.diff_pair_symmetry

## 387. 疑似差分对 MH_BF_D_D3_HS_P/MH_BF_D_D3_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-387
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_BF_D_D3_HS_P/MH_BF_D_D3_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-387-rule_engine_v3-SI.diff_pair_symmetry

## 388. 疑似差分对 MH_DIVIDE_CLK_HS_P/MH_DIVIDE_CLK_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-388
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_DIVIDE_CLK_HS_P/MH_DIVIDE_CLK_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-388-rule_engine_v3-SI.diff_pair_symmetry

## 389. 疑似差分对 MH_D_CLK_HS_P/MH_D_CLK_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-389
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_D_CLK_HS_P/MH_D_CLK_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-389-rule_engine_v3-SI.diff_pair_symmetry

## 390. 疑似差分对 MH_D_D0_HS_P/MH_D_D0_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-390
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_D_D0_HS_P/MH_D_D0_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-390-rule_engine_v3-SI.diff_pair_symmetry

## 391. 疑似差分对 MH_D_D1_HS_P/MH_D_D1_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-391
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_D_D1_HS_P/MH_D_D1_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-391-rule_engine_v3-SI.diff_pair_symmetry

## 392. 疑似差分对 MH_D_D2_HS_P/MH_D_D2_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-392
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_D_D2_HS_P/MH_D_D2_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-392-rule_engine_v3-SI.diff_pair_symmetry

## 393. 疑似差分对 MH_D_D3_HS_P/MH_D_D3_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-393
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_D_D3_HS_P/MH_D_D3_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-393-rule_engine_v3-SI.diff_pair_symmetry

## 394. 差分对 MH_SERDES_CLK_HS_P/MH_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **action_id**: ACT-394
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MH_SERDES_CLK_HS_P/MH_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-394-rule_engine_v3-SI.diff_pair_symmetry

## 395. 疑似差分对 MH_SERDES_D0_HS_P/MH_SERDES_D0_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-395
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_SERDES_D0_HS_P/MH_SERDES_D0_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-395-rule_engine_v3-SI.diff_pair_symmetry

## 396. 疑似差分对 MH_SERDES_D1_HS_P/MH_SERDES_D1_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-396
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_SERDES_D1_HS_P/MH_SERDES_D1_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-396-rule_engine_v3-SI.diff_pair_symmetry

## 397. 疑似差分对 MH_SERDES_D2_HS_P/MH_SERDES_D2_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-397
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_SERDES_D2_HS_P/MH_SERDES_D2_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-397-rule_engine_v3-SI.diff_pair_symmetry

## 398. 疑似差分对 MH_SERDES_D3_HS_P/MH_SERDES_D3_HS_N (置信度50%): 请人工确认
- **action_id**: ACT-398
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MH_SERDES_D3_HS_P/MH_SERDES_D3_HS_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-398-rule_engine_v3-SI.diff_pair_symmetry

## 399. 差分对 MIPIA_CLK_P/MIPIA_CLK_N (置信度90%): 对称 ✓
- **action_id**: ACT-399
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_CLK_P/MIPIA_CLK_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-399-rule_engine_v3-SI.diff_pair_symmetry

## 400. 差分对 MIPIA_D0_P/MIPIA_D0_N (置信度90%): 对称 ✓
- **action_id**: ACT-400
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_D0_P/MIPIA_D0_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-400-rule_engine_v3-SI.diff_pair_symmetry

## 401. 差分对 MIPIA_D1_P/MIPIA_D1_N (置信度90%): 对称 ✓
- **action_id**: ACT-401
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_D1_P/MIPIA_D1_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-401-rule_engine_v3-SI.diff_pair_symmetry

## 402. 差分对 MIPIA_D2_P/MIPIA_D2_N (置信度90%): 对称 ✓
- **action_id**: ACT-402
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_D2_P/MIPIA_D2_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-402-rule_engine_v3-SI.diff_pair_symmetry

## 403. 差分对 MIPIA_D3_P/MIPIA_D3_N (置信度90%): 对称 ✓
- **action_id**: ACT-403
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_D3_P/MIPIA_D3_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-403-rule_engine_v3-SI.diff_pair_symmetry

## 404. 差分对 MIPIA_D_D0P_HS/MIPIA_D_D0N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-404
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_D_D0P_HS/MIPIA_D_D0N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-404-rule_engine_v3-SI.diff_pair_symmetry

## 405. 差分对 MIPIA_D_D0P_LP/MIPIA_D_D0N_LP (置信度90%): 对称 ✓
- **action_id**: ACT-405
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_D_D0P_LP/MIPIA_D_D0N_LP (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-405-rule_engine_v3-SI.diff_pair_symmetry

## 406. 差分对 MIPIA_D_D1P_HS/MIPIA_D_D1N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-406
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_D_D1P_HS/MIPIA_D_D1N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-406-rule_engine_v3-SI.diff_pair_symmetry

## 407. 差分对 MIPIA_D_D2P_HS/MIPIA_D_D2N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-407
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_D_D2P_HS/MIPIA_D_D2N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-407-rule_engine_v3-SI.diff_pair_symmetry

## 408. 差分对 MIPIA_D_D3P_HS/MIPIA_D_D3N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-408
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIA_D_D3P_HS/MIPIA_D_D3N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-408-rule_engine_v3-SI.diff_pair_symmetry

## 409. 差分对 MIPIB_CLK_P/MIPIB_CLK_N (置信度90%): 对称 ✓
- **action_id**: ACT-409
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_CLK_P/MIPIB_CLK_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-409-rule_engine_v3-SI.diff_pair_symmetry

## 410. 差分对 MIPIB_D0_P/MIPIB_D0_N (置信度90%): 对称 ✓
- **action_id**: ACT-410
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_D0_P/MIPIB_D0_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-410-rule_engine_v3-SI.diff_pair_symmetry

## 411. 差分对 MIPIB_D1_P/MIPIB_D1_N (置信度90%): 对称 ✓
- **action_id**: ACT-411
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_D1_P/MIPIB_D1_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-411-rule_engine_v3-SI.diff_pair_symmetry

## 412. 差分对 MIPIB_D2_P/MIPIB_D2_N (置信度90%): 对称 ✓
- **action_id**: ACT-412
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_D2_P/MIPIB_D2_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-412-rule_engine_v3-SI.diff_pair_symmetry

## 413. 差分对 MIPIB_D3_P/MIPIB_D3_N (置信度90%): 对称 ✓
- **action_id**: ACT-413
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_D3_P/MIPIB_D3_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-413-rule_engine_v3-SI.diff_pair_symmetry

## 414. 差分对 MIPIB_D_D0P_HS/MIPIB_D_D0N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-414
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_D_D0P_HS/MIPIB_D_D0N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-414-rule_engine_v3-SI.diff_pair_symmetry

## 415. 差分对 MIPIB_D_D0P_LP/MIPIB_D_D0N_LP (置信度90%): 对称 ✓
- **action_id**: ACT-415
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_D_D0P_LP/MIPIB_D_D0N_LP (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-415-rule_engine_v3-SI.diff_pair_symmetry

## 416. 差分对 MIPIB_D_D1P_HS/MIPIB_D_D1N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-416
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_D_D1P_HS/MIPIB_D_D1N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-416-rule_engine_v3-SI.diff_pair_symmetry

## 417. 差分对 MIPIB_D_D2P_HS/MIPIB_D_D2N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-417
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_D_D2P_HS/MIPIB_D_D2N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-417-rule_engine_v3-SI.diff_pair_symmetry

## 418. 差分对 MIPIB_D_D3P_HS/MIPIB_D_D3N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-418
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIB_D_D3P_HS/MIPIB_D_D3N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-418-rule_engine_v3-SI.diff_pair_symmetry

## 419. 疑似差分对 MIPIC_CLK_P/MIPIC_CLK_N (置信度50%): 请人工确认
- **action_id**: ACT-419
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIC_CLK_P/MIPIC_CLK_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-419-rule_engine_v3-SI.diff_pair_symmetry

## 420. 疑似差分对 MIPIC_D0_P/MIPIC_D0_N (置信度50%): 请人工确认
- **action_id**: ACT-420
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIC_D0_P/MIPIC_D0_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-420-rule_engine_v3-SI.diff_pair_symmetry

## 421. 疑似差分对 MIPIC_D1_P/MIPIC_D1_N (置信度50%): 请人工确认
- **action_id**: ACT-421
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIC_D1_P/MIPIC_D1_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-421-rule_engine_v3-SI.diff_pair_symmetry

## 422. 疑似差分对 MIPIC_D2_P/MIPIC_D2_N (置信度50%): 请人工确认
- **action_id**: ACT-422
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIC_D2_P/MIPIC_D2_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-422-rule_engine_v3-SI.diff_pair_symmetry

## 423. 疑似差分对 MIPIC_D3_P/MIPIC_D3_N (置信度50%): 请人工确认
- **action_id**: ACT-423
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIC_D3_P/MIPIC_D3_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-423-rule_engine_v3-SI.diff_pair_symmetry

## 424. 差分对 MIPIC_D_D0P_HS/MIPIC_D_D0N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-424
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIC_D_D0P_HS/MIPIC_D_D0N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-424-rule_engine_v3-SI.diff_pair_symmetry

## 425. 疑似差分对 MIPIC_D_D0P_LP/MIPIC_D_D0N_LP (置信度50%): 请人工确认
- **action_id**: ACT-425
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIC_D_D0P_LP/MIPIC_D_D0N_LP (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-425-rule_engine_v3-SI.diff_pair_symmetry

## 426. 差分对 MIPIC_D_D1P_HS/MIPIC_D_D1N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-426
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIC_D_D1P_HS/MIPIC_D_D1N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-426-rule_engine_v3-SI.diff_pair_symmetry

## 427. 差分对 MIPIC_D_D2P_HS/MIPIC_D_D2N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-427
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIC_D_D2P_HS/MIPIC_D_D2N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-427-rule_engine_v3-SI.diff_pair_symmetry

## 428. 差分对 MIPIC_D_D3P_HS/MIPIC_D_D3N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-428
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIC_D_D3P_HS/MIPIC_D_D3N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-428-rule_engine_v3-SI.diff_pair_symmetry

## 429. 疑似差分对 MIPID_CLK_P/MIPID_CLK_N (置信度50%): 请人工确认
- **action_id**: ACT-429
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPID_CLK_P/MIPID_CLK_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-429-rule_engine_v3-SI.diff_pair_symmetry

## 430. 疑似差分对 MIPID_D0_P/MIPID_D0_N (置信度50%): 请人工确认
- **action_id**: ACT-430
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPID_D0_P/MIPID_D0_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-430-rule_engine_v3-SI.diff_pair_symmetry

## 431. 疑似差分对 MIPID_D1_P/MIPID_D1_N (置信度50%): 请人工确认
- **action_id**: ACT-431
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPID_D1_P/MIPID_D1_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-431-rule_engine_v3-SI.diff_pair_symmetry

## 432. 疑似差分对 MIPID_D2_P/MIPID_D2_N (置信度50%): 请人工确认
- **action_id**: ACT-432
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPID_D2_P/MIPID_D2_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-432-rule_engine_v3-SI.diff_pair_symmetry

## 433. 疑似差分对 MIPID_D3_P/MIPID_D3_N (置信度50%): 请人工确认
- **action_id**: ACT-433
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPID_D3_P/MIPID_D3_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-433-rule_engine_v3-SI.diff_pair_symmetry

## 434. 差分对 MIPID_D_D0P_HS/MIPID_D_D0N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-434
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPID_D_D0P_HS/MIPID_D_D0N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-434-rule_engine_v3-SI.diff_pair_symmetry

## 435. 疑似差分对 MIPID_D_D0P_LP/MIPID_D_D0N_LP (置信度50%): 请人工确认
- **action_id**: ACT-435
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPID_D_D0P_LP/MIPID_D_D0N_LP (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-435-rule_engine_v3-SI.diff_pair_symmetry

## 436. 差分对 MIPID_D_D1P_HS/MIPID_D_D1N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-436
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPID_D_D1P_HS/MIPID_D_D1N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-436-rule_engine_v3-SI.diff_pair_symmetry

## 437. 差分对 MIPID_D_D2P_HS/MIPID_D_D2N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-437
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPID_D_D2P_HS/MIPID_D_D2N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-437-rule_engine_v3-SI.diff_pair_symmetry

## 438. 差分对 MIPID_D_D3P_HS/MIPID_D_D3N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-438
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPID_D_D3P_HS/MIPID_D_D3N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-438-rule_engine_v3-SI.diff_pair_symmetry

## 439. 差分对 MIPIE_CLK_P/MIPIE_CLK_N (置信度90%): 对称 ✓
- **action_id**: ACT-439
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_CLK_P/MIPIE_CLK_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-439-rule_engine_v3-SI.diff_pair_symmetry

## 440. 差分对 MIPIE_D0_P/MIPIE_D0_N (置信度90%): 对称 ✓
- **action_id**: ACT-440
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_D0_P/MIPIE_D0_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-440-rule_engine_v3-SI.diff_pair_symmetry

## 441. 差分对 MIPIE_D1_P/MIPIE_D1_N (置信度90%): 对称 ✓
- **action_id**: ACT-441
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_D1_P/MIPIE_D1_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-441-rule_engine_v3-SI.diff_pair_symmetry

## 442. 差分对 MIPIE_D2_P/MIPIE_D2_N (置信度90%): 对称 ✓
- **action_id**: ACT-442
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_D2_P/MIPIE_D2_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-442-rule_engine_v3-SI.diff_pair_symmetry

## 443. 差分对 MIPIE_D3_P/MIPIE_D3_N (置信度90%): 对称 ✓
- **action_id**: ACT-443
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_D3_P/MIPIE_D3_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-443-rule_engine_v3-SI.diff_pair_symmetry

## 444. 差分对 MIPIE_D_D0P_HS/MIPIE_D_D0N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-444
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_D_D0P_HS/MIPIE_D_D0N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-444-rule_engine_v3-SI.diff_pair_symmetry

## 445. 差分对 MIPIE_D_D0P_LP/MIPIE_D_D0N_LP (置信度90%): 对称 ✓
- **action_id**: ACT-445
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_D_D0P_LP/MIPIE_D_D0N_LP (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-445-rule_engine_v3-SI.diff_pair_symmetry

## 446. 差分对 MIPIE_D_D1P_HS/MIPIE_D_D1N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-446
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_D_D1P_HS/MIPIE_D_D1N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-446-rule_engine_v3-SI.diff_pair_symmetry

## 447. 差分对 MIPIE_D_D2P_HS/MIPIE_D_D2N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-447
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_D_D2P_HS/MIPIE_D_D2N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-447-rule_engine_v3-SI.diff_pair_symmetry

## 448. 差分对 MIPIE_D_D3P_HS/MIPIE_D_D3N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-448
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIE_D_D3P_HS/MIPIE_D_D3N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-448-rule_engine_v3-SI.diff_pair_symmetry

## 449. 差分对 MIPIF_CLK_P/MIPIF_CLK_N (置信度90%): 对称 ✓
- **action_id**: ACT-449
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_CLK_P/MIPIF_CLK_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-449-rule_engine_v3-SI.diff_pair_symmetry

## 450. 差分对 MIPIF_D0_P/MIPIF_D0_N (置信度90%): 对称 ✓
- **action_id**: ACT-450
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_D0_P/MIPIF_D0_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-450-rule_engine_v3-SI.diff_pair_symmetry

## 451. 差分对 MIPIF_D1_P/MIPIF_D1_N (置信度90%): 对称 ✓
- **action_id**: ACT-451
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_D1_P/MIPIF_D1_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-451-rule_engine_v3-SI.diff_pair_symmetry

## 452. 差分对 MIPIF_D2_P/MIPIF_D2_N (置信度90%): 对称 ✓
- **action_id**: ACT-452
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_D2_P/MIPIF_D2_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-452-rule_engine_v3-SI.diff_pair_symmetry

## 453. 差分对 MIPIF_D3_P/MIPIF_D3_N (置信度90%): 对称 ✓
- **action_id**: ACT-453
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_D3_P/MIPIF_D3_N (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-453-rule_engine_v3-SI.diff_pair_symmetry

## 454. 差分对 MIPIF_D_D0P_HS/MIPIF_D_D0N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-454
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_D_D0P_HS/MIPIF_D_D0N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-454-rule_engine_v3-SI.diff_pair_symmetry

## 455. 差分对 MIPIF_D_D0P_LP/MIPIF_D_D0N_LP (置信度90%): 对称 ✓
- **action_id**: ACT-455
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_D_D0P_LP/MIPIF_D_D0N_LP (置信度90%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-455-rule_engine_v3-SI.diff_pair_symmetry

## 456. 差分对 MIPIF_D_D1P_HS/MIPIF_D_D1N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-456
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_D_D1P_HS/MIPIF_D_D1N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-456-rule_engine_v3-SI.diff_pair_symmetry

## 457. 差分对 MIPIF_D_D2P_HS/MIPIF_D_D2N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-457
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_D_D2P_HS/MIPIF_D_D2N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-457-rule_engine_v3-SI.diff_pair_symmetry

## 458. 差分对 MIPIF_D_D3P_HS/MIPIF_D_D3N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-458
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIF_D_D3P_HS/MIPIF_D_D3N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-458-rule_engine_v3-SI.diff_pair_symmetry

## 459. 疑似差分对 MIPIG_CLK_P/MIPIG_CLK_N (置信度50%): 请人工确认
- **action_id**: ACT-459
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIG_CLK_P/MIPIG_CLK_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-459-rule_engine_v3-SI.diff_pair_symmetry

## 460. 疑似差分对 MIPIG_D0_P/MIPIG_D0_N (置信度50%): 请人工确认
- **action_id**: ACT-460
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIG_D0_P/MIPIG_D0_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-460-rule_engine_v3-SI.diff_pair_symmetry

## 461. 疑似差分对 MIPIG_D1_P/MIPIG_D1_N (置信度50%): 请人工确认
- **action_id**: ACT-461
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIG_D1_P/MIPIG_D1_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-461-rule_engine_v3-SI.diff_pair_symmetry

## 462. 疑似差分对 MIPIG_D2_P/MIPIG_D2_N (置信度50%): 请人工确认
- **action_id**: ACT-462
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIG_D2_P/MIPIG_D2_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-462-rule_engine_v3-SI.diff_pair_symmetry

## 463. 疑似差分对 MIPIG_D3_P/MIPIG_D3_N (置信度50%): 请人工确认
- **action_id**: ACT-463
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIG_D3_P/MIPIG_D3_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-463-rule_engine_v3-SI.diff_pair_symmetry

## 464. 差分对 MIPIG_D_D0P_HS/MIPIG_D_D0N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-464
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIG_D_D0P_HS/MIPIG_D_D0N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-464-rule_engine_v3-SI.diff_pair_symmetry

## 465. 疑似差分对 MIPIG_D_D0P_LP/MIPIG_D_D0N_LP (置信度50%): 请人工确认
- **action_id**: ACT-465
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIG_D_D0P_LP/MIPIG_D_D0N_LP (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-465-rule_engine_v3-SI.diff_pair_symmetry

## 466. 差分对 MIPIG_D_D1P_HS/MIPIG_D_D1N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-466
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIG_D_D1P_HS/MIPIG_D_D1N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-466-rule_engine_v3-SI.diff_pair_symmetry

## 467. 差分对 MIPIG_D_D2P_HS/MIPIG_D_D2N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-467
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIG_D_D2P_HS/MIPIG_D_D2N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-467-rule_engine_v3-SI.diff_pair_symmetry

## 468. 差分对 MIPIG_D_D3P_HS/MIPIG_D_D3N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-468
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIG_D_D3P_HS/MIPIG_D_D3N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-468-rule_engine_v3-SI.diff_pair_symmetry

## 469. 疑似差分对 MIPIH_CLK_P/MIPIH_CLK_N (置信度50%): 请人工确认
- **action_id**: ACT-469
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIH_CLK_P/MIPIH_CLK_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-469-rule_engine_v3-SI.diff_pair_symmetry

## 470. 疑似差分对 MIPIH_D0_P/MIPIH_D0_N (置信度50%): 请人工确认
- **action_id**: ACT-470
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIH_D0_P/MIPIH_D0_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-470-rule_engine_v3-SI.diff_pair_symmetry

## 471. 疑似差分对 MIPIH_D1_P/MIPIH_D1_N (置信度50%): 请人工确认
- **action_id**: ACT-471
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIH_D1_P/MIPIH_D1_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-471-rule_engine_v3-SI.diff_pair_symmetry

## 472. 疑似差分对 MIPIH_D2_P/MIPIH_D2_N (置信度50%): 请人工确认
- **action_id**: ACT-472
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIH_D2_P/MIPIH_D2_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-472-rule_engine_v3-SI.diff_pair_symmetry

## 473. 疑似差分对 MIPIH_D3_P/MIPIH_D3_N (置信度50%): 请人工确认
- **action_id**: ACT-473
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIH_D3_P/MIPIH_D3_N (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-473-rule_engine_v3-SI.diff_pair_symmetry

## 474. 差分对 MIPIH_D_D0P_HS/MIPIH_D_D0N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-474
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIH_D_D0P_HS/MIPIH_D_D0N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-474-rule_engine_v3-SI.diff_pair_symmetry

## 475. 疑似差分对 MIPIH_D_D0P_LP/MIPIH_D_D0N_LP (置信度50%): 请人工确认
- **action_id**: ACT-475
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 疑似差分对 MIPIH_D_D0P_LP/MIPIH_D_D0N_LP (置信度50%): 请人工确认
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-475-rule_engine_v3-SI.diff_pair_symmetry

## 476. 差分对 MIPIH_D_D1P_HS/MIPIH_D_D1N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-476
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIH_D_D1P_HS/MIPIH_D_D1N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-476-rule_engine_v3-SI.diff_pair_symmetry

## 477. 差分对 MIPIH_D_D2P_HS/MIPIH_D_D2N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-477
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIH_D_D2P_HS/MIPIH_D_D2N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-477-rule_engine_v3-SI.diff_pair_symmetry

## 478. 差分对 MIPIH_D_D3P_HS/MIPIH_D_D3N_HS (置信度100%): 对称 ✓
- **action_id**: ACT-478
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 MIPIH_D_D3P_HS/MIPIH_D_D3N_HS (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-478-rule_engine_v3-SI.diff_pair_symmetry

## 479. 差分对 OSC_MIPI_VREF_CLK_P/OSC_MIPI_VREF_CLK_N (置信度100%): 对称 ✓
- **action_id**: ACT-479
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 OSC_MIPI_VREF_CLK_P/OSC_MIPI_VREF_CLK_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-479-rule_engine_v3-SI.diff_pair_symmetry

## 480. 差分对 SFP0_RX_P/SFP0_RX_N (置信度100%): 对称 ✓
- **action_id**: ACT-480
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 SFP0_RX_P/SFP0_RX_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-480-rule_engine_v3-SI.diff_pair_symmetry

## 481. 差分对 SFP0_TX_P/SFP0_TX_N (置信度100%): 对称 ✓
- **action_id**: ACT-481
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 SFP0_TX_P/SFP0_TX_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-481-rule_engine_v3-SI.diff_pair_symmetry

## 482. 差分对 SFP1_RX_P/SFP1_RX_N (置信度100%): 对称 ✓
- **action_id**: ACT-482
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 SFP1_RX_P/SFP1_RX_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-482-rule_engine_v3-SI.diff_pair_symmetry

## 483. 差分对 SFP1_TX_P/SFP1_TX_N (置信度100%): 对称 ✓
- **action_id**: ACT-483
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 SFP1_TX_P/SFP1_TX_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-483-rule_engine_v3-SI.diff_pair_symmetry

## 484. 差分对 SFP2_RX_P/SFP2_RX_N (置信度100%): 对称 ✓
- **action_id**: ACT-484
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 SFP2_RX_P/SFP2_RX_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-484-rule_engine_v3-SI.diff_pair_symmetry

## 485. 差分对 SFP2_TX_P/SFP2_TX_N (置信度100%): 对称 ✓
- **action_id**: ACT-485
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 SFP2_TX_P/SFP2_TX_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-485-rule_engine_v3-SI.diff_pair_symmetry

## 486. 差分对 SFP3_RX_P/SFP3_RX_N (置信度100%): 对称 ✓
- **action_id**: ACT-486
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 SFP3_RX_P/SFP3_RX_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-486-rule_engine_v3-SI.diff_pair_symmetry

## 487. 差分对 SFP3_TX_P/SFP3_TX_N (置信度100%): 对称 ✓
- **action_id**: ACT-487
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 SFP3_TX_P/SFP3_TX_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-487-rule_engine_v3-SI.diff_pair_symmetry

## 488. 差分对 SFP_VREF_CLK_P/SFP_VREF_CLK_N (置信度100%): 对称 ✓
- **action_id**: ACT-488
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.diff_pair_symmetry
- **category**: SI
- **location**: 
- **title**: 差分对 SFP_VREF_CLK_P/SFP_VREF_CLK_N (置信度100%): 对称 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-488-rule_engine_v3-SI.diff_pair_symmetry

## 489. I2C 网络 LOCK_SCL: 有上拉电阻 ✓
- **action_id**: ACT-489
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 LOCK_SCL: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-489-rule_engine_v3-SI.i2c_pullup

## 490. I2C 网络 M_I2C_SCL2: 有上拉电阻 ✓
- **action_id**: ACT-490
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_I2C_SCL2: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-490-rule_engine_v3-SI.i2c_pullup

## 491. I2C 网络 QSFP_SDA_: 有上拉电阻 ✓
- **action_id**: ACT-491
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 QSFP_SDA_: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-491-rule_engine_v3-SI.i2c_pullup

## 492. I2C 网络 QSFP_SCL_: 有上拉电阻 ✓
- **action_id**: ACT-492
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 QSFP_SCL_: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-492-rule_engine_v3-SI.i2c_pullup

## 493. I2C 网络 LOCK_SDA: 有上拉电阻 ✓
- **action_id**: ACT-493
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 LOCK_SDA: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-493-rule_engine_v3-SI.i2c_pullup

## 494. I2C 网络 M_I2C_SDA2: 有上拉电阻 ✓
- **action_id**: ACT-494
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_I2C_SDA2: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-494-rule_engine_v3-SI.i2c_pullup

## 495. I2C 网络 M_I2C_SDA2_: 有上拉电阻 ✓
- **action_id**: ACT-495
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_I2C_SDA2_: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-495-rule_engine_v3-SI.i2c_pullup

## 496. I2C 网络 M_I2C_SCL2_: 有上拉电阻 ✓
- **action_id**: ACT-496
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_I2C_SCL2_: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-496-rule_engine_v3-SI.i2c_pullup

## 497. I2C 网络 M_I2C_SCL1_: 有上拉电阻 ✓
- **action_id**: ACT-497
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_I2C_SCL1_: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-497-rule_engine_v3-SI.i2c_pullup

## 498. I2C 网络 M_I2C_SDA1_: 有上拉电阻 ✓
- **action_id**: ACT-498
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_I2C_SDA1_: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-498-rule_engine_v3-SI.i2c_pullup

## 499. I2C 网络 M_SDA: 有上拉电阻 ✓
- **action_id**: ACT-499
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_SDA: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-499-rule_engine_v3-SI.i2c_pullup

## 500. I2C 网络 M_I2C_SCL1: 有上拉电阻 ✓
- **action_id**: ACT-500
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_I2C_SCL1: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-500-rule_engine_v3-SI.i2c_pullup

## 501. I2C 网络 M_I2C_SDA1: 有上拉电阻 ✓
- **action_id**: ACT-501
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_I2C_SDA1: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-501-rule_engine_v3-SI.i2c_pullup

## 502. I2C 网络 M_SCL: 有上拉电阻 ✓
- **action_id**: ACT-502
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 M_SCL: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-502-rule_engine_v3-SI.i2c_pullup

## 503. I2C 网络 EX_POC_AMP_SCL: 有上拉电阻 ✓
- **action_id**: ACT-503
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 EX_POC_AMP_SCL: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-503-rule_engine_v3-SI.i2c_pullup

## 504. I2C 网络 EX_POC_AMP_SDA: 有上拉电阻 ✓
- **action_id**: ACT-504
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.i2c_pullup
- **category**: SI
- **location**: 
- **title**: I2C 网络 EX_POC_AMP_SDA: 有上拉电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-504-rule_engine_v3-SI.i2c_pullup

## 505. 复位网络 PMUBOARD_RST2: 有偏置电阻 ✓
- **action_id**: ACT-505
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 PMUBOARD_RST2: 有偏置电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-505-rule_engine_v3-SI.reset_bias

## 506. 复位网络 POW_RESET: 有偏置电阻 ✓
- **action_id**: ACT-506
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 POW_RESET: 有偏置电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-506-rule_engine_v3-SI.reset_bias

## 507. 复位网络 POW_RESET_: 有偏置电阻 ✓
- **action_id**: ACT-507
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 POW_RESET_: 有偏置电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-507-rule_engine_v3-SI.reset_bias

## 508. 复位网络 /CLK_DIVIDE_RST: 有偏置电阻 ✓
- **action_id**: ACT-508
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 /CLK_DIVIDE_RST: 有偏置电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-508-rule_engine_v3-SI.reset_bias

## 509. 复位网络 QSFP_RESETL: 有偏置电阻 ✓
- **action_id**: ACT-509
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 QSFP_RESETL: 有偏置电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-509-rule_engine_v3-SI.reset_bias

## 510. 复位网络 DDR4_RESET: 有偏置电阻 ✓
- **action_id**: ACT-510
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 DDR4_RESET: 有偏置电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-510-rule_engine_v3-SI.reset_bias

## 511. 复位网络 PMUBOARD_RST1: 有偏置电阻 ✓
- **action_id**: ACT-511
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.reset_bias
- **category**: SI
- **location**: 
- **title**: 复位网络 PMUBOARD_RST1: 有偏置电阻 ✓
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-511-rule_engine_v3-SI.reset_bias

## 512. 检查了 536 个信号网络，电压域一致
- **action_id**: ACT-512
- **priority**: P2
- **action_type**: manual_review
- **source**: rule_engine_v3
- **rule_id**: SI.voltage_domain_match
- **category**: SI
- **location**: 
- **title**: 检查了 536 个信号网络，电压域一致
- **recommended_action**: 人工确认该信息项是否需要转为设计约束或风险项。
- **decision_impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **evidence_id**: EVID-512-rule_engine_v3-SI.voltage_domain_match
