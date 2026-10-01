# 0010: 全局生效高危命令透视契约（三联单机制）

用户要求将高危命令透视机制精简为永久契约，并全局应用到 Hermes 的所有 Profile 中，彻底终结黑盒审查恐惧。

## 已完成的落地变更
1. **持久记忆写入 (`MEMORY.md`)**：
   - 记录全局规则：在请求危险/敏感指令（rm, chmod/chown, kill, 全局包管理, 网络系统级变更）时，必须输出三联单（目标 Target、爆炸半径 Blast Radius、救生圈 Rollback/Dry-run），严禁甩出裸命令。
2. **多 Profile 系统人设同步 (`SOUL.md`)**：
   - 已同步注入：
     - `default` (`/Users/liangbo/.hermes/SOUL.md`)
     - `hermes001` (巴菲特 / 炒股副驾)
     - `hermes002` (lushu-app 小程序专家)
     - `hermes003` (学习与认知跃迁导师)
3. **效果保障**：
   - 以后无论切换到哪个 Bot 或 Profile，只要涉及敏感指令，AI 必须老老实实交代清楚影响面与回滚命令。
