# Webアプリケーション攻撃

> [!summary] 一句話
> XSS攻擊瀏覽器端，SQLインジェクション攻擊DB，OSコマンドインジェクション攻擊OS，ディレクトリトラバーサル越權讀檔。

## 攻擊比較

| 攻擊 | 攻擊目標 | 典型結果 | 主要防禦 |
|---|---|---|---|
| XSS | 瀏覽器中的頁面 | 執行惡意script、竊取session | 輸出時escape、CSP |
| SQLインジェクション | SQL查詢 | 竊取或竄改DB | プレースホルダ／prepared statement |
| OSコマンドインジェクション | OS命令 | 執行任意command | 不拼接命令、限制輸入 |
| ディレクトリトラバーサル | 檔案路徑 | 讀取公開目錄外的檔案 | 固定base path、驗證canonical path |
| ディレクトリリスティング | Web server設定 | 顯示目錄中的檔案清單 | 關閉directory listing |

## XSS

攻擊者把script混入Web內容，由其他使用者的瀏覽器執行。

常見關鍵詞：

- 未轉義的輸出
- cookie或session被竊
- 掲示板、コメント欄

核心對策是根據輸出位置進行適當escape，而不是只在輸入時刪除特定字元。

## SQLインジェクション

把輸入直接拼接到SQL，使查詢意義被改變。

核心對策：

- 使用prepared statement／bind variable
- DB帳號採最小權限
- 不把詳細錯誤直接回傳使用者

## OSコマンドインジェクション

輸入被當成shell命令的一部分執行。優先避免呼叫shell；不得已時使用安全API與嚴格allow list。

## ディレクトリトラバーサル

利用 ../ 等路徑跳出預定目錄。只檢查字串不足，應確認正規化後的實際路徑仍在允許範圍內。

## FE考點

- 瀏覽器執行script：XSS
- SQL語句被改寫：SQLインジェクション
- shell命令被執行：OSコマンドインジェクション
- ../ 讀取任意檔案：ディレクトリトラバーサル
- 單純顯示檔案列表：ディレクトリリスティング

## 易錯點

- WAF可降低風險，但不能代替程式本身的安全實作
- HTML escape不能防止SQL injection
- 對策必須配合資料進入的語境

## 快速記憶

> Script看XSS、SQL看DB、command看OS、../看path。
