# SELECT・WHERE・ORDER BY

> [!summary] 一句話
> SELECT 選欄位、FROM 指定表、WHERE 篩選資料、ORDER BY 排序結果。

## SELECT 基本

```sql
SELECT 列名
FROM 表名
WHERE 条件;
```

作用：

> 從資料表中取得需要的資料。

## 条件指定（WHERE）

用來篩選符合條件的資料。

例：

```sql
SELECT *
FROM 販売データ
WHERE 数量 >= 5;
```

意思：

> 找出「數量5以上」的資料。

## 比較演算子

| 符號 | 意思 |
|-|-|
| = | 等於 |
| <> | 不等於 |
| < | 小於 |
| <= | 小於等於 |
| > | 大於 |
| >= | 大於等於 |

FE重點：

```text
SQL的不等於使用 <>
```

※ `!=` 有些DB可以使用，但 FE 以 `<>` 為標準。

## ORDER BY（並び替え）

排序。

```sql
ORDER BY 列名
```

## ASC

升序（小→大）

```sql
ORDER BY 数量 ASC
```

例：

```
1
5
10
```

## DESC

降序（大→小）

```sql
ORDER BY 数量 DESC
```

例：

```
10
5
1
```

FE重點：

```text
ASC = 昇順
DESC = 降順
```
