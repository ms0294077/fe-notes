# IP・IPsec

> [!summary] 一句話
> IP本身不提供加密；IPsec在IP層提供暗号化與認証，常用於VPN。

## IP／IPsec

### IP（Internet Protocol）

負責根據IP位址，把資料封包送到正確的目的地。

IP本身主要負責傳送資料，不提供加密功能。

### IPsec（IP Security）

在IP層對通訊進行加密與認證的技術。

主要作用：

- 防止竊聽
- 防止資料被竄改
- 確認通訊來源
- 常用於VPN

```text
負責把封包送到目的地
→ IP

保護、加密IP通訊
→ IPsec
```
