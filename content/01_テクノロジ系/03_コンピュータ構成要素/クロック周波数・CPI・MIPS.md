# クロック周波数・CPI・MIPS

> [!summary] 一句話
> CPU 執行時間可由命令數、CPI 與クロック周波数計算；MIPS 表示每秒可執行幾百萬條指令。

## クロック周波数

CPU 每秒產生多少個 Clock。

- 單位：Hz
- 1 MHz＝每秒 100萬 Clock
- 1 GHz＝每秒 10億 Clock
- 數值通常越大，處理速度越快

## CPI

CPI＝Clock Cycles Per Instruction

表示平均執行一條指令需要幾個 Clock。

- CPI 越小越好
- CPI＝2：平均一條指令需要 2 個 Clock

## MIPS

MIPS＝Million Instructions Per Second

表示 CPU 每秒可以執行幾百萬條指令。

- 1 MIPS＝每秒 100萬條指令
- MIPS 越大，通常效能越高

## 公式

每秒指令數：

クロック周波数 ÷ CPI

MIPS：

MIPS ＝ クロック周波数 ÷ CPI ÷ 10⁶

若クロック周波数使用 MHz：

MIPS ＝ クロック周波数（MHz）÷ CPI

## 例題

クロック周波数：100 MHz
CPI：2

100 ÷ 2 ＝ 50 MIPS

答案：每秒執行 5,000 萬條指令。

## 必背關係

クロック周波数
＝一秒有幾個 Clock
＝越大通常越好

CPI
＝一條指令需要幾個 Clock
＝越小越好

MIPS
＝一秒完成幾百萬條指令
＝越大通常越好
