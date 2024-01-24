（習慣粵語？請點[呢度](README_yue.md)閲讀粵語版。）

LineprollBot 是一個為“線性滾動Bot”創建的倉庫，用於存放實現她功能的全部代碼，並將其公開。

# “線性滾動Bot”是誰？
這緣起於 Miraheze 農場曾託管，現已關閉的 DiamoWiki。Diamochang 曾在該wiki上創建名為“DiamoWiki-AWBRobot”的全域賬號，準備通過這個賬號操作 [AutoWikiBrowser](https://zh.wikipedia.org/wiki/Wikipedia:AutoWikiBrowser) 執行自動化任務。結果，技術還沒搞好，DiamoWiki 於 2022 年關站了，Diamochang 本人因此退出 MediaWiki 建站領域，此機器人就此胎死腹中。

2023 年中，Diamochang 向 Miraheze 申請創建“[明安裏市 Wiki](https://minganlicity.miraheze.org)”，申請獲批，就此重回 MediaWiki 建站領域。此時的他已經接觸 Python，希望將以前註冊的全域機器人賬號重新利用，結果——他把機器人的登錄密碼忘了。沒辦法，他只好重新註冊一個全域賬號，[LineprollBot](https://login.miraheze.org/wiki/User:LineprollBot)（線性滾動Bot）誕生。

# 技術
線性滾動Bot使用 Python，不過特殊情況也會使用 PHP 和 JavaScript。目前所有功能實現均依靠 Python，所使用的 Bot 包如下：
* [Pywikibot](https://github.com/wikimedia/pywikibot) - 維基媒體基金會官方開發的 MediaWiki Python Bot 包
* Misskey Python Bot 包
    * [Misskey.py](https://github.com/YuzuRyo61/Misskey.py) - 適用於大多數主流 Misskey 版本的 Bot 包
    * [Misspy](https://github.com/misspy-dev/misspy) - 適用於實例 Misskey 版本為 v13 及以上的 Bot 包

# To-do list
* [ ] 機器人遠程停止
* [ ] 將[推薦的明安裏市 Wiki 條目和文章](https://minganlicity.miraheze.org/wiki/User:LineprollBot/Featured_Articles)選擇性地搬至聯邦宇宙
* [ ] 通過 UptimeRobot 實時監控明安裏市系列站點運行情況，每 6 小時（東八區 UTC+8）在聯邦宇宙跟進情況。有異常則馬上在聯邦宇宙跟進，並向我的即時通訊賬號發信通知
* [ ] 給所有出現五處以上常見髒話的條目添加模板{{[Tone](https://minganlicity.miraheze.org/wiki/Template:Tone)}}

# 參與和改進
如果機器人有問題，可以向這個倉庫提 Issues；如果有建議，歡迎 PR。

如果問題或建議有關明安裏市系列網站，且你在 Miraheze 擁有全域賬號，也可以在提出 Issues 或 PR 之後到[這裏](https://minganlicity.miraheze.org/wiki/User_talk:LineprollBot/Issues)把問題或建議再説一遍。你可以直接把 Github 的描述複製過來然後 wikitext 化，也可以以對着女孩子説話的口吻把它們複述一遍（因為這個機器人在明安裏市世界觀內是一位女性機械生命體）。只要我看得懂，溝通基本不成問題。

# 許可證
由於使用的包許可證多樣，為防止衝突，本倉庫不設統一的許可證。如果要以我的代碼為基礎編寫新的機器人，記得多關注一下上游的許可證，以免衝突。
