### 问题 1: 执行 git commit 时，Git 提示需要检查并设置你的 用户名 和 电子邮件地址，以确保它们正确反映你的身份(Git 会自动根据你的系统用户名和主机名来推测这些信息，但如果它们不准确，Git 会提醒你进行修正)

```
执行 git commit 时，Git 提示需要检查并设置你的 用户名 和 电子邮件地址，以确保它们正确反映你的身份(Git 会自动根据你的系统用户名和主机名来推测这些信息，但如果它们不准确，Git 会提醒你进行修正)
Committer: your-username <demo@test.tech.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 86 insertions(+)
 create mode 100644 Create Git repository.md
```

### 解决方案：

1. **设置全局用户名和电子邮件地址**

首先，设置全局的用户名和电子邮件地址，确保 Git 在所有仓库中都使用这个配置：

```git
git config --global user.name "Dakang Qi"
git config --global user.email "aaa@abcCN.TECH.COM"
```

这样，你的 **用户名** 和 **电子邮件地址** 就会被正确配置，每次提交时都会使用这些信息。

2. **如果你只想修改当前仓库的用户名和电子邮件**

如果你只希望在当前仓库使用不同的用户名和电子邮件地址，可以不使用 --global 选项：

```git
git config user.name "Dakang Qi"
git config user.email "aaa@abcCN.TECH.COM"
```

3. **修改提交历史中的身份信息**

如果你已经提交了代码，并且希望 修正提交历史中的身份信息，可以使用 git commit --amend --reset-author 来重新设置作者信息并修改最后一次提交：

```git
git commit --amend --reset-author
```

这个命令会重新打开你的编辑器，允许你修改提交信息和作者信息，之后可以保存并退出，提交就会更新为新的身份。

**解释：**

git config --global：设置全局配置，意味着所有 Git 仓库都会使用该设置。

git config：仅针对当前仓库设置用户名和电子邮件地址。

git commit --amend --reset-author：修正最新提交的作者信息。
