LineprollBot 系一個為“線性滾動Bot”創建嘅倉庫，用於存放實現佢功能嘅全部代碼，並將其公開。

# “線性滾動Bot”系邊個？
呢緣起於 Miraheze 農場曾託管，現已關閉嘅 DiamoWiki。Diamochang 曾喺該wiki上創建名為“DiamoWiki-AWBRobot”嘅全域賬號，準備通過呢個賬號操作 [AutoWikiBrowser](https://zh-yue.wikipedia.org/wiki/Wikipedia:AutoWikiBrowser) 執行自動化任務。結果，技術都冇搞好，DiamoWiki 於 2022 年關站，Diamochang 本人就退出 MediaWiki 建站領域，此機械人一嘢抹胎死腹中。

2023 年中，Diamochang 向 Miraheze 申請創建“[明安裏市Wiki](https://minganlicity.miraheze.org)”，申請獲批，佢得以重回 MediaWiki 建站領域。此時嘅佢已經接觸 Python，希望將以前註冊嘅全域機械人賬號重新利用，結果——佢將機械人嘅登錄密碼唔記得咗。冇辦法，佢要重新註冊一個全域賬號，[LineprollBot](https://login.miraheze.org/wiki/User:LineprollBot)（線性滾動Bot）誕生。

# 技術
線性滾動Bot使用 Python，不過特殊情況都會使用 PHP 同 JavaScript。目前所有功能實現均靠 Python，所使用嘅 Bot 包如下：
* [Pywikibot](https://github.com/wikimedia/pywikibot) - 維基媒體基金會官方開發嘅 MediaWiki Python Bot 包
* Misskey Python Bot 包
    * [Misskey.py](https://github.com/YuzuRyo61/Misskey.py) - 適用於大多數主流 Misskey 版本嘅 Bot 包
    * [Misspy](https://github.com/misspy-dev/misspy) - 適用於實例 Misskey 版本為 v13 同以上嘅 Bot 包

# To-do list
* [ ] 機械人遠程閘住
* [ ] 將[舉薦嘅明安裏市 Wiki 條目同文章](https://minganlicity.miraheze.org/wiki/User:LineprollBot/Featured_Articles)選擇性噉搬至聯邦宇宙
* [ ] 通過 UptimeRobot 即時睇實明安裏市系列站點運行情況，每 6 個鐘（東八區 UTC+8）喺聯邦宇宙跟進情況。有異常就馬上喺聯邦宇宙跟進，並向我即時通信賬號發信通知
* [ ] 畀所有出現五處以上常見粗口嘅條目添加模板{{[Tone](https://minganlicity.miraheze.org/wiki/Template:Tone)}}

# 參與和改進
如果機械人有問題，可以向個倉庫走提 Issues；如果有建議，歡迎PR。

如果問題或者建議有關明安裏市系列網站，且你喺 Miraheze 擁有全域賬號，都可以喺提出 Issues 或者 PR 之後到[呢度](https://minganlicity.miraheze.org/wiki/User_talk:LineprollBot/Issues)將問題同建議再講一次。你可唔可以直接將 Github 嘅描述複製過嚟，然後 wikitext 化，都可以以對女仔講口吻將佢哋複述一次（因為呢個機械人喺明安裏市世界觀內系一位女性機械生命體）。只要我睇得明，溝通基本唔成問題。

# 許可證
由於使用嘅包許可證多嘢架，為防止衝突，本倉庫唔設統一嘅許可證。如果要以我代碼為基礎編寫新嘅機械人，記得多關注下上游嘅許可證，以免衝突。

