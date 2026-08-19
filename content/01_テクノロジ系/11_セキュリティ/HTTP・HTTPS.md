# HTTP・HTTPS

> [!summary] 一句話
> HTTPS是在HTTP上使用TLS，提供加密、改竄檢知與伺服器認證。

## HTTP／HTTPS

### HTTP（Hypertext Transfer Protocol）

Web瀏覽器與Web伺服器之間傳送資料的通訊協定。

- 通訊內容沒有加密
- 容易遭到竊聽或竄改
- 預設埠號：80

### HTTPS（HTTP over SSL／TLS）

使用SSL／TLS加密HTTP通訊的協定。

- 防止通訊內容被竊聽
- 防止資料被竄改
- 使用數位憑證確認網站身分
- 預設埠號：443

```text
沒有加密的Web通訊
→ HTTP

加密的Web通訊
→ HTTPS
```
