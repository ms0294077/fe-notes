# グローバルIP・プライベートIP・NAT・NAPT

> [!summary] 一句話
> NAT轉換IP位址；NAPT再利用連接埠讓多台主機共用一個全球IP。

## グローバルIPとプライベートIP

### グローバルIPアドレス

> Internet上使用的公有IP，全世界不能重複。

### プライベートIPアドレス

> LAN內使用的私有IP，不同LAN可以重複。

例如：

192.168.x.x

## NATとNAPT

### NAT

- **用語：** NAT（Network Address Translation）
> 將私有IP轉換成公有IP。

基本上是：

1個私有IP
↔
1個公有IP

### NAPT／IPマスカレード

- **用語：** NAPT（Network Address and Port Translation）
> 多個私有IP利用不同的Port，共用一個公有IP。

多個私有IP
↔
1個公有IP

家用Router通常使用NAPT。
