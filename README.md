# 晚枝配置仓库

晚枝微信虚拟女友的配置文件共享仓库。

## 快速使用

### 下载配置

在 Operit 中执行：

- 调用 wanzhi_github_sync:download_config
- 参数：github_repo=qawse110/wanzhi-configs, file_name=文件名

### 上传配置

1. 生成 GitHub Token: https://github.com/settings/tokens/new （勾选 repo 权限）
2. 在 Operit 中执行：
   - 调用 wanzhi_github_sync:upload_all_configs
   - 参数：github_token=你的token, github_repo=qawse110/wanzhi-configs

## 配置文件说明

| 文件 | 用途 | 说明 |
|------|------|------|
| wanzhi_configs/relationship_rules.json | 6阶段关系规则 | 加减分、红线、语气风格、主动关心规则 |
| wanzhi_configs/reply_guardrails.json | 回复质检 | 禁用词、长度约束、系统暴露防护 |
| wanzhi_configs/晚枝.json | 角色卡 | 人设、说话风格、各阶段行为约束 |

## 重要提醒

上传配置时请务必检查，确保不包含以下隐私数据：
- 聊天记录
- 微信账号/微信号
- 真实姓名/地址
- 手机号/身份证号
- 任何个人隐私信息

## 仓库结构

```
wanzhi-configs/
├── README.md
├── .gitignore
└── wanzhi_configs/
    ├── relationship_rules.json
    ├── reply_guardrails.json
    └── 晚枝.json
```

## 许可

MIT License
