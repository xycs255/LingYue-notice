# LingYue-notice

灵悦（LingYue）读取本仓库 `main` 分支的 [`control.json`](control.json)，用于推送公告和强制结束可信会话。

- 发布公告：填写 `announcement`（`id`、`title`、`message`、`level`），新公告请使用新的 `id`；撤下公告把它改为 `null`。
- 强制所有设备退出可信会话：把 `revokeTrustedSessionsRevision` 加 1。只能增大。

修改后通常几分钟内生效（GitHub raw CDN 缓存约 5 分钟）。字段说明见主仓库 `docs/REMOTE_CONTROL.md`。

本仓库是公开的，只放这个控制文件，不要提交源码、密码或 TOTP 相关内容。
