# BILIBILI

眾所周知的一點，BILIBILI 的 CDN 管理相當混亂。所以很多時候，在線播放視頻的體驗會非常糟糕。

最佳的解決方案當然是保證每次播放視頻前可以優選 CDN 到最合適的服務器 IP 地址。但顯然是小題大做。

～～OptimizeOptions.txt 文件中只包含了 MCDN～～。就筆者的體驗來說，MCDN 的效果是最糟糕的。建議各位可以自行嘗試。

OptimizeOptions.txt 現在已經替換成DomesticCDN. txt.

有時候 CN 區域內也會使用 Akamai CDN，造成極為難受的使用感受，如果沒有分區需求，建議直接屏蔽掉。

～～截止 2023-11-09，屏蔽掉 Akamai、MCDN，就能自動回落到 sz CDN～～。
Update：2023-11-11，DomesticCDN.txt 盡可能覆蓋全面了嗶哩嗶哩的自建 CDN 和第三方 CDN 服務商，目前結果是會回落到 upos-sz。

# 部分常見 CDN
- upos-hz-mirrorakam.akamaized.net：通常作為海外（臺灣、美國…） CDN。
- upos-sz-mirroraliov.bilivideo：國內最佳 CDN。
- cn-hk-eq-*.bilivideo.com：香港 CDN。

# 供參考的資料
- [能不能搞个B站锁定CDN的方法，防止播放卡顿](https://github.com/bilibili-helper/bilibili-helper-o/issues/713)
- [话说我宽带网速都有挺好 有 1000M，但为啥用 Chrome 系浏览器看 B 站经常缓冲不过来？](https://v2ex.com/t/830394)
- [B 站自建的视频云域名和第三方服务商域名](https://rec.danmuji.org/dev/cdn-info/)