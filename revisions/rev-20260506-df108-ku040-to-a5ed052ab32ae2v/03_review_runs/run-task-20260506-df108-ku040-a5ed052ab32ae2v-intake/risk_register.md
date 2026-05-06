# Risk Register

## 1. RISK-001
- **risk_id**: RISK-001
- **severity**: ERROR
- **priority**: P0
- **category**: SYSTEM
- **source**: board_review
- **description**: Board review failed: 'DiffPairCheck' object has no attribute 'pair_name'
- **impact**: SYSTEM 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 修复后重新运行 sch-review，并确认该项关闭。
- **status**: open
- **evidence_id**: EVID-001-board_review-ENGINE-ERROR

## 2. RISK-002
- **risk_id**: RISK-002
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: A_DC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-002-power_tree-PWR-RISK

## 3. RISK-003
- **risk_id**: RISK-003
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: A_POC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-003-power_tree-PWR-RISK

## 4. RISK-004
- **risk_id**: RISK-004
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: B_DC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-004-power_tree-PWR-RISK

## 5. RISK-005
- **risk_id**: RISK-005
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: B_POC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-005-power_tree-PWR-RISK

## 6. RISK-006
- **risk_id**: RISK-006
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: C_DC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-006-power_tree-PWR-RISK

## 7. RISK-007
- **risk_id**: RISK-007
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: C_POC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-007-power_tree-PWR-RISK

## 8. RISK-008
- **risk_id**: RISK-008
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: D_DC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-008-power_tree-PWR-RISK

## 9. RISK-009
- **risk_id**: RISK-009
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: D_POC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-009-power_tree-PWR-RISK

