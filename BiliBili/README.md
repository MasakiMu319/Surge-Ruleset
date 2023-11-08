# BILIBILI

眾所周知的一點，BILIBILI 的 CDN 管理相當混亂。所以很多時候，在線播放視頻的體驗會非常糟糕。

最佳的解決方案當然是保證每次播放視頻前可以優選 CDN 到最合適的服務器 IP 地址。但顯然是小題大做。

OptimizeOptions.txt 文件中只包含了 MCDN。就筆者的體驗來說，MCDN 的效果是最糟糕的。建議各位可以自行嘗試。

有時候 CN 區域內也會使用 Akamai CDN，造成極為難受的使用感受，如果沒有分區需求，建議直接屏蔽掉。

截止 2023-11-09，屏蔽掉 Akamai、MCDN，就能自動回落到 sz CDN。

# 部分常見 CDN
- upos-hz-mirrorakam.akamaized.net：通常作為海外（臺灣、美國…） CDN。
- upos-sz-mirroraliov.bilivideo：國內最佳 CDN。
- cn-hk-eq-*.bilivideo.com：香港 CDN。
