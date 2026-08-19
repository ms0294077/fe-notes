# DHCP・DNS・ICMP・ARP・MACアドレス

> [!summary] 一句話
> DHCP配發設定、DNS解析名稱、ICMP傳遞控制訊息、ARP由IP查MAC。

## DHCP

- **用語：** DHCP（Dynamic Host Configuration Protocol）
> 自動分配IP位址及網路設定。

通常會自動設定：

- IPアドレス
- サブネットマスク
- デフォルトゲートウェイ
- DNSサーバー

## DNS

- **用語：** DNS（Domain Name System）
> 將容易記憶的ドメイン名轉換成IP位址。

例如：

example.com
→ DNS查詢
→ 對應的IP位址

## ICMP

- **用語：** ICMP（Internet Control Message Protocol）
> 傳送網路錯誤及狀態訊息。

例如：

- ping
- 通知目的地無法到達

## ARP

- **用語：** ARP（Address Resolution Protocol）
> 根據IP位址查詢同一LAN內對應的MAC位址。

## MACアドレス

> 用來識別同一LAN內網路設備的位址。

- 第2層使用
- Switch根據MAC位址轉送資料
