# Git 实验仓库（learngit63）

> 开源文化课程 · Git 常用命令练习

| 项目 | 内容 |
| --- | --- |
| 姓名 | 李春辉 |
| 学号 | 2025131063 |
| 环境 | Windows · Git Bash · Git 2.53.0 |
| 日期 | 2026-10-29 |

## 实验内容

按课件顺序完整练习了一遍 Git 的本地操作与远程协作：

1. **基本流程**：`git status` 查看状态 → `git diff` 查看改动 → `git add` 暂存 → `git commit` 提交
2. **查看历史**：`git log`、`git log --pretty=oneline`、`git log --oneline`
3. **版本回退**：`git reset --hard HEAD^` 回到上一版；`git reset --hard <commit_id>` 指定版本
4. **找回版本**：`git reflog` 查看 HEAD 移动记录，救回被回退掉的提交
5. **撤销修改**：`git checkout -- <file>` 丢弃工作区改动
6. **删除文件**：`rm` 后 `git status` 看到 `deleted`；`git rm` 一步完成删除并暂存
7. **远程仓库**：`ssh-keygen` 生成密钥 → GitHub 添加公钥 → `git remote add origin` → `git push -u origin main`

## 文件说明

| 文件 | 说明 |
| --- | --- |
| `test2025131063.txt` | 主实验文件，内容经历了 `I am learning git.` → `111` → `222` |
| `file2025131063.txt` | 删除实验中创建的文件，已从历史恢复 |

## 常用命令速查

```bash
git status                  # 看当前状态
git diff                    # 看工作区改了什么
git add <file>              # 放进暂存区
git commit -m "说明"         # 生成一个版本
git log --oneline           # 一行一个版本
git reset --hard HEAD^      # 回退到上一版（危险）
git reflog                  # 后悔药：看所有 HEAD 移动记录
git rm <file>               # 删除文件并暂存
git push                    # 推送到 GitHub
```

## 更新记录

- 2026-10-29：完成 SSH 配置、git remote add origin 与 git push -u origin main，本地仓库与 GitHub 同步。
