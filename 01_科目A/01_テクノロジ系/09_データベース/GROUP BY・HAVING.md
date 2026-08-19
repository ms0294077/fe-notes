# GROUP BY・HAVING

> [!summary] 一句話
> GROUP BY進行分組；WHERE在分組前篩選資料列，HAVING在分組後篩選群組。

## 基本形

SELECT 部門, COUNT(*)
FROM 社員
WHERE 在籍中 = 1
GROUP BY 部門
HAVING COUNT(*) >= 5
ORDER BY COUNT(*) DESC;

## 各句作用

| 句 | 作用 |
|---|---|
| WHERE | 分組前刪除不需要的資料列 |
| GROUP BY | 把相同值的資料列組成群組 |
| HAVING | 對集計後的群組設定條件 |
| ORDER BY | 對最終結果排序 |

## SQL的論理處理順序

1. FROM
2. WHERE
3. GROUP BY
4. HAVING
5. SELECT
6. ORDER BY

這是理解用的論理順序，不代表DB內部一定照此實作。

## WHERE與HAVING

- 年齡大於20：資料列條件，使用WHERE
- 部門平均年齡大於30：集計後條件，使用HAVING

能在WHERE完成的條件通常應先在WHERE篩選，以減少後續分組資料量。

## GROUP BY的規則

SELECT中出現的非集計欄位，一般必須包含在GROUP BY中。

正確例：

SELECT 部門, AVG(給与)
FROM 社員
GROUP BY 部門;

## FE考點

- 集計前條件：WHERE
- 集計後條件：HAVING
- 群組欄位：GROUP BY
- 結果排序：ORDER BY
- COUNT(*)計算資料列；COUNT(欄位)通常忽略NULL

## 易錯點

- HAVING不是WHERE的替代品
- GROUP BY不保證排序
- SQL方言與設定可能有差異，考題通常依標準概念判斷

## 快速記憶

> WHERE先篩人，GROUP BY分組，HAVING再篩組。
