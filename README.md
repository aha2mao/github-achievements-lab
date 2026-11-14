# github-achievements-lab
GitHub 协作练习：验证 Issue、Pull Request 与成就触发流程。

## 练习流程

1. 在 Issue 中写清任务和验收条件。
2. 在分支上完成一个可独立审阅的改动。
3. 检查差异，将验证结果写入 PR。
4. 合并后核对主分支，并关闭已完成的 Issue。
5. 查看个人 Achievements 页面，单独确认徽章结果。

## 命令示例

以下命令只读取本练习仓库。写操作应先核对目标和内容。

```sh
gh repo view aha2mao/github-achievements-lab
gh issue list --repo aha2mao/github-achievements-lab --state all
gh pr list --repo aha2mao/github-achievements-lab --state all
git diff --check
```

## 免费成就路线

下表门槛来自社区观察，GitHub 未保证固定条件或到账时间。

| 成就 | 基础条件 | 练习重点 |
| --- | --- | --- |
| Quickdraw | 创建 Issue 或 PR 后 5 分钟内关闭 | 提前明确验收步骤，完成后及时关闭 |
| YOLO | 自己的 PR 未经审查即合并 | 仅适用于无需他人审查的低风险练习 |
| Pull Shark | 2 个 PR 被合并；后续档位 16、128、1024 | 每次提交一个完整改动 |
| Pair Extraordinaire | 含共同作者提交的 PR 被合并 | 准确记录实际共同作者；AI 署名能否触发待验证 |
| Galaxy Brain | 2 个 Discussions 回答被采纳 | 回答真实问题，由其他用户采纳 |
| Starstruck | 自己创建的仓库达到 16 个 Star | 提供别人愿意使用、收藏的项目 |

Public Sponsor 需要赞助支出，不属于免费路线。Arctic Code Vault 和 Mars 2020 属于历史活动。

## 协作署名

此次说明由 aha2mao 提出目标，Codex 起草并核对命令与来源。
提交中的 Codex 署名表示 AI 辅助贡献，不表示另一位人类参与。
署名邮箱不保证关联到 GitHub 用户，也不保证触发 Pair Extraordinaire。
GitHub 官方要求贡献计入某位共同作者时，使用与其账号关联的邮箱。

## 参考

- [GitHub 成就说明](https://docs.github.com/en/account-and-profile/reference/profile-reference#earning-achievements)
- [共同作者提交格式](https://docs.github.com/en/pull-requests/how-tos/commit-changes/creating-a-commit-with-multiple-authors)
- [社区维护的徽章条件与等级](https://github.com/Schweinepriester/github-profile-achievements)
- [GitHub Community 停发成就公告](https://github.com/orgs/community/discussions/106536)
