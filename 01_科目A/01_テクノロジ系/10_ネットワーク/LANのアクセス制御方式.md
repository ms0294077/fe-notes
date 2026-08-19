# LANのアクセス制御方式

> [!summary] 一句話
> CSMA/CD 用於傳統有線乙太網路；CSMA/CA 用於無線LAN；トークンパッシング取得權杖後才能傳送。

## CSMA/CD

- **用語：** CSMA/CD（Carrier Sense Multiple Access with Collision Detection）
> 有線LAN使用的方式，先確認線路是否空閒，發生碰撞後再重新傳送。

流程：

```text
確認線路
→ 空閒就傳送
→ 發生碰撞
→ 等待隨機時間
→ 重新傳送
```

重點：

```text
有線LAN
碰撞後處理
```

## CSMA/CA

- **用語：** CSMA/CA（Carrier Sense Multiple Access with Collision Avoidance）
> 無線LAN使用的方式，在傳送前盡量避免碰撞。

重點：

```text
無線LAN
事前避免碰撞
```

## Token Ring

- **用語：** Token Ring（トークンリング）
> 只有取得Token（トークン，令牌）的節點才能傳送資料。

流程：

```text
Token依序傳遞
→ 拿到Token
→ 才能傳送
```

重點：

```text
拿到Token才可傳送
通常為環狀網路
```

## FE快速比較

| 方式 | 使用環境 | 特色 |
|---|---|---|
| CSMA/CD | 有線LAN | 碰撞後等待並重新傳送 |
| CSMA/CA | 無線LAN | 傳送前避免碰撞 |
| Token Ring | 環狀網路 | 取得Token後才能傳送 |

## 快速記法

```text
CD＝Collision Detection
＝碰撞檢測
＝撞了再處理

CA＝Collision Avoidance
＝碰撞避免
＝先避免再傳

Token Ring
＝拿到令牌才傳
```
