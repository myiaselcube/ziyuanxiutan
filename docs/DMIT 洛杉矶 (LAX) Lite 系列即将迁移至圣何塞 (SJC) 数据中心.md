# DMIT 洛杉矶 (LAX) Lite 系列即将迁移至圣何塞 (SJC) 数据中心

## 重要通知：LAX.Lite.u 系列服务迁移详情

尊敬的 DMIT.LAX.Lite.u 系列用户：

请查收您的邮箱，获取关于 LAX.Lite.u 系列服务迁移的完整通知。该系列服务代表「Unmetered Traffic Los Angeles Lite VM」，现将迁移至圣何塞数据中心。

### 迁移补偿方案
- **折扣优惠**：每项有效服务将获得常规6折+专属5折优惠（详见邮件）
- **退款政策**：剩余时长将按双倍金额退款，不符合条件部分退至账户余额
- **截止时间**：服务将于2022年10月14日23:00（UTC）后断网，请及时备份数据

> 提示：请务必查阅邮件中的具体条款细则

## 迁移背景与网络优化

DMIT 官方确认将把洛杉矶(LAX)的VM服务全面迁移至圣何塞(SJC)。调整后：
- 洛杉矶仅保留高端Pro网络（GIA线路）
- 圣何塞将提供4837优化线路

👉 [【点击查看】2025年最新 DMIT 优惠码及特价云服务器方案汇总](https://bit.ly/dmit_coupon)

## 迁移技术细节

### 核心变更项
1. **数据安全**：所有数据将完整迁移
2. **IP更换**：IPv4/IPv6地址均会更新为全新未使用IP
3. **价格不变**：续费价格保持原价
4. **补偿金**：可获得VM月付价值30%的账户余额
5. **硬件升级**：迁移至AMD EPYC Gen3平台（原为Gen2）
6. **时间规划**：预计一周内完成迁移
7. **后续通知**：将通过工单发送迁移完成报告

### IP变更注意事项
**必须安装Cloud-init**：
bash
Debian/Ubuntu: apt install cloud-init
CentOS 7: yum install cloud-init
CentOS 8+/RockyLinux/AlmaLinux: dnf install cloud-init
ArchLinux: pacman -S cloud-init

**未安装Cloud-init的处理方案**：
- 通过noVNC手动配置新IP
- 需提前设置root密码（即使使用SSH Key登录）

## 数据备份指南
强烈建议执行多维度备份：
- 采用「3-2-1」原则：3份备份，2种介质，1份异地
- 验证备份可恢复性
- 推荐使用rsync/scp等工具进行跨服务器备份

## 圣何塞4837线路优势
当前处于OpenBeta阶段，主要特点：
- **网络路由**：三网回程联通4837优化线路
- **测试IP**：174.136.205.15
- **注意事项**：暂不提供SLA保证，6.9美元基础款尚未开放

## 限时优惠活动
**特别提醒**：以下优惠仅适用于圣何塞VPS

### 折扣码
- 年付7折：`Lite-Annually-Recur-30OFF`
- 半年付8折：`Lite-Semi-Annually-Recur-20OFF`

### 买一送一活动
**截止时间**：2022年10月21日23:59（UTC）
- 赠品规则：
  - 首年免费（限年付订单）
  - 可拆分多订单（≤原订单金额）
  - 支持跨账户创建（需工单备注）
- 注意事项：
  - 每个订单限享一次
  - 需在10月26日前提交工单
  - 不适用TINY套餐