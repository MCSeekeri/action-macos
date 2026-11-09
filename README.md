# action-macos

在 GitHub Actions 的 `macos-latest` runner 上开一个标准 SSH 调试会话（`owenthereal/action-upterm`）。

## 说明

- `limit-access-to-actor` 自动使用触发者 GitHub 账号上的 SSH 公钥；`users` 可指定其他人。
- `secrets.SSH_AUTHORIZED_KEYS` 可选，仅写入 runner 的 `authorized_keys` 备用。
- job 最长 6 小时，无人连接 30 分钟后自动关闭。
