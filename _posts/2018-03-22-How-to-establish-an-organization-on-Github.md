---
layout: post
title: 在Github上创建Organization
categories:
- Tutorials
---

系统分析与设计这门课要求做一个完整团队协作过程的大作业， 老师原意是创建一个新的Github个人账号来存放项目仓库， 但实际上， Github Organization 可以很方便的创建团队账号。 邀请别人加入自己的Organization， 我们可以继续用自己的账号在Organization下创建、管理Repo， 而对外显示的时候，Repo实际从属于Organization，这就达到了我们想要的效果。

![Displayed on Dashboard]({{site.url}}/assets/img/organization-setup/dashboard-display-2.png}})

例如： 我们的Organization名字是`Chun-Ge`，就可以直接从这里看到我们的[Organization Profile](https://github.com/Chun-Ge)，以及下面的Repo。 你目前看到的博客就是部署在该Organization下的`Chun-Ge.github.io`的`jekyll github page`。

## Step by Step

首先， 在自己的Github首页右上方处， 点击“+”号， 然后在下拉选项中， 选`New Organization`。

![Click New Organization Button]({{site.url}}/assets/img/organization-setup/new-organization.png}})

然后进入到创建Organization的页面。 设置好Organization Name和Billing Email。 我们只是用来做校内的课程项目， Plan显然选择Free， 以及不要勾选"This account is owned by a business"。 设置完毕之后到页面底部，点击`Create Organization`。

PS： Billing Email 是Github向该Organization发送账单用的邮箱 (如果有消费的话)， **并不是**此Organization对外显示的邮箱。 后者需要在Organization创建完毕后再进行设置。

![Set Organization Name]({{site.url}}/assets/img/organization-setup/set-name.png}})

单击`Create Organization`之后， 会进入到Invite Members的页面， 我们可以在页面中的搜索框中直接输入队友的Github账号来邀请其加入。 在搜索结果中点击队友的账号即可发出邀请。 操作十分简单，这里不再赘述。

![Invite Members]({{site.url}}/assets/img/organization-setup/invite-members.png}})

**如果后面还想要邀请其他人加入Organization， 可以到你的Organization信息页面中， 点击People选项卡， 然后在出现的界面中点击右边的"Invite member"。**

![Invite Members 2]({{site.url}}/assets/img/organization-setup/invite-members-2.png}})

到此我们的Organization已经创建完毕了， 我们以后可以通过`github.com/{your-organization-name}`的路径来查看和管理该Organization的信息。 然后就可以像操作普通个人账号一样，为我们的Organization创建Repo、修改信息等等。 以后依然使用我们自己的账号（已从属于该Organization）登陆后， 就可以在首页→Browse Activity左上方的下拉菜单中， 选择自己的Organization 进行查看。

![Displayed on Dashboard]({{site.url}}/assets/img/organization-setup/dashboard-display.png}})

PS： **成员权限：** People选项卡中可以看到， Member的权限有2种： `Owner` 和 `Member`。 `Owner` 拥有的权限最高， `Member`属于"普通用户"， **不过二者都可以进行常见的Repo操作**， 想要了解具体的权限差别， 可以查看官方对2种权限的说明。 默认情况下， Organization的创建者是`Owner`， 邀请进来的其他成员默认是`Member`。 但`Owner`可以同时存在多个。 成员的权限也都可以很方便地在People选项卡中修改。

<!-- Syntax highlighting with Solarized theme.

{% highlight ruby %}
class User < ActiveRecord::Base
  attr_accessible :email, :name

  ... tons of other crap ...

end

{% endhighlight %} -->
