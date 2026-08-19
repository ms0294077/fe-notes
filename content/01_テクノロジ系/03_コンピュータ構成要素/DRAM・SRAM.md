# DRAM・SRAM
> [!summary] 一句話
> DRAM 需要刷新、容量大且便宜，用於主記憶；SRAM 不需刷新、速度快且昂貴，用於キャッシュ。

## DRAM（Dynamic RAM）

- 使用：コンデンサ（電容）
- 電容會漏電，因此需要定期 Refresh
- 集積度高，可以製作大容量記憶體
- 價格便宜
- 速度較慢
- 主要用途：主記憶體

例：
- DDR4
- DDR5
- LPDDR

## SRAM（Static RAM）

- 使用：フリップフロップ回路
- 只要有供電就能保持資料，不需要 Refresh
- 集積度低，容量較小
- 價格昂貴
- 速度快
- 主要用途：Cache Memory

例：
- L1 Cache
- L2 Cache
- L3 Cache

## 比較

| 項目 | DRAM | SRAM |
|---|---|---|
| 電路 | コンデンサ | フリップフロップ |
| Refresh | 需要 | 不需要 |
| 集積度 | 高 | 低 |
| 價格 | 便宜 | 昂貴 |
| 速度 | 慢 | 快 |
| 用途 | 主記憶體 | Cache Memory |

## FE 記憶口訣

DRAM：便宜、容量大、較慢、要 Refresh、用於主記憶體。
SRAM：昂貴、容量小、較快、不用 Refresh、用於 Cache。
