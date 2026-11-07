# G5/G9 产品修改记录

- 产品编号：$(@{number=3; product_id=JLZ-EDU-SK-003; chinese_name=年度招生规划; english_name=Annual Enrollment Planner; repository_name=edu-annual-enrollment-planner; repository_url=https://github.com/jinlize-tech/edu-annual-enrollment-planner; product_type=Skill; category_code=01; category=01 招生营销中心; description=年度招生目标、月度计划、招生节点和资源配置。; target_users=System.Object[]; core_input=年度营收与招生目标、校区容量、开班计划、季节节奏、预算与人员; main_output=年度招生目标表、月度节点、渠道与预算分配、里程碑和风险清单; product_risk=将目标假设当作实际市场容量; dedup_label=需要明确差异化; dedup_note=与校长经营OS LITE相比聚焦招生目标分解，不输出综合经营系统；与单次活动策划相比覆盖全年节奏。; development_status=Planned / 待研发; license=Apache-2.0; spec_version=1.0.0; workbuddy_status=PLANNED_FOR_WORKBUDDY}.product_id)
- 产品名称：年度招生规划
- 基线：EDUCATION_BASELINE_V1.0.0
- 基线提交：$BaselineCommit
- 原版本：1.0.0
- 新版本：1.0.1

## 本次修改

1. 强化产品专属执行流程、输入核对和输出验收规则。
2. 新增 scripts/validate_input.js，实际检查必填字段、冲突、未确认数据和敏感信息。
3. 新增正常、缺失、冲突、敏感信息和非法JSON场景输入。
4. 测试升级为 T1–T7 分层并保存逐项检查结果。
5. 安装包加入 Apache-2.0 LICENSE 和 THIRD_PARTY_NOTICES.md。
6. 安装包升级为 1.0.1，加入许可证、第三方声明和输入校验脚本，保留 1.0.0 ZIP。
7. 按本产品冻结规格补充专属处理规则、输入到成果的核对矩阵和去重边界。

## 产品专属增强

- 核心任务：年度招生目标、月度计划、招生节点和资源配置。
- 主要风险：将目标假设当作实际市场容量
- 去重边界：与校长经营OS LITE相比聚焦招生目标分解，不输出综合经营系统；与单次活动策划相比覆盖全年节奏。

- 先锁定招生目标、课程、时间窗口、目标客群和可得预算，再讨论创意与渠道。
- 把假设线索量、转化率和单价分别列示，不以单一历史数据外推全部结果。
- 逐项检查渠道费用、人员投入、活动固定成本和单人可变成本，防止重复计费。
- 对宣传承诺、价格、名额、效果和第三方素材做合规与真实性复核。

## 运行边界

- 本地模型行为：NOT_RUNTIME_VERIFIED
- WorkBuddy平台验证：WORKBUDDY_VALIDATION_NOT_IN_SCOPE
- 本轮不执行上传、安装、审核或正式发布。
