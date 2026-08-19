# SQL・DDL・DML

> [!summary] 一句話
> DDL 定義資料庫結構；DML 查詢或更新資料；DCL 控制權限與交易。

## SQLとは

**SQL（Structured Query Language）**：

> 資料庫操作使用的語言。

可以用來：

- 建立資料表
- 查詢資料
- 新增、修改、刪除資料

## DDL

- **用語：** DDL（Data Definition Language，資料定義語言）
> 用來操作資料庫或資料表的結構。

| 指令 | 意思 |
|---|---|
| CREATE | 建立資料表 |
| ALTER | 修改資料表結構 |
| TRUNCATE | 清空表內全部資料，保留表 |
| DROP | 刪除整張表，連結構一起刪除 |

## DML

- **用語：** DML（Data Manipulation Language，資料操作語言）
> 用來操作資料表中的資料。

| 指令 | 意思 |
|---|---|
| SELECT | 查詢資料 |
| INSERT | 新增資料 |
| UPDATE | 修改資料 |
| DELETE | 刪除資料 |

## DELETE・TRUNCATE・DROP的差別

| 指令 | 資料 | 表結構 |
|---|---|---|
| DELETE | 刪除指定或全部資料 | 保留 |
| TRUNCATE | 全部清空 | 保留 |
| DROP | 全部刪除 | 也刪除 |

## FE考點

```text
DDL＝操作資料表結構
CREATE・ALTER・TRUNCATE・DROP

DML＝操作表內資料
SELECT・INSERT・UPDATE・DELETE
```

## 關鍵詞

| 日文     | 讀音     | 英文       | 中文解釋 |
| ------ | ------ | -------- | ---- |
| データベース | でーたべーす | Database | 資料庫  |
| テーブル   | てーぶる   | Table    | 資料表  |
| レコード   | れこーど   | Record   | 一筆資料 |