## 10. RISK-010
- **risk_id**: RISK-010
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点: EX_IO1_1V8 (1.8V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-010-power_tree-PWR-RISK

## 11. RISK-011
- **risk_id**: RISK-011
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点: EX_IO2_1V8 (1.8V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-011-power_tree-PWR-RISK

## 12. RISK-012
- **risk_id**: RISK-012
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: EX_POC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-012-power_tree-PWR-RISK

## 13. RISK-013
- **risk_id**: RISK-013
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: E_DC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-013-power_tree-PWR-RISK

## 14. RISK-014
- **risk_id**: RISK-014
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: E_POC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-014-power_tree-PWR-RISK

## 15. RISK-015
- **risk_id**: RISK-015
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: FAN_12V (12.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-015-power_tree-PWR-RISK

## 16. RISK-016
- **risk_id**: RISK-016
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点: FPGA_1V8 (1.8V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-016-power_tree-PWR-RISK

## 17. RISK-017
- **risk_id**: RISK-017
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: F_DC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-017-power_tree-PWR-RISK

## 18. RISK-018
- **risk_id**: RISK-018
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: F_POC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-018-power_tree-PWR-RISK

## 19. RISK-019
- **risk_id**: RISK-019
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: G_DC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-019-power_tree-PWR-RISK

## 20. RISK-020
- **risk_id**: RISK-020
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: G_POC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-020-power_tree-PWR-RISK

## 21. RISK-021
- **risk_id**: RISK-021
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: H_DC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-021-power_tree-PWR-RISK

## 22. RISK-022
- **risk_id**: RISK-022
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: H_POC_PWR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-022-power_tree-PWR-RISK

## 23. RISK-023
- **risk_id**: RISK-023
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合: M1V8 (1.8V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-023-power_tree-PWR-RISK

## 24. RISK-024
- **risk_id**: RISK-024
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合: M24V (24.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-024-power_tree-PWR-RISK

## 25. RISK-025
- **risk_id**: RISK-025
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点: MGTVCCAUX_R (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-025-power_tree-PWR-RISK

## 26. RISK-026
- **risk_id**: RISK-026
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点: UART_RX_F/EX_IO3_1V8 (1.8V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-026-power_tree-PWR-RISK

## 27. RISK-027
- **risk_id**: RISK-027
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点: UART_TX_F/EX_IO4_1V8 (1.8V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-027-power_tree-PWR-RISK

## 28. RISK-028
- **risk_id**: RISK-028
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: VCC1 (1.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-028-power_tree-PWR-RISK

## 29. RISK-029
- **risk_id**: RISK-029
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点: VCCAUX (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-029-power_tree-PWR-RISK

## 30. RISK-030
- **risk_id**: RISK-030
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: VCCR (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-030-power_tree-PWR-RISK

## 31. RISK-031
- **risk_id**: RISK-031
- **severity**: ERROR
- **priority**: P0
- **category**: POWER
- **source**: power_tree
- **description**: 上游未闭合 / 缺测试点 / 外部依赖: VCCT (0.0V)
- **impact**: POWER 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 检查电源链路完整性
- **status**: open
- **evidence_id**: EVID-031-power_tree-PWR-RISK

## 32. RISK-032
- **risk_id**: RISK-032
- **severity**: ERROR
- **priority**: P0
- **category**: PI
- **source**: rule_engine_v3
- **description**: U9 没有连接到 GND
- **impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 连接的网络: ['NC']
- **status**: open
- **evidence_id**: EVID-032-rule_engine_v3-PI.ic_grounding

## 33. RISK-033
- **risk_id**: RISK-033
- **severity**: ERROR
- **priority**: P0
- **category**: PI
- **source**: rule_engine_v3
- **description**: U122 没有连接到任何电源网络
- **impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 连接的网络: ['N20359018', 'N20359112', 'NC', 'S3V3']
- **status**: open
- **evidence_id**: EVID-033-rule_engine_v3-PI.ic_power_supply

## 34. RISK-034
- **risk_id**: RISK-034
- **severity**: ERROR
- **priority**: P0
- **category**: PI
- **source**: rule_engine_v3
- **description**: U123 没有连接到任何电源网络
- **impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 连接的网络: ['N20361029', 'N20361040', 'N20361064', 'NC']
- **status**: open
- **evidence_id**: EVID-034-rule_engine_v3-PI.ic_power_supply

## 35. RISK-035
- **risk_id**: RISK-035
- **severity**: ERROR
- **priority**: P0
- **category**: PI
- **source**: rule_engine_v3
- **description**: U124 没有连接到任何电源网络
- **impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 连接的网络: ['N20360328', 'N20360401', 'N20360576', 'POW_EN', 'S3V3']
- **status**: open
- **evidence_id**: EVID-035-rule_engine_v3-PI.ic_power_supply

## 36. RISK-036
- **risk_id**: RISK-036
- **severity**: ERROR
- **priority**: P0
- **category**: PI
- **source**: rule_engine_v3
- **description**: U125 没有连接到任何电源网络
- **impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 连接的网络: ['POW_EN', 'POW_EN1', 'POW_EN2', 'POW_EN3', 'S3V3']
- **status**: open
- **evidence_id**: EVID-036-rule_engine_v3-PI.ic_power_supply

## 37. RISK-037
- **risk_id**: RISK-037
- **severity**: ERROR
- **priority**: P0
- **category**: PI
- **source**: rule_engine_v3
- **description**: U260 没有连接到任何电源网络
- **impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 连接的网络: ['EX_POC_VOLTAGE_TEST', 'N25616805', 'N25642853', 'NC']
- **status**: open
- **evidence_id**: EVID-037-rule_engine_v3-PI.ic_power_supply

## 38. RISK-038
- **risk_id**: RISK-038
- **severity**: ERROR
- **priority**: P0
- **category**: PI
- **source**: rule_engine_v3
- **description**: U1 没有连接到任何电源网络
- **impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 连接的网络: ['N20357505', 'N20357507']
- **status**: open
- **evidence_id**: EVID-038-rule_engine_v3-PI.ic_power_supply

## 39. RISK-039
- **risk_id**: RISK-039
- **severity**: ERROR
- **priority**: P0
- **category**: PI
- **source**: rule_engine_v3
- **description**: U154 没有连接到任何电源网络
- **impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 连接的网络: ['EX_POC_AMP_SCL', 'EX_POC_AMP_SDA', 'N25558477', 'N25582134']
- **status**: open
- **evidence_id**: EVID-039-rule_engine_v3-PI.ic_power_supply

## 40. RISK-040
- **risk_id**: RISK-040
- **severity**: ERROR
- **priority**: P0
- **category**: PI
- **source**: rule_engine_v3
- **description**: U9 没有连接到任何电源网络
- **impact**: PI 类阻断风险，可能导致设计不可用、启动失败或验证返工。
- **mitigation**: 连接的网络: ['NC']
- **status**: open
- **evidence_id**: EVID-040-rule_engine_v3-PI.ic_power_supply

## 41. RISK-041
- **risk_id**: RISK-041
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点 / 外部依赖: 24_VIN (24.0V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-041-power_tree-PWR-RISK

## 42. RISK-042
- **risk_id**: RISK-042
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: DDR4_VDD (1.2V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-042-power_tree-PWR-RISK

## 43. RISK-043
- **risk_id**: RISK-043
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: FPGA_1V2 (1.2V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-043-power_tree-PWR-RISK

## 44. RISK-044
- **risk_id**: RISK-044
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: FPGA_3V3 (3.3V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-044-power_tree-PWR-RISK

## 45. RISK-045
- **risk_id**: RISK-045
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: M3V3 (3.3V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-045-power_tree-PWR-RISK

## 46. RISK-046
- **risk_id**: RISK-046
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: M5V (5.0V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-046-power_tree-PWR-RISK

## 47. RISK-047
- **risk_id**: RISK-047
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: M5V_A-D (5.0V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-047-power_tree-PWR-RISK

## 48. RISK-048
- **risk_id**: RISK-048
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: M5V_E-H (5.0V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-048-power_tree-PWR-RISK

## 49. RISK-049
- **risk_id**: RISK-049
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: MGTAVCC_L (1.0V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-049-power_tree-PWR-RISK

## 50. RISK-050
- **risk_id**: RISK-050
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: MGTAVCC_R (1.0V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-050-power_tree-PWR-RISK

## 51. RISK-051
- **risk_id**: RISK-051
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: PMU1_VDDIO (3.3V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-051-power_tree-PWR-RISK

## 52. RISK-052
- **risk_id**: RISK-052
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: PMU2_VDDIO (3.3V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-052-power_tree-PWR-RISK

## 53. RISK-053
- **risk_id**: RISK-053
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: VCCINT (0.95V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-053-power_tree-PWR-RISK

## 54. RISK-054
- **risk_id**: RISK-054
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: VDDIO_A-D (3.3V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-054-power_tree-PWR-RISK

## 55. RISK-055
- **risk_id**: RISK-055
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: VDDIO_B6465 (3.3V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-055-power_tree-PWR-RISK

## 56. RISK-056
- **risk_id**: RISK-056
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: VDDIO_E-H (3.3V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-056-power_tree-PWR-RISK

## 57. RISK-057
- **risk_id**: RISK-057
- **severity**: WARNING
- **priority**: P1
- **category**: POWER
- **source**: power_tree
- **description**: 缺测试点: VDDIO_OUT (3.3V)
- **impact**: POWER 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-057-power_tree-PWR-RISK

## 58. RISK-058
- **risk_id**: RISK-058
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 电路有 34 个独立分量（可能有断开的子电路）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 分量大小: [2630, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
- **status**: open
- **evidence_id**: EVID-058-rule_engine_v3-CONN.connected_components

## 59. RISK-059
- **risk_id**: RISK-059
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U14.IO_L12P_T1U_N10_GC_A08_D24_65/H: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-059-rule_engine_v3-CONN.device_id_pins

## 60. RISK-060
- **risk_id**: RISK-060
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U14.IO_T0U_N12_A28_65/HR: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-060-rule_engine_v3-CONN.device_id_pins

## 61. RISK-061
- **risk_id**: RISK-061
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U44.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-061-rule_engine_v3-CONN.device_id_pins

## 62. RISK-062
- **risk_id**: RISK-062
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U44.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-062-rule_engine_v3-CONN.device_id_pins

## 63. RISK-063
- **risk_id**: RISK-063
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U36.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-063-rule_engine_v3-CONN.device_id_pins

## 64. RISK-064
- **risk_id**: RISK-064
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U36.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-064-rule_engine_v3-CONN.device_id_pins

## 65. RISK-065
- **risk_id**: RISK-065
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U105.A2: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-065-rule_engine_v3-CONN.device_id_pins

## 66. RISK-066
- **risk_id**: RISK-066
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U56.A0+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-066-rule_engine_v3-CONN.device_id_pins

## 67. RISK-067
- **risk_id**: RISK-067
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U56.A0-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-067-rule_engine_v3-CONN.device_id_pins

## 68. RISK-068
- **risk_id**: RISK-068
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U16.A2: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-068-rule_engine_v3-CONN.device_id_pins

## 69. RISK-069
- **risk_id**: RISK-069
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U18.A2: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-069-rule_engine_v3-CONN.device_id_pins

## 70. RISK-070
- **risk_id**: RISK-070
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U69.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-070-rule_engine_v3-CONN.device_id_pins

## 71. RISK-071
- **risk_id**: RISK-071
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U69.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-071-rule_engine_v3-CONN.device_id_pins

## 72. RISK-072
- **risk_id**: RISK-072
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U37.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-072-rule_engine_v3-CONN.device_id_pins

## 73. RISK-073
- **risk_id**: RISK-073
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U37.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-073-rule_engine_v3-CONN.device_id_pins

## 74. RISK-074
- **risk_id**: RISK-074
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U62.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-074-rule_engine_v3-CONN.device_id_pins

## 75. RISK-075
- **risk_id**: RISK-075
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U62.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-075-rule_engine_v3-CONN.device_id_pins

## 76. RISK-076
- **risk_id**: RISK-076
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U91.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-076-rule_engine_v3-CONN.device_id_pins

## 77. RISK-077
- **risk_id**: RISK-077
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U91.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-077-rule_engine_v3-CONN.device_id_pins

## 78. RISK-078
- **risk_id**: RISK-078
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U58.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-078-rule_engine_v3-CONN.device_id_pins

## 79. RISK-079
- **risk_id**: RISK-079
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U58.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-079-rule_engine_v3-CONN.device_id_pins

## 80. RISK-080
- **risk_id**: RISK-080
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U32.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-080-rule_engine_v3-CONN.device_id_pins

## 81. RISK-081
- **risk_id**: RISK-081
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U32.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-081-rule_engine_v3-CONN.device_id_pins

## 82. RISK-082
- **risk_id**: RISK-082
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U63.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-082-rule_engine_v3-CONN.device_id_pins

## 83. RISK-083
- **risk_id**: RISK-083
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U63.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-083-rule_engine_v3-CONN.device_id_pins

## 84. RISK-084
- **risk_id**: RISK-084
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U53.A1+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-084-rule_engine_v3-CONN.device_id_pins

## 85. RISK-085
- **risk_id**: RISK-085
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U53.A1-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-085-rule_engine_v3-CONN.device_id_pins

## 86. RISK-086
- **risk_id**: RISK-086
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U93.A0+: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-086-rule_engine_v3-CONN.device_id_pins

## 87. RISK-087
- **risk_id**: RISK-087
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U93.A0-: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-087-rule_engine_v3-CONN.device_id_pins

## 88. RISK-088
- **risk_id**: RISK-088
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.APROBE_GTSL1A_CH3,BA107: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-088-rule_engine_v3-CONN.device_id_pins

## 89. RISK-089
- **risk_id**: RISK-089
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.APROBE_GTSR4A_CH3,BA29: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-089-rule_engine_v3-CONN.device_id_pins

## 90. RISK-090
- **risk_id**: RISK-090
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.DNU,BA104: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-090-rule_engine_v3-CONN.device_id_pins

## 91. RISK-091
- **risk_id**: RISK-091
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,A103: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-091-rule_engine_v3-CONN.device_id_pins

## 92. RISK-092
- **risk_id**: RISK-092
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,A119: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-092-rule_engine_v3-CONN.device_id_pins

## 93. RISK-093
- **risk_id**: RISK-093
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,A132: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-093-rule_engine_v3-CONN.device_id_pins

## 94. RISK-094
- **risk_id**: RISK-094
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,A134: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-094-rule_engine_v3-CONN.device_id_pins

## 95. RISK-095
- **risk_id**: RISK-095
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,A26: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-095-rule_engine_v3-CONN.device_id_pins

## 96. RISK-096
- **risk_id**: RISK-096
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,AA134: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-096-rule_engine_v3-CONN.device_id_pins

## 97. RISK-097
- **risk_id**: RISK-097
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,AA2: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-097-rule_engine_v3-CONN.device_id_pins

## 98. RISK-098
- **risk_id**: RISK-098
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA1: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-098-rule_engine_v3-CONN.device_id_pins

## 99. RISK-099
- **risk_id**: RISK-099
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA100: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-099-rule_engine_v3-CONN.device_id_pins

## 100. RISK-100
- **risk_id**: RISK-100
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA111: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-100-rule_engine_v3-CONN.device_id_pins

## 101. RISK-101
- **risk_id**: RISK-101
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA115: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-101-rule_engine_v3-CONN.device_id_pins

## 102. RISK-102
- **risk_id**: RISK-102
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA120: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-102-rule_engine_v3-CONN.device_id_pins

## 103. RISK-103
- **risk_id**: RISK-103
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA123: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-103-rule_engine_v3-CONN.device_id_pins

## 104. RISK-104
- **risk_id**: RISK-104
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA13: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-104-rule_engine_v3-CONN.device_id_pins

## 105. RISK-105
- **risk_id**: RISK-105
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA131: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-105-rule_engine_v3-CONN.device_id_pins

## 106. RISK-106
- **risk_id**: RISK-106
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA133: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-106-rule_engine_v3-CONN.device_id_pins

## 107. RISK-107
- **risk_id**: RISK-107
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA135: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-107-rule_engine_v3-CONN.device_id_pins

## 108. RISK-108
- **risk_id**: RISK-108
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA16: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-108-rule_engine_v3-CONN.device_id_pins

## 109. RISK-109
- **risk_id**: RISK-109
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA21: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-109-rule_engine_v3-CONN.device_id_pins

## 110. RISK-110
- **risk_id**: RISK-110
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,BA25: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-110-rule_engine_v3-CONN.device_id_pins

## 111. RISK-111
- **risk_id**: RISK-111
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,CA19: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-111-rule_engine_v3-CONN.device_id_pins

## 112. RISK-112
- **risk_id**: RISK-112
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GND,CA28: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-112-rule_engine_v3-CONN.device_id_pins

## 113. RISK-113
- **risk_id**: RISK-113
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GTSL1B_TX_CH2N,BA126: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-113-rule_engine_v3-CONN.device_id_pins

## 114. RISK-114
- **risk_id**: RISK-114
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GTSL1B_TX_CH2P,BA129: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-114-rule_engine_v3-CONN.device_id_pins

## 115. RISK-115
- **risk_id**: RISK-115
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.GTSR4B_TX_CH2N,BA10: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-115-rule_engine_v3-CONN.device_id_pins

## 116. RISK-116
- **risk_id**: RISK-116
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.NC,AA1: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-116-rule_engine_v3-CONN.device_id_pins

## 117. RISK-117
- **risk_id**: RISK-117
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.NC,AA135: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-117-rule_engine_v3-CONN.device_id_pins

## 118. RISK-118
- **risk_id**: RISK-118
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.SDM_IO1,AVSTX8_DATA2,AS_DATA1: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-118-rule_engine_v3-CONN.device_id_pins

## 119. RISK-119
- **risk_id**: RISK-119
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.SDM_IO11,AVSTX8_VALID,PWRMGT_SD: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-119-rule_engine_v3-CONN.device_id_pins

## 120. RISK-120
- **risk_id**: RISK-120
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.SDM_IO2,AVSTX8_DATA0,AS_CLK: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-120-rule_engine_v3-CONN.device_id_pins

## 121. RISK-121
- **risk_id**: RISK-121
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.SDM_IO3,AVSTX8_DATA3,AS_DATA2: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-121-rule_engine_v3-CONN.device_id_pins

## 122. RISK-122
- **risk_id**: RISK-122
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: U9.SDM_IO4,AVSTX8_DATA1,AS_DATA0: 地址/ID 引脚未连接 (NC)
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-122-rule_engine_v3-CONN.device_id_pins

## 123. RISK-123
- **risk_id**: RISK-123
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J20 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-123-rule_engine_v3-CONN.isolated_devices

## 124. RISK-124
- **risk_id**: RISK-124
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J21 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-124-rule_engine_v3-CONN.isolated_devices

## 125. RISK-125
- **risk_id**: RISK-125
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J22 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-125-rule_engine_v3-CONN.isolated_devices

## 126. RISK-126
- **risk_id**: RISK-126
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J23 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-126-rule_engine_v3-CONN.isolated_devices

## 127. RISK-127
- **risk_id**: RISK-127
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J24 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-127-rule_engine_v3-CONN.isolated_devices

## 128. RISK-128
- **risk_id**: RISK-128
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J25 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-128-rule_engine_v3-CONN.isolated_devices

## 129. RISK-129
- **risk_id**: RISK-129
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J26 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-129-rule_engine_v3-CONN.isolated_devices

## 130. RISK-130
- **risk_id**: RISK-130
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J27 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-130-rule_engine_v3-CONN.isolated_devices

## 131. RISK-131
- **risk_id**: RISK-131
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J28 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-131-rule_engine_v3-CONN.isolated_devices

## 132. RISK-132
- **risk_id**: RISK-132
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J16 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-132-rule_engine_v3-CONN.isolated_devices

## 133. RISK-133
- **risk_id**: RISK-133
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: J17 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-133-rule_engine_v3-CONN.isolated_devices

## 134. RISK-134
- **risk_id**: RISK-134
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: P1 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-134-rule_engine_v3-CONN.isolated_devices

## 135. RISK-135
- **risk_id**: RISK-135
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: P2 只连接到 GND（可能未连接）
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-135-rule_engine_v3-CONN.isolated_devices

## 136. RISK-136
- **risk_id**: RISK-136
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 DDR4_DQS_P2: 多个输出引脚冲突 — U14.IO_L16P_T2U_N6_QBC_AD3P_44/HP, U5.LDQS_T
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-136-rule_engine_v3-CONN.output_conflict

## 137. RISK-137
- **risk_id**: RISK-137
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 DDR4_DQS_N2: 多个输出引脚冲突 — U14.IO_L16N_T2U_N7_QBC_AD3N_44/HP, U5.LDQS_C
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-137-rule_engine_v3-CONN.output_conflict

## 138. RISK-138
- **risk_id**: RISK-138
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 MA_BF_D_D3_HS_P: 多个输出引脚冲突 — U14.IO_L10P_T1U_N6_QBC_AD4P_48/HP, U25.OUT+
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-138-rule_engine_v3-CONN.output_conflict

## 139. RISK-139
- **risk_id**: RISK-139
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 DDR4_DQS_P1: 多个输出引脚冲突 — U14.IO_L10P_T1U_N6_QBC_AD4P_44/HP, U6.UDQS_T
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-139-rule_engine_v3-CONN.output_conflict

## 140. RISK-140
- **risk_id**: RISK-140
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 DDR4_DQS_N1: 多个输出引脚冲突 — U14.IO_L10N_T1U_N7_QBC_AD4N_44/HP, U6.UDQS_C
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-140-rule_engine_v3-CONN.output_conflict

## 141. RISK-141
- **risk_id**: RISK-141
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 DDR4_DQS_P5: 多个输出引脚冲突 — U14.IO_L10P_T1U_N6_QBC_AD4P_46/HP, U4.UDQS_T
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-141-rule_engine_v3-CONN.output_conflict

## 142. RISK-142
- **risk_id**: RISK-142
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 DDR4_DQS_N5: 多个输出引脚冲突 — U14.IO_L10N_T1U_N7_QBC_AD4N_46/HP, U4.UDQS_C
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-142-rule_engine_v3-CONN.output_conflict

## 143. RISK-143
- **risk_id**: RISK-143
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 MA_BF_D_D3_HS_N: 多个输出引脚冲突 — U14.IO_L10N_T1U_N7_QBC_AD4N_48/HP, U25.OUT-
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-143-rule_engine_v3-CONN.output_conflict

## 144. RISK-144
- **risk_id**: RISK-144
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 DDR4_DQS_P6: 多个输出引脚冲突 — U14.IO_L16P_T2U_N6_QBC_AD3P_46/HP, U3.LDQS_T
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-144-rule_engine_v3-CONN.output_conflict

## 145. RISK-145
- **risk_id**: RISK-145
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 DDR4_DQS_N6: 多个输出引脚冲突 — U14.IO_L16N_T2U_N7_QBC_AD3N_46/HP, U3.LDQS_C
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-145-rule_engine_v3-CONN.output_conflict

## 146. RISK-146
- **risk_id**: RISK-146
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 ME_SERDES_D3_HS_N: 输入引脚 U14.MGTHRXN2_228/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-146-rule_engine_v3-CONN.undriven_inputs

## 147. RISK-147
- **risk_id**: RISK-147
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 ME_SERDES_D0_HS_P: 输入引脚 U14.MGTHRXP1_228/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-147-rule_engine_v3-CONN.undriven_inputs

## 148. RISK-148
- **risk_id**: RISK-148
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 ME_SERDES_D0_HS_N: 输入引脚 U14.MGTHRXN1_228/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-148-rule_engine_v3-CONN.undriven_inputs

## 149. RISK-149
- **risk_id**: RISK-149
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 ME_SERDES_D2_HS_P: 输入引脚 U14.MGTHRXP3_228/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-149-rule_engine_v3-CONN.undriven_inputs

## 150. RISK-150
- **risk_id**: RISK-150
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 ME_SERDES_D2_HS_N: 输入引脚 U14.MGTHRXN3_228/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-150-rule_engine_v3-CONN.undriven_inputs

## 151. RISK-151
- **risk_id**: RISK-151
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 MF_SERDES_D0_HS_P: 输入引脚 U14.MGTHRXP3_227/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-151-rule_engine_v3-CONN.undriven_inputs

## 152. RISK-152
- **risk_id**: RISK-152
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 MF_SERDES_D0_HS_N: 输入引脚 U14.MGTHRXN3_227/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-152-rule_engine_v3-CONN.undriven_inputs

## 153. RISK-153
- **risk_id**: RISK-153
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 MF_SERDES_D2_HS_P: 输入引脚 U14.MGTHRXP1_227/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-153-rule_engine_v3-CONN.undriven_inputs

## 154. RISK-154
- **risk_id**: RISK-154
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 MF_SERDES_D2_HS_N: 输入引脚 U14.MGTHRXN1_227/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-154-rule_engine_v3-CONN.undriven_inputs

## 155. RISK-155
- **risk_id**: RISK-155
- **severity**: WARNING
- **priority**: P1
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 网络 MG_SERDES_D1_HS_N: 输入引脚 U14.MGTHRXN3_225/GTH 可能无驱动源
- **impact**: CONN 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-155-rule_engine_v3-CONN.undriven_inputs

## 156. RISK-156
- **risk_id**: RISK-156
- **severity**: WARNING
- **priority**: P1
- **category**: DBG
- **source**: rule_engine_v3
- **description**: U122: MCU/FPGA 无调试接口
- **impact**: DBG 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-156-rule_engine_v3-DBG.debug_interface

## 157. RISK-157
- **risk_id**: RISK-157
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: A-D_DECODER_5V_EN: 有 1 个 IC 负载但无去耦电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: IC: ['U14']
- **status**: open
- **evidence_id**: EVID-157-rule_engine_v3-PI.decoupling_caps

## 158. RISK-158
- **risk_id**: RISK-158
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: A-D_DECODER_VDDIO_EN: 有 1 个 IC 负载但无去耦电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: IC: ['U14']
- **status**: open
- **evidence_id**: EVID-158-rule_engine_v3-PI.decoupling_caps

## 159. RISK-159
- **risk_id**: RISK-159
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: E-H_DECODER_5V_EN: 有 1 个 IC 负载但无去耦电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: IC: ['U14']
- **status**: open
- **evidence_id**: EVID-159-rule_engine_v3-PI.decoupling_caps

## 160. RISK-160
- **risk_id**: RISK-160
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: E-H__DECODER_VDDIO_EN: 有 1 个 IC 负载但无去耦电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: IC: ['U14']
- **status**: open
- **evidence_id**: EVID-160-rule_engine_v3-PI.decoupling_caps

## 161. RISK-161
- **risk_id**: RISK-161
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: EX_IO1_1V8: 有 1 个 IC 负载但无去耦电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: IC: ['U14']
- **status**: open
- **evidence_id**: EVID-161-rule_engine_v3-PI.decoupling_caps

## 162. RISK-162
- **risk_id**: RISK-162
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: EX_IO2_1V8: 有 1 个 IC 负载但无去耦电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: IC: ['U14']
- **status**: open
- **evidence_id**: EVID-162-rule_engine_v3-PI.decoupling_caps

## 163. RISK-163
- **risk_id**: RISK-163
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: UART_RX_F/EX_IO3_1V8: 有 2 个 IC 负载但无去耦电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: IC: ['U14', 'U18']
- **status**: open
- **evidence_id**: EVID-163-rule_engine_v3-PI.decoupling_caps

## 164. RISK-164
- **risk_id**: RISK-164
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: UART_TX_F/EX_IO4_1V8: 有 2 个 IC 负载但无去耦电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: IC: ['U14', 'U16']
- **status**: open
- **evidence_id**: EVID-164-rule_engine_v3-PI.decoupling_caps

## 165. RISK-165
- **risk_id**: RISK-165
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: EN 信号 POW_EN2: 连接 3 个 IC 但无滤波电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-165-rule_engine_v3-PI.enable_pin_filter

## 166. RISK-166
- **risk_id**: RISK-166
- **severity**: WARNING
- **priority**: P1
- **category**: PI
- **source**: rule_engine_v3
- **description**: EN 信号 POW_EN1: 连接 3 个 IC 但无滤波电容
- **impact**: PI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-166-rule_engine_v3-PI.enable_pin_filter

## 167. RISK-167
- **risk_id**: RISK-167
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 A_I2C1_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN32', 'RN5']
- **status**: open
- **evidence_id**: EVID-167-rule_engine_v3-SI.i2c_pullup

## 168. RISK-168
- **risk_id**: RISK-168
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 A_I2C2_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN32', 'RN5']
- **status**: open
- **evidence_id**: EVID-168-rule_engine_v3-SI.i2c_pullup

## 169. RISK-169
- **risk_id**: RISK-169
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 A_I2C2_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN32', 'RN5']
- **status**: open
- **evidence_id**: EVID-169-rule_engine_v3-SI.i2c_pullup

## 170. RISK-170
- **risk_id**: RISK-170
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 H_I2C1_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN41']
- **status**: open
- **evidence_id**: EVID-170-rule_engine_v3-SI.i2c_pullup

## 171. RISK-171
- **risk_id**: RISK-171
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 H_I2C1_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN41']
- **status**: open
- **evidence_id**: EVID-171-rule_engine_v3-SI.i2c_pullup

## 172. RISK-172
- **risk_id**: RISK-172
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 H_I2C2_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN41']
- **status**: open
- **evidence_id**: EVID-172-rule_engine_v3-SI.i2c_pullup

## 173. RISK-173
- **risk_id**: RISK-173
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 H_I2C2_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN41']
- **status**: open
- **evidence_id**: EVID-173-rule_engine_v3-SI.i2c_pullup

## 174. RISK-174
- **risk_id**: RISK-174
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 C_I2C1_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN33', 'RN34']
- **status**: open
- **evidence_id**: EVID-174-rule_engine_v3-SI.i2c_pullup

## 175. RISK-175
- **risk_id**: RISK-175
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 C_I2C1_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN33', 'RN34']
- **status**: open
- **evidence_id**: EVID-175-rule_engine_v3-SI.i2c_pullup

## 176. RISK-176
- **risk_id**: RISK-176
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 H_I2C2_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN36', 'RN41']
- **status**: open
- **evidence_id**: EVID-176-rule_engine_v3-SI.i2c_pullup

## 177. RISK-177
- **risk_id**: RISK-177
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 E_I2C1_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN31', 'RN35']
- **status**: open
- **evidence_id**: EVID-177-rule_engine_v3-SI.i2c_pullup

## 178. RISK-178
- **risk_id**: RISK-178
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 H_I2C2_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN36', 'RN41']
- **status**: open
- **evidence_id**: EVID-178-rule_engine_v3-SI.i2c_pullup

## 179. RISK-179
- **risk_id**: RISK-179
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 B_I2C1_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN37', 'RN38']
- **status**: open
- **evidence_id**: EVID-179-rule_engine_v3-SI.i2c_pullup

## 180. RISK-180
- **risk_id**: RISK-180
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 E_I2C1_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN31', 'RN35']
- **status**: open
- **evidence_id**: EVID-180-rule_engine_v3-SI.i2c_pullup

## 181. RISK-181
- **risk_id**: RISK-181
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 B_I2C1_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN37', 'RN38']
- **status**: open
- **evidence_id**: EVID-181-rule_engine_v3-SI.i2c_pullup

## 182. RISK-182
- **risk_id**: RISK-182
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 G_I2C1_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN30', 'RN4']
- **status**: open
- **evidence_id**: EVID-182-rule_engine_v3-SI.i2c_pullup

## 183. RISK-183
- **risk_id**: RISK-183
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 G_I2C1_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN30', 'RN4']
- **status**: open
- **evidence_id**: EVID-183-rule_engine_v3-SI.i2c_pullup

## 184. RISK-184
- **risk_id**: RISK-184
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 G_I2C2_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN30']
- **status**: open
- **evidence_id**: EVID-184-rule_engine_v3-SI.i2c_pullup

## 185. RISK-185
- **risk_id**: RISK-185
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 F_I2C1_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN18']
- **status**: open
- **evidence_id**: EVID-185-rule_engine_v3-SI.i2c_pullup

## 186. RISK-186
- **risk_id**: RISK-186
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 F_I2C1_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN18', 'RN21']
- **status**: open
- **evidence_id**: EVID-186-rule_engine_v3-SI.i2c_pullup

## 187. RISK-187
- **risk_id**: RISK-187
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 F_I2C1_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN18', 'RN21']
- **status**: open
- **evidence_id**: EVID-187-rule_engine_v3-SI.i2c_pullup

## 188. RISK-188
- **risk_id**: RISK-188
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 F_I2C2_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN18', 'RN21']
- **status**: open
- **evidence_id**: EVID-188-rule_engine_v3-SI.i2c_pullup

## 189. RISK-189
- **risk_id**: RISK-189
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 F_I2C2_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN18', 'RN21']
- **status**: open
- **evidence_id**: EVID-189-rule_engine_v3-SI.i2c_pullup

## 190. RISK-190
- **risk_id**: RISK-190
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 G_I2C1_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN30']
- **status**: open
- **evidence_id**: EVID-190-rule_engine_v3-SI.i2c_pullup

## 191. RISK-191
- **risk_id**: RISK-191
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 A_I2C1_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN32']
- **status**: open
- **evidence_id**: EVID-191-rule_engine_v3-SI.i2c_pullup

## 192. RISK-192
- **risk_id**: RISK-192
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 A_I2C2_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN32']
- **status**: open
- **evidence_id**: EVID-192-rule_engine_v3-SI.i2c_pullup

## 193. RISK-193
- **risk_id**: RISK-193
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 D_I2C1_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN14', 'RN15']
- **status**: open
- **evidence_id**: EVID-193-rule_engine_v3-SI.i2c_pullup

## 194. RISK-194
- **risk_id**: RISK-194
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 H_I2C1_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN36', 'RN41']
- **status**: open
- **evidence_id**: EVID-194-rule_engine_v3-SI.i2c_pullup

## 195. RISK-195
- **risk_id**: RISK-195
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 D_I2C1_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN14', 'RN15']
- **status**: open
- **evidence_id**: EVID-195-rule_engine_v3-SI.i2c_pullup

## 196. RISK-196
- **risk_id**: RISK-196
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 H_I2C1_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN36', 'RN41']
- **status**: open
- **evidence_id**: EVID-196-rule_engine_v3-SI.i2c_pullup

## 197. RISK-197
- **risk_id**: RISK-197
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 B_I2C1_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN38']
- **status**: open
- **evidence_id**: EVID-197-rule_engine_v3-SI.i2c_pullup

## 198. RISK-198
- **risk_id**: RISK-198
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 A_I2C1_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN32']
- **status**: open
- **evidence_id**: EVID-198-rule_engine_v3-SI.i2c_pullup

## 199. RISK-199
- **risk_id**: RISK-199
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 C_I2C2_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN33', 'RN34']
- **status**: open
- **evidence_id**: EVID-199-rule_engine_v3-SI.i2c_pullup

## 200. RISK-200
- **risk_id**: RISK-200
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 G_I2C2_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN30']
- **status**: open
- **evidence_id**: EVID-200-rule_engine_v3-SI.i2c_pullup

## 201. RISK-201
- **risk_id**: RISK-201
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 C_I2C2_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN33', 'RN34']
- **status**: open
- **evidence_id**: EVID-201-rule_engine_v3-SI.i2c_pullup

## 202. RISK-202
- **risk_id**: RISK-202
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 D_I2C2_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN15']
- **status**: open
- **evidence_id**: EVID-202-rule_engine_v3-SI.i2c_pullup

## 203. RISK-203
- **risk_id**: RISK-203
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 E_I2C1_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN31']
- **status**: open
- **evidence_id**: EVID-203-rule_engine_v3-SI.i2c_pullup

## 204. RISK-204
- **risk_id**: RISK-204
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 F_I2C1_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN18']
- **status**: open
- **evidence_id**: EVID-204-rule_engine_v3-SI.i2c_pullup

## 205. RISK-205
- **risk_id**: RISK-205
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 F_I2C2_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN18']
- **status**: open
- **evidence_id**: EVID-205-rule_engine_v3-SI.i2c_pullup

## 206. RISK-206
- **risk_id**: RISK-206
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 F_I2C2_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN18']
- **status**: open
- **evidence_id**: EVID-206-rule_engine_v3-SI.i2c_pullup

## 207. RISK-207
- **risk_id**: RISK-207
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 G_I2C1_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN30']
- **status**: open
- **evidence_id**: EVID-207-rule_engine_v3-SI.i2c_pullup

## 208. RISK-208
- **risk_id**: RISK-208
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 B_I2C2_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN38']
- **status**: open
- **evidence_id**: EVID-208-rule_engine_v3-SI.i2c_pullup

## 209. RISK-209
- **risk_id**: RISK-209
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 E_I2C2_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN31']
- **status**: open
- **evidence_id**: EVID-209-rule_engine_v3-SI.i2c_pullup

## 210. RISK-210
- **risk_id**: RISK-210
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 B_I2C2_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN38']
- **status**: open
- **evidence_id**: EVID-210-rule_engine_v3-SI.i2c_pullup

## 211. RISK-211
- **risk_id**: RISK-211
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 B_I2C2_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN37', 'RN38']
- **status**: open
- **evidence_id**: EVID-211-rule_engine_v3-SI.i2c_pullup

## 212. RISK-212
- **risk_id**: RISK-212
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 C_I2C2_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN33']
- **status**: open
- **evidence_id**: EVID-212-rule_engine_v3-SI.i2c_pullup

## 213. RISK-213
- **risk_id**: RISK-213
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 B_I2C2_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN37', 'RN38']
- **status**: open
- **evidence_id**: EVID-213-rule_engine_v3-SI.i2c_pullup

## 214. RISK-214
- **risk_id**: RISK-214
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 E_I2C2_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN31']
- **status**: open
- **evidence_id**: EVID-214-rule_engine_v3-SI.i2c_pullup

## 215. RISK-215
- **risk_id**: RISK-215
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 E_I2C1_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN31']
- **status**: open
- **evidence_id**: EVID-215-rule_engine_v3-SI.i2c_pullup

## 216. RISK-216
- **risk_id**: RISK-216
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 D_I2C2_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN14', 'RN15']
- **status**: open
- **evidence_id**: EVID-216-rule_engine_v3-SI.i2c_pullup

## 217. RISK-217
- **risk_id**: RISK-217
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 B_I2C1_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN38']
- **status**: open
- **evidence_id**: EVID-217-rule_engine_v3-SI.i2c_pullup

## 218. RISK-218
- **risk_id**: RISK-218
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 D_I2C2_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN14', 'RN15']
- **status**: open
- **evidence_id**: EVID-218-rule_engine_v3-SI.i2c_pullup

## 219. RISK-219
- **risk_id**: RISK-219
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 E_I2C2_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN31', 'RN35']
- **status**: open
- **evidence_id**: EVID-219-rule_engine_v3-SI.i2c_pullup

## 220. RISK-220
- **risk_id**: RISK-220
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 E_I2C2_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN31', 'RN35']
- **status**: open
- **evidence_id**: EVID-220-rule_engine_v3-SI.i2c_pullup

## 221. RISK-221
- **risk_id**: RISK-221
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 G_I2C2_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN30', 'RN4']
- **status**: open
- **evidence_id**: EVID-221-rule_engine_v3-SI.i2c_pullup

## 222. RISK-222
- **risk_id**: RISK-222
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 G_I2C2_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN30', 'RN4']
- **status**: open
- **evidence_id**: EVID-222-rule_engine_v3-SI.i2c_pullup

## 223. RISK-223
- **risk_id**: RISK-223
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 C_I2C2_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN33']
- **status**: open
- **evidence_id**: EVID-223-rule_engine_v3-SI.i2c_pullup

## 224. RISK-224
- **risk_id**: RISK-224
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 C_I2C1_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN33']
- **status**: open
- **evidence_id**: EVID-224-rule_engine_v3-SI.i2c_pullup

## 225. RISK-225
- **risk_id**: RISK-225
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 QSFP_SDA: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN44']
- **status**: open
- **evidence_id**: EVID-225-rule_engine_v3-SI.i2c_pullup

## 226. RISK-226
- **risk_id**: RISK-226
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 QSFP_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN44']
- **status**: open
- **evidence_id**: EVID-226-rule_engine_v3-SI.i2c_pullup

## 227. RISK-227
- **risk_id**: RISK-227
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 D_I2C2_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN15']
- **status**: open
- **evidence_id**: EVID-227-rule_engine_v3-SI.i2c_pullup

## 228. RISK-228
- **risk_id**: RISK-228
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 C_I2C1_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN33']
- **status**: open
- **evidence_id**: EVID-228-rule_engine_v3-SI.i2c_pullup

## 229. RISK-229
- **risk_id**: RISK-229
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 D_I2C1_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN15']
- **status**: open
- **evidence_id**: EVID-229-rule_engine_v3-SI.i2c_pullup

## 230. RISK-230
- **risk_id**: RISK-230
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 D_I2C1_SCL_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN15']
- **status**: open
- **evidence_id**: EVID-230-rule_engine_v3-SI.i2c_pullup

## 231. RISK-231
- **risk_id**: RISK-231
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 A_I2C2_SDA_: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN32']
- **status**: open
- **evidence_id**: EVID-231-rule_engine_v3-SI.i2c_pullup

## 232. RISK-232
- **risk_id**: RISK-232
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 A_I2C1_SCL: 未检测到上拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 网络上的器件: ['RN32', 'RN5']
- **status**: open
- **evidence_id**: EVID-232-rule_engine_v3-SI.i2c_pullup

## 233. RISK-233
- **risk_id**: RISK-233
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 /CLK_DIVIDE_RST_: 无上拉/下拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-233-rule_engine_v3-SI.reset_bias

## 234. RISK-234
- **risk_id**: RISK-234
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 PMUBOARD_RST1_: 无上拉/下拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-234-rule_engine_v3-SI.reset_bias

## 235. RISK-235
- **risk_id**: RISK-235
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 PMUBOARD_RST2_: 无上拉/下拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-235-rule_engine_v3-SI.reset_bias

## 236. RISK-236
- **risk_id**: RISK-236
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 WD_POW_RESET: 无上拉/下拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-236-rule_engine_v3-SI.reset_bias

## 237. RISK-237
- **risk_id**: RISK-237
- **severity**: WARNING
- **priority**: P1
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 QSFP_RESETL_: 无上拉/下拉电阻
- **impact**: SI 类中风险，可能增加调试成本或量产不确定性。
- **mitigation**: 评估修复成本和风险接受条件，必要时更新原理图后复审。
- **status**: open
- **evidence_id**: EVID-237-rule_engine_v3-SI.reset_bias

## 238. RISK-238
- **risk_id**: RISK-238
- **severity**: INFO
- **priority**: P2
- **category**: CONSTRAINT
- **source**: constraint_checker
- **description**: 未找到可检查的设计约束，约束冲突检查已跳过。提供 requirements.yaml 或 pipeline_result.design_constraints 后会启用。
- **impact**: CONSTRAINT 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-238-constraint_checker-CONSTRAINT-NO-INPUT

## 239. RISK-239
- **risk_id**: RISK-239
- **severity**: INFO
- **priority**: P2
- **category**: EMC
- **source**: emc_checker
- **description**: 未找到 requirements.yaml，跳过 EMC 预评估
- **impact**: EMC 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-239-emc_checker-EMC-NO-REQ

## 240. RISK-240
- **risk_id**: RISK-240
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R176: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-240-rule_engine_v3-COMP.abnormal_values

## 241. RISK-241
- **risk_id**: RISK-241
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R310: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-241-rule_engine_v3-COMP.abnormal_values

## 242. RISK-242
- **risk_id**: RISK-242
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R222: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-242-rule_engine_v3-COMP.abnormal_values

## 243. RISK-243
- **risk_id**: RISK-243
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R236: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-243-rule_engine_v3-COMP.abnormal_values

## 244. RISK-244
- **risk_id**: RISK-244
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R234: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-244-rule_engine_v3-COMP.abnormal_values

## 245. RISK-245
- **risk_id**: RISK-245
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R229: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-245-rule_engine_v3-COMP.abnormal_values

## 246. RISK-246
- **risk_id**: RISK-246
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R248: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-246-rule_engine_v3-COMP.abnormal_values

## 247. RISK-247
- **risk_id**: RISK-247
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R240: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-247-rule_engine_v3-COMP.abnormal_values

## 248. RISK-248
- **risk_id**: RISK-248
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R200: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-248-rule_engine_v3-COMP.abnormal_values

## 249. RISK-249
- **risk_id**: RISK-249
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R209: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-249-rule_engine_v3-COMP.abnormal_values

## 250. RISK-250
- **risk_id**: RISK-250
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R221: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-250-rule_engine_v3-COMP.abnormal_values

## 251. RISK-251
- **risk_id**: RISK-251
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R213: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-251-rule_engine_v3-COMP.abnormal_values

## 252. RISK-252
- **risk_id**: RISK-252
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R48: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-252-rule_engine_v3-COMP.abnormal_values

## 253. RISK-253
- **risk_id**: RISK-253
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R46: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-253-rule_engine_v3-COMP.abnormal_values

## 254. RISK-254
- **risk_id**: RISK-254
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R47: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-254-rule_engine_v3-COMP.abnormal_values

## 255. RISK-255
- **risk_id**: RISK-255
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R178: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-255-rule_engine_v3-COMP.abnormal_values

## 256. RISK-256
- **risk_id**: RISK-256
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R183: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-256-rule_engine_v3-COMP.abnormal_values

## 257. RISK-257
- **risk_id**: RISK-257
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R56: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-257-rule_engine_v3-COMP.abnormal_values

## 258. RISK-258
- **risk_id**: RISK-258
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: R55: 0R 电阻在电源路径上（确认是否为设计意图）
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-258-rule_engine_v3-COMP.abnormal_values

## 259. RISK-259
- **risk_id**: RISK-259
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: BOM 与网表 Refdes 完全一致
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-259-rule_engine_v3-COMP.bom_netlist_coverage

## 260. RISK-260
- **risk_id**: RISK-260
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: BOM Value/Description 一致性良好
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-260-rule_engine_v3-COMP.bom_value_consistency

## 261. RISK-261
- **risk_id**: RISK-261
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: 物料封装一致，无需整合
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-261-rule_engine_v3-COMP.consolidation

## 262. RISK-262
- **risk_id**: RISK-262
- **severity**: INFO
- **priority**: P2
- **category**: COMP
- **source**: rule_engine_v3
- **description**: 封装一致性良好
- **impact**: COMP 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-262-rule_engine_v3-COMP.package_consistency

## 263. RISK-263
- **risk_id**: RISK-263
- **severity**: INFO
- **priority**: P2
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 无悬空网络
- **impact**: CONN 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-263-rule_engine_v3-CONN.dangling_nets

## 264. RISK-264
- **risk_id**: RISK-264
- **severity**: INFO
- **priority**: P2
- **category**: CONN
- **source**: rule_engine_v3
- **description**: 无单引脚网络
- **impact**: CONN 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-264-rule_engine_v3-CONN.single_pin_nets

## 265. RISK-265
- **risk_id**: RISK-265
- **severity**: INFO
- **priority**: P2
- **category**: CONST
- **source**: rule_engine_v3
- **description**: 电容降额检查通过
- **impact**: CONST 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-265-rule_engine_v3-CONST.cap_derating

## 266. RISK-266
- **risk_id**: RISK-266
- **severity**: INFO
- **priority**: P2
- **category**: CONST
- **source**: rule_engine_v3
- **description**: 协议合规检查通过
- **impact**: CONST 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-266-rule_engine_v3-CONST.protocol_compliance

## 267. RISK-267
- **risk_id**: RISK-267
- **severity**: INFO
- **priority**: P2
- **category**: CONST
- **source**: rule_engine_v3
- **description**: VIN 绝对最大值检查通过
- **impact**: CONST 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-267-rule_engine_v3-CONST.voltage_abs_max

## 268. RISK-268
- **risk_id**: RISK-268
- **severity**: INFO
- **priority**: P2
- **category**: CONST
- **source**: rule_engine_v3
- **description**: 未找到 VCC/VCCIO 电源网络
- **impact**: CONST 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-268-rule_engine_v3-CONST.voltage_ripple

## 269. RISK-269
- **risk_id**: RISK-269
- **severity**: INFO
- **priority**: P2
- **category**: DRC
- **source**: rule_engine_v3
- **description**: 未找到 DRC 文件，跳过交叉引用检查
- **impact**: DRC 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-269-rule_engine_v3-DRC.drc_cross_reference

## 270. RISK-270
- **risk_id**: RISK-270
- **severity**: INFO
- **priority**: P2
- **category**: DRC
- **source**: rule_engine_v3
- **description**: 未找到 DRC 文件，跳过 DRC 检查
- **impact**: DRC 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-270-rule_engine_v3-DRC.drc_summary

## 271. RISK-271
- **risk_id**: RISK-271
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-271-rule_engine_v3-FPGA.bank_voltage

## 272. RISK-272
- **risk_id**: RISK-272
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-272-rule_engine_v3-FPGA.cfgbvs

## 273. RISK-273
- **risk_id**: RISK-273
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-273-rule_engine_v3-FPGA.config_design_guide

## 274. RISK-274
- **risk_id**: RISK-274
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-274-rule_engine_v3-FPGA.design_guide_clocking

## 275. RISK-275
- **risk_id**: RISK-275
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-275-rule_engine_v3-FPGA.design_guide_io_signaling

## 276. RISK-276
- **risk_id**: RISK-276
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-276-rule_engine_v3-FPGA.design_guide_power_integrity

## 277. RISK-277
- **risk_id**: RISK-277
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-277-rule_engine_v3-FPGA.done_pullup

## 278. RISK-278
- **risk_id**: RISK-278
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-278-rule_engine_v3-FPGA.mode_strap

## 279. RISK-279
- **risk_id**: RISK-279
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-279-rule_engine_v3-FPGA.pudc_static

## 280. RISK-280
- **risk_id**: RISK-280
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-280-rule_engine_v3-FPGA.reconfig_n_bias

## 281. RISK-281
- **risk_id**: RISK-281
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-281-rule_engine_v3-FPGA.serdes_ac_coupling

## 282. RISK-282
- **risk_id**: RISK-282
- **severity**: INFO
- **priority**: P2
- **category**: FPGA
- **source**: rule_engine_v3
- **description**: 未发现 FPGA 器件
- **impact**: FPGA 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-282-rule_engine_v3-FPGA.sspi_pin_swap

## 283. RISK-283
- **risk_id**: RISK-283
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: 电容耐压降额检查通过
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-283-rule_engine_v3-PI.cap_voltage_derating

## 284. RISK-284
- **risk_id**: RISK-284
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: 未发现 SerDes/MIPI 电源网络
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-284-rule_engine_v3-PI.ferrite_isolation

## 285. RISK-285
- **risk_id**: RISK-285
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R176: 0R 电阻在电源路径上 (M1V8 ↔ VCCAUX)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-285-rule_engine_v3-PI.zero_ohm_on_power

## 286. RISK-286
- **risk_id**: RISK-286
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R310: 0R 电阻在电源路径上 (M1V8 ↔ VCCAUX)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-286-rule_engine_v3-PI.zero_ohm_on_power

## 287. RISK-287
- **risk_id**: RISK-287
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R222: 0R 电阻在电源路径上 (5V ↔ M5V)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-287-rule_engine_v3-PI.zero_ohm_on_power

## 288. RISK-288
- **risk_id**: RISK-288
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R236: 0R 电阻在电源路径上 (5V ↔ M5V)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-288-rule_engine_v3-PI.zero_ohm_on_power

## 289. RISK-289
- **risk_id**: RISK-289
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R234: 0R 电阻在电源路径上 (5V ↔ M5V)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-289-rule_engine_v3-PI.zero_ohm_on_power

## 290. RISK-290
- **risk_id**: RISK-290
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R229: 0R 电阻在电源路径上 (5V ↔ M5V)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-290-rule_engine_v3-PI.zero_ohm_on_power

## 291. RISK-291
- **risk_id**: RISK-291
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R248: 0R 电阻在电源路径上 (DDR4_VDD ↔ M1V2)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-291-rule_engine_v3-PI.zero_ohm_on_power

## 292. RISK-292
- **risk_id**: RISK-292
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R240: 0R 电阻在电源路径上 (DDR4_VDD ↔ M1V2)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-292-rule_engine_v3-PI.zero_ohm_on_power

## 293. RISK-293
- **risk_id**: RISK-293
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R200: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-293-rule_engine_v3-PI.zero_ohm_on_power

## 294. RISK-294
- **risk_id**: RISK-294
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R209: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-294-rule_engine_v3-PI.zero_ohm_on_power

## 295. RISK-295
- **risk_id**: RISK-295
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R221: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-295-rule_engine_v3-PI.zero_ohm_on_power

## 296. RISK-296
- **risk_id**: RISK-296
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R213: 0R 电阻在电源路径上 (M0V95 ↔ VCCINT)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-296-rule_engine_v3-PI.zero_ohm_on_power

## 297. RISK-297
- **risk_id**: RISK-297
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R48: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-297-rule_engine_v3-PI.zero_ohm_on_power

## 298. RISK-298
- **risk_id**: RISK-298
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R46: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-298-rule_engine_v3-PI.zero_ohm_on_power

## 299. RISK-299
- **risk_id**: RISK-299
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R47: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-299-rule_engine_v3-PI.zero_ohm_on_power

## 300. RISK-300
- **risk_id**: RISK-300
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R178: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-300-rule_engine_v3-PI.zero_ohm_on_power

## 301. RISK-301
- **risk_id**: RISK-301
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R183: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_R)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-301-rule_engine_v3-PI.zero_ohm_on_power

## 302. RISK-302
- **risk_id**: RISK-302
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R56: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_L)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-302-rule_engine_v3-PI.zero_ohm_on_power

## 303. RISK-303
- **risk_id**: RISK-303
- **severity**: INFO
- **priority**: P2
- **category**: PI
- **source**: rule_engine_v3
- **description**: R55: 0R 电阻在电源路径上 (M1V0 ↔ MGTAVCC_L)
- **impact**: PI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 确认是否为设计意图，大电流场景需评估压降
- **status**: open
- **evidence_id**: EVID-303-rule_engine_v3-PI.zero_ohm_on_power

## 304. RISK-304
- **risk_id**: RISK-304
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 发现 112 对确认差分对, 72 对疑似
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-304-rule_engine_v3-SI.diff_pair_symmetry

## 305. RISK-305
- **risk_id**: RISK-305
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 DDR4_CLK_P/DDR4_CLK_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-305-rule_engine_v3-SI.diff_pair_symmetry

## 306. RISK-306
- **risk_id**: RISK-306
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 DDR4_DQS_P0/DDR4_DQS_N0 (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-306-rule_engine_v3-SI.diff_pair_symmetry

## 307. RISK-307
- **risk_id**: RISK-307
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 DDR4_DQS_P1/DDR4_DQS_N1 (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-307-rule_engine_v3-SI.diff_pair_symmetry

## 308. RISK-308
- **risk_id**: RISK-308
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 DDR4_DQS_P2/DDR4_DQS_N2 (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-308-rule_engine_v3-SI.diff_pair_symmetry

## 309. RISK-309
- **risk_id**: RISK-309
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 DDR4_DQS_P3/DDR4_DQS_N3 (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-309-rule_engine_v3-SI.diff_pair_symmetry

## 310. RISK-310
- **risk_id**: RISK-310
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 DDR4_DQS_P4/DDR4_DQS_N4 (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-310-rule_engine_v3-SI.diff_pair_symmetry

## 311. RISK-311
- **risk_id**: RISK-311
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 DDR4_DQS_P5/DDR4_DQS_N5 (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-311-rule_engine_v3-SI.diff_pair_symmetry

## 312. RISK-312
- **risk_id**: RISK-312
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 DDR4_DQS_P6/DDR4_DQS_N6 (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-312-rule_engine_v3-SI.diff_pair_symmetry

## 313. RISK-313
- **risk_id**: RISK-313
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 DDR4_DQS_P7/DDR4_DQS_N7 (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-313-rule_engine_v3-SI.diff_pair_symmetry

## 314. RISK-314
- **risk_id**: RISK-314
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 DDR4_VREF_CLK_P/DDR4_VREF_CLK_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-314-rule_engine_v3-SI.diff_pair_symmetry

## 315. RISK-315
- **risk_id**: RISK-315
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MA_BF_D_CLK_HS_P/MA_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-315-rule_engine_v3-SI.diff_pair_symmetry

## 316. RISK-316
- **risk_id**: RISK-316
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MA_BF_D_D0_HS_P/MA_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-316-rule_engine_v3-SI.diff_pair_symmetry

## 317. RISK-317
- **risk_id**: RISK-317
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MA_BF_D_D1_HS_P/MA_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-317-rule_engine_v3-SI.diff_pair_symmetry

## 318. RISK-318
- **risk_id**: RISK-318
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MA_BF_D_D2_HS_P/MA_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-318-rule_engine_v3-SI.diff_pair_symmetry

## 319. RISK-319
- **risk_id**: RISK-319
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MA_BF_D_D3_HS_P/MA_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-319-rule_engine_v3-SI.diff_pair_symmetry

## 320. RISK-320
- **risk_id**: RISK-320
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MB_BF_D_CLK_HS_P/MB_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-320-rule_engine_v3-SI.diff_pair_symmetry

## 321. RISK-321
- **risk_id**: RISK-321
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MB_BF_D_D0_HS_P/MB_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-321-rule_engine_v3-SI.diff_pair_symmetry

## 322. RISK-322
- **risk_id**: RISK-322
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MB_BF_D_D1_HS_P/MB_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-322-rule_engine_v3-SI.diff_pair_symmetry

## 323. RISK-323
- **risk_id**: RISK-323
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MB_BF_D_D2_HS_P/MB_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-323-rule_engine_v3-SI.diff_pair_symmetry

## 324. RISK-324
- **risk_id**: RISK-324
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MB_BF_D_D3_HS_P/MB_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-324-rule_engine_v3-SI.diff_pair_symmetry

## 325. RISK-325
- **risk_id**: RISK-325
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MC_BF_D_CLK_HS_P/MC_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-325-rule_engine_v3-SI.diff_pair_symmetry

## 326. RISK-326
- **risk_id**: RISK-326
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MC_BF_D_D0_HS_P/MC_BF_D_D0_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-326-rule_engine_v3-SI.diff_pair_symmetry

## 327. RISK-327
- **risk_id**: RISK-327
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MC_BF_D_D1_HS_P/MC_BF_D_D1_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-327-rule_engine_v3-SI.diff_pair_symmetry

## 328. RISK-328
- **risk_id**: RISK-328
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MC_BF_D_D2_HS_P/MC_BF_D_D2_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-328-rule_engine_v3-SI.diff_pair_symmetry

## 329. RISK-329
- **risk_id**: RISK-329
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MC_BF_D_D3_HS_P/MC_BF_D_D3_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-329-rule_engine_v3-SI.diff_pair_symmetry

## 330. RISK-330
- **risk_id**: RISK-330
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MD_BF_D_CLK_HS_P/MD_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-330-rule_engine_v3-SI.diff_pair_symmetry

## 331. RISK-331
- **risk_id**: RISK-331
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MD_BF_D_D0_HS_P/MD_BF_D_D0_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-331-rule_engine_v3-SI.diff_pair_symmetry

## 332. RISK-332
- **risk_id**: RISK-332
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MD_BF_D_D1_HS_P/MD_BF_D_D1_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-332-rule_engine_v3-SI.diff_pair_symmetry

## 333. RISK-333
- **risk_id**: RISK-333
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MD_BF_D_D2_HS_P/MD_BF_D_D2_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-333-rule_engine_v3-SI.diff_pair_symmetry

## 334. RISK-334
- **risk_id**: RISK-334
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MD_BF_D_D3_HS_P/MD_BF_D_D3_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-334-rule_engine_v3-SI.diff_pair_symmetry

## 335. RISK-335
- **risk_id**: RISK-335
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_BF_D_CLK_HS_P/ME_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-335-rule_engine_v3-SI.diff_pair_symmetry

## 336. RISK-336
- **risk_id**: RISK-336
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_BF_D_D0_HS_P/ME_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-336-rule_engine_v3-SI.diff_pair_symmetry

## 337. RISK-337
- **risk_id**: RISK-337
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_BF_D_D1_HS_P/ME_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-337-rule_engine_v3-SI.diff_pair_symmetry

## 338. RISK-338
- **risk_id**: RISK-338
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_BF_D_D2_HS_P/ME_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-338-rule_engine_v3-SI.diff_pair_symmetry

## 339. RISK-339
- **risk_id**: RISK-339
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_BF_D_D3_HS_P/ME_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-339-rule_engine_v3-SI.diff_pair_symmetry

## 340. RISK-340
- **risk_id**: RISK-340
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_DIVIDE_CLK_HS_P/ME_DIVIDE_CLK_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-340-rule_engine_v3-SI.diff_pair_symmetry

## 341. RISK-341
- **risk_id**: RISK-341
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_D_CLK_HS_P/ME_D_CLK_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-341-rule_engine_v3-SI.diff_pair_symmetry

## 342. RISK-342
- **risk_id**: RISK-342
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_D_D0_HS_P/ME_D_D0_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-342-rule_engine_v3-SI.diff_pair_symmetry

## 343. RISK-343
- **risk_id**: RISK-343
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_D_D1_HS_P/ME_D_D1_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-343-rule_engine_v3-SI.diff_pair_symmetry

## 344. RISK-344
- **risk_id**: RISK-344
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_D_D2_HS_P/ME_D_D2_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-344-rule_engine_v3-SI.diff_pair_symmetry

## 345. RISK-345
- **risk_id**: RISK-345
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_D_D3_HS_P/ME_D_D3_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-345-rule_engine_v3-SI.diff_pair_symmetry

## 346. RISK-346
- **risk_id**: RISK-346
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_SERDES_CLK_HS_P/ME_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-346-rule_engine_v3-SI.diff_pair_symmetry

## 347. RISK-347
- **risk_id**: RISK-347
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_SERDES_D0_HS_P/ME_SERDES_D0_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-347-rule_engine_v3-SI.diff_pair_symmetry

## 348. RISK-348
- **risk_id**: RISK-348
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_SERDES_D1_HS_P/ME_SERDES_D1_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-348-rule_engine_v3-SI.diff_pair_symmetry

## 349. RISK-349
- **risk_id**: RISK-349
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_SERDES_D2_HS_P/ME_SERDES_D2_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-349-rule_engine_v3-SI.diff_pair_symmetry

## 350. RISK-350
- **risk_id**: RISK-350
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 ME_SERDES_D3_HS_P/ME_SERDES_D3_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-350-rule_engine_v3-SI.diff_pair_symmetry

## 351. RISK-351
- **risk_id**: RISK-351
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_BF_D_CLK_HS_P/MF_BF_D_CLK_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-351-rule_engine_v3-SI.diff_pair_symmetry

## 352. RISK-352
- **risk_id**: RISK-352
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_BF_D_D0_HS_P/MF_BF_D_D0_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-352-rule_engine_v3-SI.diff_pair_symmetry

## 353. RISK-353
- **risk_id**: RISK-353
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_BF_D_D1_HS_P/MF_BF_D_D1_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-353-rule_engine_v3-SI.diff_pair_symmetry

## 354. RISK-354
- **risk_id**: RISK-354
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_BF_D_D2_HS_P/MF_BF_D_D2_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-354-rule_engine_v3-SI.diff_pair_symmetry

## 355. RISK-355
- **risk_id**: RISK-355
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_BF_D_D3_HS_P/MF_BF_D_D3_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-355-rule_engine_v3-SI.diff_pair_symmetry

## 356. RISK-356
- **risk_id**: RISK-356
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_DIVIDE_CLK_HS_P/MF_DIVIDE_CLK_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-356-rule_engine_v3-SI.diff_pair_symmetry

## 357. RISK-357
- **risk_id**: RISK-357
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_D_CLK_HS_P/MF_D_CLK_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-357-rule_engine_v3-SI.diff_pair_symmetry

## 358. RISK-358
- **risk_id**: RISK-358
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_D_D0_HS_P/MF_D_D0_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-358-rule_engine_v3-SI.diff_pair_symmetry

## 359. RISK-359
- **risk_id**: RISK-359
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_D_D1_HS_P/MF_D_D1_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-359-rule_engine_v3-SI.diff_pair_symmetry

## 360. RISK-360
- **risk_id**: RISK-360
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_D_D2_HS_P/MF_D_D2_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-360-rule_engine_v3-SI.diff_pair_symmetry

## 361. RISK-361
- **risk_id**: RISK-361
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_D_D3_HS_P/MF_D_D3_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-361-rule_engine_v3-SI.diff_pair_symmetry

## 362. RISK-362
- **risk_id**: RISK-362
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_SERDES_CLK_HS_P/MF_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-362-rule_engine_v3-SI.diff_pair_symmetry

## 363. RISK-363
- **risk_id**: RISK-363
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_SERDES_D0_HS_P/MF_SERDES_D0_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-363-rule_engine_v3-SI.diff_pair_symmetry

## 364. RISK-364
- **risk_id**: RISK-364
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_SERDES_D1_HS_P/MF_SERDES_D1_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-364-rule_engine_v3-SI.diff_pair_symmetry

## 365. RISK-365
- **risk_id**: RISK-365
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_SERDES_D2_HS_P/MF_SERDES_D2_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-365-rule_engine_v3-SI.diff_pair_symmetry

## 366. RISK-366
- **risk_id**: RISK-366
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MF_SERDES_D3_HS_P/MF_SERDES_D3_HS_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-366-rule_engine_v3-SI.diff_pair_symmetry

## 367. RISK-367
- **risk_id**: RISK-367
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_BF_D_CLK_HS_P/MG_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-367-rule_engine_v3-SI.diff_pair_symmetry

## 368. RISK-368
- **risk_id**: RISK-368
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_BF_D_D0_HS_P/MG_BF_D_D0_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-368-rule_engine_v3-SI.diff_pair_symmetry

## 369. RISK-369
- **risk_id**: RISK-369
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_BF_D_D1_HS_P/MG_BF_D_D1_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-369-rule_engine_v3-SI.diff_pair_symmetry

## 370. RISK-370
- **risk_id**: RISK-370
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_BF_D_D2_HS_P/MG_BF_D_D2_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-370-rule_engine_v3-SI.diff_pair_symmetry

## 371. RISK-371
- **risk_id**: RISK-371
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_BF_D_D3_HS_P/MG_BF_D_D3_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-371-rule_engine_v3-SI.diff_pair_symmetry

## 372. RISK-372
- **risk_id**: RISK-372
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_DIVIDE_CLK_HS_P/MG_DIVIDE_CLK_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-372-rule_engine_v3-SI.diff_pair_symmetry

## 373. RISK-373
- **risk_id**: RISK-373
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_D_CLK_HS_P/MG_D_CLK_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-373-rule_engine_v3-SI.diff_pair_symmetry

## 374. RISK-374
- **risk_id**: RISK-374
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_D_D0_HS_P/MG_D_D0_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-374-rule_engine_v3-SI.diff_pair_symmetry

## 375. RISK-375
- **risk_id**: RISK-375
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_D_D1_HS_P/MG_D_D1_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-375-rule_engine_v3-SI.diff_pair_symmetry

## 376. RISK-376
- **risk_id**: RISK-376
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_D_D2_HS_P/MG_D_D2_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-376-rule_engine_v3-SI.diff_pair_symmetry

## 377. RISK-377
- **risk_id**: RISK-377
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_D_D3_HS_P/MG_D_D3_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-377-rule_engine_v3-SI.diff_pair_symmetry

## 378. RISK-378
- **risk_id**: RISK-378
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MG_SERDES_CLK_HS_P/MG_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-378-rule_engine_v3-SI.diff_pair_symmetry

## 379. RISK-379
- **risk_id**: RISK-379
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_SERDES_D0_HS_P/MG_SERDES_D0_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-379-rule_engine_v3-SI.diff_pair_symmetry

## 380. RISK-380
- **risk_id**: RISK-380
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_SERDES_D1_HS_P/MG_SERDES_D1_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-380-rule_engine_v3-SI.diff_pair_symmetry

## 381. RISK-381
- **risk_id**: RISK-381
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_SERDES_D2_HS_P/MG_SERDES_D2_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-381-rule_engine_v3-SI.diff_pair_symmetry

## 382. RISK-382
- **risk_id**: RISK-382
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MG_SERDES_D3_HS_P/MG_SERDES_D3_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-382-rule_engine_v3-SI.diff_pair_symmetry

## 383. RISK-383
- **risk_id**: RISK-383
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_BF_D_CLK_HS_P/MH_BF_D_CLK_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-383-rule_engine_v3-SI.diff_pair_symmetry

## 384. RISK-384
- **risk_id**: RISK-384
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_BF_D_D0_HS_P/MH_BF_D_D0_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-384-rule_engine_v3-SI.diff_pair_symmetry

## 385. RISK-385
- **risk_id**: RISK-385
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_BF_D_D1_HS_P/MH_BF_D_D1_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-385-rule_engine_v3-SI.diff_pair_symmetry

## 386. RISK-386
- **risk_id**: RISK-386
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_BF_D_D2_HS_P/MH_BF_D_D2_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-386-rule_engine_v3-SI.diff_pair_symmetry

## 387. RISK-387
- **risk_id**: RISK-387
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_BF_D_D3_HS_P/MH_BF_D_D3_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-387-rule_engine_v3-SI.diff_pair_symmetry

## 388. RISK-388
- **risk_id**: RISK-388
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_DIVIDE_CLK_HS_P/MH_DIVIDE_CLK_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-388-rule_engine_v3-SI.diff_pair_symmetry

## 389. RISK-389
- **risk_id**: RISK-389
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_D_CLK_HS_P/MH_D_CLK_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-389-rule_engine_v3-SI.diff_pair_symmetry

## 390. RISK-390
- **risk_id**: RISK-390
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_D_D0_HS_P/MH_D_D0_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-390-rule_engine_v3-SI.diff_pair_symmetry

## 391. RISK-391
- **risk_id**: RISK-391
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_D_D1_HS_P/MH_D_D1_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-391-rule_engine_v3-SI.diff_pair_symmetry

## 392. RISK-392
- **risk_id**: RISK-392
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_D_D2_HS_P/MH_D_D2_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-392-rule_engine_v3-SI.diff_pair_symmetry

## 393. RISK-393
- **risk_id**: RISK-393
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_D_D3_HS_P/MH_D_D3_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-393-rule_engine_v3-SI.diff_pair_symmetry

## 394. RISK-394
- **risk_id**: RISK-394
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MH_SERDES_CLK_HS_P/MH_SERDES_CLK_HS_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-394-rule_engine_v3-SI.diff_pair_symmetry

## 395. RISK-395
- **risk_id**: RISK-395
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_SERDES_D0_HS_P/MH_SERDES_D0_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-395-rule_engine_v3-SI.diff_pair_symmetry

## 396. RISK-396
- **risk_id**: RISK-396
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_SERDES_D1_HS_P/MH_SERDES_D1_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-396-rule_engine_v3-SI.diff_pair_symmetry

## 397. RISK-397
- **risk_id**: RISK-397
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_SERDES_D2_HS_P/MH_SERDES_D2_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-397-rule_engine_v3-SI.diff_pair_symmetry

## 398. RISK-398
- **risk_id**: RISK-398
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MH_SERDES_D3_HS_P/MH_SERDES_D3_HS_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-398-rule_engine_v3-SI.diff_pair_symmetry

## 399. RISK-399
- **risk_id**: RISK-399
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_CLK_P/MIPIA_CLK_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-399-rule_engine_v3-SI.diff_pair_symmetry

## 400. RISK-400
- **risk_id**: RISK-400
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_D0_P/MIPIA_D0_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-400-rule_engine_v3-SI.diff_pair_symmetry

## 401. RISK-401
- **risk_id**: RISK-401
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_D1_P/MIPIA_D1_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-401-rule_engine_v3-SI.diff_pair_symmetry

## 402. RISK-402
- **risk_id**: RISK-402
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_D2_P/MIPIA_D2_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-402-rule_engine_v3-SI.diff_pair_symmetry

## 403. RISK-403
- **risk_id**: RISK-403
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_D3_P/MIPIA_D3_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-403-rule_engine_v3-SI.diff_pair_symmetry

## 404. RISK-404
- **risk_id**: RISK-404
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_D_D0P_HS/MIPIA_D_D0N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-404-rule_engine_v3-SI.diff_pair_symmetry

## 405. RISK-405
- **risk_id**: RISK-405
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_D_D0P_LP/MIPIA_D_D0N_LP (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-405-rule_engine_v3-SI.diff_pair_symmetry

## 406. RISK-406
- **risk_id**: RISK-406
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_D_D1P_HS/MIPIA_D_D1N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-406-rule_engine_v3-SI.diff_pair_symmetry

## 407. RISK-407
- **risk_id**: RISK-407
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_D_D2P_HS/MIPIA_D_D2N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-407-rule_engine_v3-SI.diff_pair_symmetry

## 408. RISK-408
- **risk_id**: RISK-408
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIA_D_D3P_HS/MIPIA_D_D3N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-408-rule_engine_v3-SI.diff_pair_symmetry

## 409. RISK-409
- **risk_id**: RISK-409
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_CLK_P/MIPIB_CLK_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-409-rule_engine_v3-SI.diff_pair_symmetry

## 410. RISK-410
- **risk_id**: RISK-410
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_D0_P/MIPIB_D0_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-410-rule_engine_v3-SI.diff_pair_symmetry

## 411. RISK-411
- **risk_id**: RISK-411
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_D1_P/MIPIB_D1_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-411-rule_engine_v3-SI.diff_pair_symmetry

## 412. RISK-412
- **risk_id**: RISK-412
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_D2_P/MIPIB_D2_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-412-rule_engine_v3-SI.diff_pair_symmetry

## 413. RISK-413
- **risk_id**: RISK-413
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_D3_P/MIPIB_D3_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-413-rule_engine_v3-SI.diff_pair_symmetry

## 414. RISK-414
- **risk_id**: RISK-414
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_D_D0P_HS/MIPIB_D_D0N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-414-rule_engine_v3-SI.diff_pair_symmetry

## 415. RISK-415
- **risk_id**: RISK-415
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_D_D0P_LP/MIPIB_D_D0N_LP (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-415-rule_engine_v3-SI.diff_pair_symmetry

## 416. RISK-416
- **risk_id**: RISK-416
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_D_D1P_HS/MIPIB_D_D1N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-416-rule_engine_v3-SI.diff_pair_symmetry

## 417. RISK-417
- **risk_id**: RISK-417
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_D_D2P_HS/MIPIB_D_D2N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-417-rule_engine_v3-SI.diff_pair_symmetry

## 418. RISK-418
- **risk_id**: RISK-418
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIB_D_D3P_HS/MIPIB_D_D3N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-418-rule_engine_v3-SI.diff_pair_symmetry

## 419. RISK-419
- **risk_id**: RISK-419
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIC_CLK_P/MIPIC_CLK_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-419-rule_engine_v3-SI.diff_pair_symmetry

## 420. RISK-420
- **risk_id**: RISK-420
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIC_D0_P/MIPIC_D0_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-420-rule_engine_v3-SI.diff_pair_symmetry

## 421. RISK-421
- **risk_id**: RISK-421
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIC_D1_P/MIPIC_D1_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-421-rule_engine_v3-SI.diff_pair_symmetry

## 422. RISK-422
- **risk_id**: RISK-422
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIC_D2_P/MIPIC_D2_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-422-rule_engine_v3-SI.diff_pair_symmetry

## 423. RISK-423
- **risk_id**: RISK-423
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIC_D3_P/MIPIC_D3_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-423-rule_engine_v3-SI.diff_pair_symmetry

## 424. RISK-424
- **risk_id**: RISK-424
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIC_D_D0P_HS/MIPIC_D_D0N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-424-rule_engine_v3-SI.diff_pair_symmetry

## 425. RISK-425
- **risk_id**: RISK-425
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIC_D_D0P_LP/MIPIC_D_D0N_LP (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-425-rule_engine_v3-SI.diff_pair_symmetry

## 426. RISK-426
- **risk_id**: RISK-426
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIC_D_D1P_HS/MIPIC_D_D1N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-426-rule_engine_v3-SI.diff_pair_symmetry

## 427. RISK-427
- **risk_id**: RISK-427
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIC_D_D2P_HS/MIPIC_D_D2N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-427-rule_engine_v3-SI.diff_pair_symmetry

## 428. RISK-428
- **risk_id**: RISK-428
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIC_D_D3P_HS/MIPIC_D_D3N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-428-rule_engine_v3-SI.diff_pair_symmetry

## 429. RISK-429
- **risk_id**: RISK-429
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPID_CLK_P/MIPID_CLK_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-429-rule_engine_v3-SI.diff_pair_symmetry

## 430. RISK-430
- **risk_id**: RISK-430
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPID_D0_P/MIPID_D0_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-430-rule_engine_v3-SI.diff_pair_symmetry

## 431. RISK-431
- **risk_id**: RISK-431
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPID_D1_P/MIPID_D1_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-431-rule_engine_v3-SI.diff_pair_symmetry

## 432. RISK-432
- **risk_id**: RISK-432
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPID_D2_P/MIPID_D2_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-432-rule_engine_v3-SI.diff_pair_symmetry

## 433. RISK-433
- **risk_id**: RISK-433
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPID_D3_P/MIPID_D3_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-433-rule_engine_v3-SI.diff_pair_symmetry

## 434. RISK-434
- **risk_id**: RISK-434
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPID_D_D0P_HS/MIPID_D_D0N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-434-rule_engine_v3-SI.diff_pair_symmetry

## 435. RISK-435
- **risk_id**: RISK-435
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPID_D_D0P_LP/MIPID_D_D0N_LP (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-435-rule_engine_v3-SI.diff_pair_symmetry

## 436. RISK-436
- **risk_id**: RISK-436
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPID_D_D1P_HS/MIPID_D_D1N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-436-rule_engine_v3-SI.diff_pair_symmetry

## 437. RISK-437
- **risk_id**: RISK-437
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPID_D_D2P_HS/MIPID_D_D2N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-437-rule_engine_v3-SI.diff_pair_symmetry

## 438. RISK-438
- **risk_id**: RISK-438
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPID_D_D3P_HS/MIPID_D_D3N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-438-rule_engine_v3-SI.diff_pair_symmetry

## 439. RISK-439
- **risk_id**: RISK-439
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_CLK_P/MIPIE_CLK_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-439-rule_engine_v3-SI.diff_pair_symmetry

## 440. RISK-440
- **risk_id**: RISK-440
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_D0_P/MIPIE_D0_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-440-rule_engine_v3-SI.diff_pair_symmetry

## 441. RISK-441
- **risk_id**: RISK-441
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_D1_P/MIPIE_D1_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-441-rule_engine_v3-SI.diff_pair_symmetry

## 442. RISK-442
- **risk_id**: RISK-442
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_D2_P/MIPIE_D2_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-442-rule_engine_v3-SI.diff_pair_symmetry

## 443. RISK-443
- **risk_id**: RISK-443
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_D3_P/MIPIE_D3_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-443-rule_engine_v3-SI.diff_pair_symmetry

## 444. RISK-444
- **risk_id**: RISK-444
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_D_D0P_HS/MIPIE_D_D0N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-444-rule_engine_v3-SI.diff_pair_symmetry

## 445. RISK-445
- **risk_id**: RISK-445
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_D_D0P_LP/MIPIE_D_D0N_LP (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-445-rule_engine_v3-SI.diff_pair_symmetry

## 446. RISK-446
- **risk_id**: RISK-446
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_D_D1P_HS/MIPIE_D_D1N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-446-rule_engine_v3-SI.diff_pair_symmetry

## 447. RISK-447
- **risk_id**: RISK-447
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_D_D2P_HS/MIPIE_D_D2N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-447-rule_engine_v3-SI.diff_pair_symmetry

## 448. RISK-448
- **risk_id**: RISK-448
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIE_D_D3P_HS/MIPIE_D_D3N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-448-rule_engine_v3-SI.diff_pair_symmetry

## 449. RISK-449
- **risk_id**: RISK-449
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_CLK_P/MIPIF_CLK_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-449-rule_engine_v3-SI.diff_pair_symmetry

## 450. RISK-450
- **risk_id**: RISK-450
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_D0_P/MIPIF_D0_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-450-rule_engine_v3-SI.diff_pair_symmetry

## 451. RISK-451
- **risk_id**: RISK-451
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_D1_P/MIPIF_D1_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-451-rule_engine_v3-SI.diff_pair_symmetry

## 452. RISK-452
- **risk_id**: RISK-452
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_D2_P/MIPIF_D2_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-452-rule_engine_v3-SI.diff_pair_symmetry

## 453. RISK-453
- **risk_id**: RISK-453
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_D3_P/MIPIF_D3_N (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-453-rule_engine_v3-SI.diff_pair_symmetry

## 454. RISK-454
- **risk_id**: RISK-454
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_D_D0P_HS/MIPIF_D_D0N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-454-rule_engine_v3-SI.diff_pair_symmetry

## 455. RISK-455
- **risk_id**: RISK-455
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_D_D0P_LP/MIPIF_D_D0N_LP (置信度90%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-455-rule_engine_v3-SI.diff_pair_symmetry

## 456. RISK-456
- **risk_id**: RISK-456
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_D_D1P_HS/MIPIF_D_D1N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-456-rule_engine_v3-SI.diff_pair_symmetry

## 457. RISK-457
- **risk_id**: RISK-457
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_D_D2P_HS/MIPIF_D_D2N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-457-rule_engine_v3-SI.diff_pair_symmetry

## 458. RISK-458
- **risk_id**: RISK-458
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIF_D_D3P_HS/MIPIF_D_D3N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-458-rule_engine_v3-SI.diff_pair_symmetry

## 459. RISK-459
- **risk_id**: RISK-459
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIG_CLK_P/MIPIG_CLK_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-459-rule_engine_v3-SI.diff_pair_symmetry

## 460. RISK-460
- **risk_id**: RISK-460
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIG_D0_P/MIPIG_D0_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-460-rule_engine_v3-SI.diff_pair_symmetry

## 461. RISK-461
- **risk_id**: RISK-461
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIG_D1_P/MIPIG_D1_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-461-rule_engine_v3-SI.diff_pair_symmetry

## 462. RISK-462
- **risk_id**: RISK-462
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIG_D2_P/MIPIG_D2_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-462-rule_engine_v3-SI.diff_pair_symmetry

## 463. RISK-463
- **risk_id**: RISK-463
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIG_D3_P/MIPIG_D3_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-463-rule_engine_v3-SI.diff_pair_symmetry

## 464. RISK-464
- **risk_id**: RISK-464
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIG_D_D0P_HS/MIPIG_D_D0N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-464-rule_engine_v3-SI.diff_pair_symmetry

## 465. RISK-465
- **risk_id**: RISK-465
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIG_D_D0P_LP/MIPIG_D_D0N_LP (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-465-rule_engine_v3-SI.diff_pair_symmetry

## 466. RISK-466
- **risk_id**: RISK-466
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIG_D_D1P_HS/MIPIG_D_D1N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-466-rule_engine_v3-SI.diff_pair_symmetry

## 467. RISK-467
- **risk_id**: RISK-467
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIG_D_D2P_HS/MIPIG_D_D2N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-467-rule_engine_v3-SI.diff_pair_symmetry

## 468. RISK-468
- **risk_id**: RISK-468
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIG_D_D3P_HS/MIPIG_D_D3N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-468-rule_engine_v3-SI.diff_pair_symmetry

## 469. RISK-469
- **risk_id**: RISK-469
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIH_CLK_P/MIPIH_CLK_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-469-rule_engine_v3-SI.diff_pair_symmetry

## 470. RISK-470
- **risk_id**: RISK-470
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIH_D0_P/MIPIH_D0_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-470-rule_engine_v3-SI.diff_pair_symmetry

## 471. RISK-471
- **risk_id**: RISK-471
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIH_D1_P/MIPIH_D1_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-471-rule_engine_v3-SI.diff_pair_symmetry

## 472. RISK-472
- **risk_id**: RISK-472
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIH_D2_P/MIPIH_D2_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-472-rule_engine_v3-SI.diff_pair_symmetry

## 473. RISK-473
- **risk_id**: RISK-473
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIH_D3_P/MIPIH_D3_N (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-473-rule_engine_v3-SI.diff_pair_symmetry

## 474. RISK-474
- **risk_id**: RISK-474
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIH_D_D0P_HS/MIPIH_D_D0N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-474-rule_engine_v3-SI.diff_pair_symmetry

## 475. RISK-475
- **risk_id**: RISK-475
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 疑似差分对 MIPIH_D_D0P_LP/MIPIH_D_D0N_LP (置信度50%): 请人工确认
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-475-rule_engine_v3-SI.diff_pair_symmetry

## 476. RISK-476
- **risk_id**: RISK-476
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIH_D_D1P_HS/MIPIH_D_D1N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-476-rule_engine_v3-SI.diff_pair_symmetry

## 477. RISK-477
- **risk_id**: RISK-477
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIH_D_D2P_HS/MIPIH_D_D2N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-477-rule_engine_v3-SI.diff_pair_symmetry

## 478. RISK-478
- **risk_id**: RISK-478
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 MIPIH_D_D3P_HS/MIPIH_D_D3N_HS (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-478-rule_engine_v3-SI.diff_pair_symmetry

## 479. RISK-479
- **risk_id**: RISK-479
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 OSC_MIPI_VREF_CLK_P/OSC_MIPI_VREF_CLK_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-479-rule_engine_v3-SI.diff_pair_symmetry

## 480. RISK-480
- **risk_id**: RISK-480
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 SFP0_RX_P/SFP0_RX_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-480-rule_engine_v3-SI.diff_pair_symmetry

## 481. RISK-481
- **risk_id**: RISK-481
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 SFP0_TX_P/SFP0_TX_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-481-rule_engine_v3-SI.diff_pair_symmetry

## 482. RISK-482
- **risk_id**: RISK-482
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 SFP1_RX_P/SFP1_RX_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-482-rule_engine_v3-SI.diff_pair_symmetry

## 483. RISK-483
- **risk_id**: RISK-483
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 SFP1_TX_P/SFP1_TX_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-483-rule_engine_v3-SI.diff_pair_symmetry

## 484. RISK-484
- **risk_id**: RISK-484
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 SFP2_RX_P/SFP2_RX_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-484-rule_engine_v3-SI.diff_pair_symmetry

## 485. RISK-485
- **risk_id**: RISK-485
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 SFP2_TX_P/SFP2_TX_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-485-rule_engine_v3-SI.diff_pair_symmetry

## 486. RISK-486
- **risk_id**: RISK-486
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 SFP3_RX_P/SFP3_RX_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-486-rule_engine_v3-SI.diff_pair_symmetry

## 487. RISK-487
- **risk_id**: RISK-487
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 SFP3_TX_P/SFP3_TX_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-487-rule_engine_v3-SI.diff_pair_symmetry

## 488. RISK-488
- **risk_id**: RISK-488
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 差分对 SFP_VREF_CLK_P/SFP_VREF_CLK_N (置信度100%): 对称 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-488-rule_engine_v3-SI.diff_pair_symmetry

## 489. RISK-489
- **risk_id**: RISK-489
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 LOCK_SCL: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-489-rule_engine_v3-SI.i2c_pullup

## 490. RISK-490
- **risk_id**: RISK-490
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_I2C_SCL2: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-490-rule_engine_v3-SI.i2c_pullup

## 491. RISK-491
- **risk_id**: RISK-491
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 QSFP_SDA_: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-491-rule_engine_v3-SI.i2c_pullup

## 492. RISK-492
- **risk_id**: RISK-492
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 QSFP_SCL_: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-492-rule_engine_v3-SI.i2c_pullup

## 493. RISK-493
- **risk_id**: RISK-493
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 LOCK_SDA: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-493-rule_engine_v3-SI.i2c_pullup

## 494. RISK-494
- **risk_id**: RISK-494
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_I2C_SDA2: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-494-rule_engine_v3-SI.i2c_pullup

## 495. RISK-495
- **risk_id**: RISK-495
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_I2C_SDA2_: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-495-rule_engine_v3-SI.i2c_pullup

## 496. RISK-496
- **risk_id**: RISK-496
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_I2C_SCL2_: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-496-rule_engine_v3-SI.i2c_pullup

## 497. RISK-497
- **risk_id**: RISK-497
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_I2C_SCL1_: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-497-rule_engine_v3-SI.i2c_pullup

## 498. RISK-498
- **risk_id**: RISK-498
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_I2C_SDA1_: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-498-rule_engine_v3-SI.i2c_pullup

## 499. RISK-499
- **risk_id**: RISK-499
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_SDA: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-499-rule_engine_v3-SI.i2c_pullup

## 500. RISK-500
- **risk_id**: RISK-500
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_I2C_SCL1: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-500-rule_engine_v3-SI.i2c_pullup

## 501. RISK-501
- **risk_id**: RISK-501
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_I2C_SDA1: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-501-rule_engine_v3-SI.i2c_pullup

## 502. RISK-502
- **risk_id**: RISK-502
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 M_SCL: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-502-rule_engine_v3-SI.i2c_pullup

## 503. RISK-503
- **risk_id**: RISK-503
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 EX_POC_AMP_SCL: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-503-rule_engine_v3-SI.i2c_pullup

## 504. RISK-504
- **risk_id**: RISK-504
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: I2C 网络 EX_POC_AMP_SDA: 有上拉电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-504-rule_engine_v3-SI.i2c_pullup

## 505. RISK-505
- **risk_id**: RISK-505
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 PMUBOARD_RST2: 有偏置电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-505-rule_engine_v3-SI.reset_bias

## 506. RISK-506
- **risk_id**: RISK-506
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 POW_RESET: 有偏置电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-506-rule_engine_v3-SI.reset_bias

## 507. RISK-507
- **risk_id**: RISK-507
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 POW_RESET_: 有偏置电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-507-rule_engine_v3-SI.reset_bias

## 508. RISK-508
- **risk_id**: RISK-508
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 /CLK_DIVIDE_RST: 有偏置电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-508-rule_engine_v3-SI.reset_bias

## 509. RISK-509
- **risk_id**: RISK-509
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 QSFP_RESETL: 有偏置电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-509-rule_engine_v3-SI.reset_bias

## 510. RISK-510
- **risk_id**: RISK-510
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 DDR4_RESET: 有偏置电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-510-rule_engine_v3-SI.reset_bias

## 511. RISK-511
- **risk_id**: RISK-511
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 复位网络 PMUBOARD_RST1: 有偏置电阻 ✓
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-511-rule_engine_v3-SI.reset_bias

## 512. RISK-512
- **risk_id**: RISK-512
- **severity**: INFO
- **priority**: P2
- **category**: SI
- **source**: rule_engine_v3
- **description**: 检查了 536 个信号网络，电压域一致
- **impact**: SI 类信息项，需要人工判断是否影响当前设计目标。
- **mitigation**: 人工确认该信息项是否需要转为设计约束或风险项。
- **status**: open
- **evidence_id**: EVID-512-rule_engine_v3-SI.voltage_domain_match
