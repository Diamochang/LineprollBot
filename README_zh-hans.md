LineprollBot 是一个为“线性滚动Bot”创建的仓库，用于存放实现她功能的全部代码，并将其公开。

# “线性滚动Bot”是谁？
这缘起于 Miraheze 农场曾托管，现已关闭的 DiamoWiki。Diamochang 曾在该wiki上创建名为“DiamoWiki-AWBRobot”的全域账号，准备通过这个账号操作 [AutoWikiBrowser](https://zh.wikipedia.org/wiki/Wikipedia:AutoWikiBrowser) 执行自动化任务。结果，技术还没搞好，DiamoWiki 于 2022 年关站了，Diamochang 本人因此退出 MediaWiki 建站领域，此机器人就此胎死腹中。

2023 年中，Diamochang 向 Miraheze 申请创建“[明安里市 Wiki](https://minganlicity.miraheze.org)”，申请获批，就此重回 MediaWiki 建站领域。此时的他已经接触 Python，希望将以前注册的全域机器人账号重新利用，结果——他把机器人的登录密码忘了。没办法，他只好重新注册一个全域账号，[LineprollBot](https://login.miraheze.org/wiki/User:LineprollBot)（线性滚动Bot）就此诞生。

# 技术
线性滚动Bot使用 Python，不过特殊情况也会使用 PHP 和 JavaScript。目前所有功能实现均依靠 Python，所使用的 Bot 包如下：
* [Pywikibot](https://github.com/wikimedia/pywikibot) - 维基媒体基金会官方开发的 MediaWiki Python Bot 包
* Misskey Python Bot 包
    * [Misskey.py](https://github.com/YuzuRyo61/Misskey.py) - 适用于大多数主流 Misskey 版本的 Bot 包
    * [Misspy](https://github.com/misspy-dev/misspy) - 适用于实例 Misskey 版本为 v13 及以上的 Bot 包

# To-do list
* [ ] 机器人远程停止
* [ ] 将[推荐的明安里市 Wiki 条目和文章](https://minganlicity.miraheze.org/wiki/User:LineprollBot/Featured_Articles)选择性地搬至联邦宇宙
* [ ] 通过 UptimeRobot 实时监控明安里市系列站点运行情况，每 6 小时（东八区 UTC+8）在联邦宇宙跟进情况。有异常则马上在联邦宇宙跟进，并向我的即时通讯账号发信通知
* [ ] 给所有出现五处以上常见脏话的条目添加模板{{[Tone](https://minganlicity.miraheze.org/wiki/Template:Tone)}}

# 参与和改进
如果机器人有问题，可以向这个仓库提 Issues；如果有建议，欢迎 PR。

如果问题和建议有关明安里市系列网站，且你在 Miraheze 拥有全域账号，也可以在提出 Issues 和 PR 之后到[这里](https://minganlicity.miraheze.org/wiki/User_talk:LineprollBot/Issues)把问题和建议再说一遍。你可以直接把 Github 的描述复制过来然后 wikitext 化，也可以以对着女孩子说话的口吻把它们复述一遍（因为这个机器人在明安里市世界观内是一位女性机械生命体）。只要我看得懂，沟通基本不成问题。

# 许可证
由于使用的包许可证多样，为防止冲突，本仓库不设统一的许可证。如果要以我的代码为基础编写新的机器人，记得多关注一下上游的许可证，以免冲突。

