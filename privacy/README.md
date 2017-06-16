# 区块链中的隐私保护

一次交易中的隐私信息包括

* 交易发起方地址
* 交易接收方地址
* 交易内容


### 一次性地址

每次交易使用一个临时密钥作为交易地址，从而隐藏真实的交易地址，降低交易之间的关联性。

为了解决临时密钥的管理与分发问题，发展出了利用密钥交换协议派生临时地址的[隐形地址](https://github.com/AlverLyu/kb/blob/master/privacy/stealth.md)技术。

### 账户混合
将多个用户的账户资产混合后重新分配，隐藏实际的交易方。

混合过程使得交易的逻辑复杂化。

https://bitmixer.io/

https://www.mixcoin.us/

https://bitcoin-mix.com/


### 环签名
交易发起方生成的签名需使用一组用户的公钥去验证，从而无法通过签名获知发起方的准确信息。

环签名数据占用的空间较大。

[CryptoNote](https://github.com/cryptonotefoundation/cryptonote)

[monero](https://github.com/monero-project)

### 通道
创建独立于区块链平台的通道/子链，进行私有交易。

[Lightning Network](https://lightning.network)

[Blockstream](https://www.blockstream.com)


### zk-SNARK

[libsnark](https://github.com/scipr-lab/libsnark)

[Zcash](https://z.cash)

#### 同态加密
a*b=c => f(a)·f(b)=f(c)

使用同态加密可以对加密的交易信息进行验证。
