# DevOps Trending Collector 🔥

自动收集 GitHub 上最热门的 DevOps 相关项目和技能。

## 📁 文件结构

```
DevOps/
├── README.md              # 本文件
├── trending.md            # 热门项目总结 (每 6 小时更新)
├── collect_devops_trending.py  # 收集脚本
└── .git/                  # Git 仓库
```

## ⏰ 更新频率

- **每 6 小时** 自动执行一次
- 自动收集 GitHub 上 Star 数最高的 DevOps 相关项目
- 生成 Markdown 格式的报告

## 🚀 使用方法

### 手动执行

```bash
cd /home/admin/.openclaw/workspace/DevOps
python3 collect_devops_trending.py
```

### 查看报告

打开 `trending.md` 文件查看最新的热门项目列表。

## 📊 数据说明

- 数据来源：GitHub Search API
- 搜索条件：`topic:devops stars:>1000`
- 排序方式：按 Star 数降序
- 每次收集：Top 15 项目

## 🔧 配置

如需使用 GitHub API 获取更高配额，可设置环境变量：

```bash
export GITHUB_TOKEN=your_github_token
```

## 📝 更新日志

- 2026-02-27: 初始版本创建

---
*Automated DevOps Trending Collector*
