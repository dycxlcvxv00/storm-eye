# 风暴之眼 · 统计台账

> 仓库名 `storm-eye`（GitHub 仓库名只能用 ASCII 字母/数字/`.`/`-`/`_`，故用英文拼音；中文名写在这里）

《爆战丨无限弹幕》账号运营台账：**角色晶石台账**（收支闭合 / 来源分桶 / 转移模型）与**打图经验台账**（升级记录 / 8 点结算口径）。

## 仓库定位

- ✅ 本仓库**只放统计台账**——各类数据快照、分析文档、录入工具
- ❌ **游戏源码不在这里**——请去独立仓库 [`baozhan-demo`](https://github.com/dycxlcvxv00/baozhan-demo)

## 🔗 固定链接（GitHub Pages）

> **https://dycxlcvxv00.github.io/storm-eye/**

- 根路径 `index.html` = 导航页，自动跳转台账首页
- **角色晶石台账**：`index-records.html`（自包含单文件）
- **打图经验台账**：`index-xp.html`（自包含单文件）
- 看到旧内容先强刷：Windows `Ctrl+F5` / macOS `Cmd+Shift+R`

> 注：本仓库由原 `baozhan-game` 改名而来。存档在浏览器 localStorage（按域名隔离，不随路径变化），换址后存档仍在；如丢失可用 `data.json` 快照通过页面「仓库恢复」按钮导入。

## 目录结构

```
index.html              导航页（跳转台账首页）
index-records.html      角色晶石台账（v12 竖版卡牌 · A 版深空霓虹配色）
index-xp.html           打图经验台账
data.json               数据快照（供页面「仓库恢复」按钮使用）
data/
  data.json             快照副本
  scripts/              push_snapshot.py（同步快照）+ 各项测试脚本
docs/
  台账维护手册.md        ★ 项目唯一权威文档，新会话必读
  台账维护手册-详细版.md  详细版（数据架构 / 口径 / SOP / 变更日志）
  档位与每日产出分析.md   档位 × 产出分析报告
  档位加成对异界产出影响分析.md
tools/
  xp.py                 经验台账工具脚本（单条/批量录入、发布）
  readshot.py           经验台账截图一键识别
  retry_*.py            推送重试工具
theme-preview.html       卡牌配色重做模板（仅预览，未实装）
.nojekyll                禁用 Jekyll，Pages 原样发布
```

## 数据真相源

台账记录的真相源在**私有仓 `baozhan-data`**；本仓 `data.json` 只是快照。

## 新会话接续

1. 先读 `docs/台账维护手册.md`（数据架构 / 口径 / SOP / 变更日志）
2. 改代码 → `git push origin main` → Pages 1~2 分钟自动生效
