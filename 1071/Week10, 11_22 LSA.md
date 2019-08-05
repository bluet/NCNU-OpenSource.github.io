# Week10, 11/22 LSA

- 第一組：
    - 106213014 歐芷欣
    - 106213019 蘇美婷
- 第二組：
    - 107213511
    - 107213517
    - 107213506
- 第三組 :
    - 105213007 王威
    - 105213028 丁翊軒
    - 106407023 陳于真
- 第四組：
    - 106213017 蔡佳軒
    - 106213022 莊詠婷
- 第五組：
    - 105213004 陳冠瑜
    - 105213019 許家瑋
- 第六組:
    - 104321002 何建宏
    - 104321003 謝萬霖
    - 104321024 蔡旻勳
- 第七組:
    - 106321009 羅罡兆
- 第八組︰
    - 104321051 林煒星
    - 104321059 錢詠恩
    - 104321067 梁杏兒
- 第九組︰
    - 104321060 何曉倩
    - 104321062 王子佳
    - 104321070 鄭芷君

## OSI架構
+ 傳送層
    + TCP: 會去確認這個封包有實際被對方接收，所需時間比 UDP 長
    + UDP: 不去確定對方是否有收到，會交給應用層去做確認 (多應用於串流時序)
+ ARP: 負責將 IP 位址轉換(對應)成 Mac 位址的一種通訊協定
+ RARP: 將 Mac 位址對應到 IP 位址 
+ `arp -n` ARP緩存表，表裡有互相對應的IP地址與MAC地址
+ DNS: Domain Name System，會把host對應到IP位址
    + 推薦用1.1.1.1
+ `dig +trace +dnssec <domain name>. @<nearest dns server>` (學校DNS server: 163.22.2.1) trace dns 查詢過程
+ 内網傳輸是使用MAC Address傳輸
+ `route -n` 與本機直接連線的網路區段

Q: 101.23.45.67/27 起始到結束IP位址
Q: 101.23.45.168/28 起始到結束IP位址
A: [ip calculater](http://jodies.de/ipcalc)