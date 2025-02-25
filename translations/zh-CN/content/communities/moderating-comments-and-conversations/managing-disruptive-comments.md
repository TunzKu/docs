---
title: 管理破坏性评论
intro: '您可以{% ifversion fpt or ghec %}隐藏、编辑、{% else %}编辑{% endif %}或删除对议题、拉取请求和提交的评论。'
redirect_from:
  - /articles/editing-a-comment
  - /articles/deleting-a-comment
  - /articles/managing-disruptive-comments
  - /github/building-a-strong-community/managing-disruptive-comments
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Community
shortTitle: 管理评论
---

## 隐藏评论

{% ifversion fpt or ghec %}组织版主以及对存储库有写入权限的任何人{% else %}任何人{% endif %} 都可以隐藏对议题、拉取请求和提交的评论。

如果评论偏离主题、已过期或已解决，您可能想要隐藏评论，以保持讨论重点或使拉取请求更易于导航和审查。 隐藏的评论已最小化，但对仓库具有读取权限的人员可将其展开。

![最小化的评论](/assets/images/help/repository/hidden-comment.png)

1. 导航到您要隐藏的评论。
2. 在评论的右上角，单击 {% octicon "kebab-horizontal" aria-label="The horizontal kebab icon" %}，然后单击 **Hide（隐藏）**。 ![显示编辑、隐藏、删除选项的水平烤肉串图标和评论调解菜单](/assets/images/help/repository/comment-menu.png)
3. 使用 "Choose a reason"（选择原因）下拉菜单，单击隐藏评论的原因。 然后单击 **Hide comment（隐藏评论）**。
  {% ifversion fpt or ghec %}
  ![选择隐藏评论的原因下拉菜单](/assets/images/help/repository/choose-reason-for-hiding-comment.png)
  {% else %}
  ![选择隐藏评论的原因下拉菜单](/assets/images/help/repository/choose-reason-for-hiding-comment-ghe.png)
  {% endif %}

## 取消隐藏评论

{% ifversion fpt or ghec %}组织版主以及对存储库有写入权限的任何人{% else %}任何人{% endif %} 都可以取消隐藏对议题、拉取请求和提交的评论。

1. 导航到您要取消隐藏的评论。
2. 在评论右上角，单击 **{% octicon "fold" aria-label="The fold icon" %} Show comment（显示评论）**。 ![显示评论文本](/assets/images/help/repository/hidden-comment-show.png)
3. 在展开的评论右上角，单击 {% octicon "kebab-horizontal" aria-label="The horizontal kebab icon" %}，然后单击 **Unhide（取消隐藏）**。 ![显示编辑、取消隐藏、删除选项的水平烤肉串图标和评论调解菜单](/assets/images/help/repository/comment-menu-hidden.png)

## 编辑评论

对仓库具有写入权限的任何人都可以编辑议题、拉取请求及提交上的评论。

编辑评论和删除无助于促进对话以及违反社区行为准则{% ifversion fpt or ghec %} 或 GitHub [社区指导方针](/free-pro-team@latest/github/site-policy/github-community-guidelines){% endif %} 的内容是明智之举。

Sometimes it may make sense to clearly indicate edits and their justification.

That said, anyone with read access to a repository can view a comment's edit history. 评论顶部的 **edited（已编辑）**下拉菜单包含编辑历史记录，其中会显示每次编辑的用户和时间戳。

![添加了表示内容编辑过的注释的评论](/assets/images/help/repository/content-redacted-comment.png)

## Redacting sensitive information

评论作者和具有仓库写入权限的任何人也都可以删除评论编辑历史记录中的敏感信息。 更多信息请参阅“[跟踪评论中的更改](/communities/moderating-comments-and-conversations/tracking-changes-in-a-comment)”。

1. 导航到您要编辑的评论。
2. 在评论的右上角，单击 {% octicon "kebab-horizontal" aria-label="The horizontal kebab icon" %}，然后单击 **Edit（编辑）**。 ![显示编辑、隐藏、删除和报告选项的水平烤肉串图标和评论调解菜单](/assets/images/help/repository/comment-menu.png)
3. 在评论窗口中，删除要删除的评论，然后输入 `[REDACTED]` 进行替换。 ![包含编辑过的内容的评论窗口](/assets/images/help/issues/redacted-content-comment.png)
4. 在评论底部，输入注释，说明您已编辑评论，也可以输入编辑的原因。 ![添加了表示内容编辑过的注释的评论窗口](/assets/images/help/issues/note-content-redacted-comment.png)
5. 单击 **Update comment（更新评论）**。

## 删除评论

对仓库具有写入权限的任何人都可以删除议题、拉取请求及提交上的评论。 组织所有者、团队维护员和评论作者也可删除团队页面上的评论。

如果评论包含一些对议题或拉取请求中的对话有建设性的内容，您可以编辑评论。

删除评论是调解员最后的选择。 如果整个评论没有给对话带来建设性的内容，或者违反社区的行为准则{% ifversion fpt or ghec %} 或 GitHub [社区指导方针](/free-pro-team@latest/github/site-policy/github-community-guidelines){% endif %}，删除评论是明智之举。

删除评论会创建对仓库具有读取权限的所有人可见的时间表事件。 但评论删除者的用户名只有能够写入仓库的人可见。 对于没有写入权限的任何人，时间表事件会匿名化。

![已删除评论的匿名化时间表事件](/assets/images/help/issues/anonymized-timeline-entry-for-deleted-comment.png)

{% note %}

**注：**议题或拉取请求的初始评论（或正文）不能删除。 但可以编辑议题和拉取请求正文，以删除不需要的内容。

{% endnote %}

### Steps to delete a comment

1. 导航到您要删除的评论。
2. 在评论的右上角，单击 {% octicon "kebab-horizontal" aria-label="The horizontal kebab icon" %}，然后单击 **Delete（删除）**。 ![显示编辑、隐藏、删除和报告选项的水平烤肉串图标和评论调解菜单](/assets/images/help/repository/comment-menu.png)
3. 也可以说明您删除了哪些评论，为什么要删除。

{% ifversion fpt or ghec %}
## 延伸阅读
- “[管理组织中的版主](/organizations/managing-peoples-access-to-your-organization-with-roles/managing-moderators-in-your-organization)”
{% endif %} 
