# 区块链python模拟教程
* 源代码是基于 <Mastering Bitcoin 2nd>  https://github.com/dvf/blockchain  https://github.com/adilmoujahid/blockchain-python-tutorial 上的改进.

## 注意: 此工程只可用于教学，不可商用，因为它没有很好的安全性和扩展性，也缺乏很多区块链的重要特性。


<div style="display:block;margin:auto;height:80%;width:80%">
  <img src="blockchain-simulation.gif">
</div>

该repo 采用python实现了一个基本的区块链及客户端，它拥有以下特性：

- 可以在区块链中增加多个节点
- Proof of Work (PoW)
- 节点间的简单冲突处理
- RSA加密的Transaction

区块链客户端拥有以下特性:

- 采用加密 Public/Private key生成钱包(基于RSA算法)
- 采用RSA加密生成Transactions

该repo也包含了两个dashboards: 

- 供挖矿的"Blockchain Frontend"  
- 供用户生成钱包和发送币的"Blockchain Client" 


# 依赖库

- ```Python 3.6``` 环境
- pip install -r requirements.txt
- 也可以用[Anaconda's Python distribution](https://www.continuum.io/downloads) 

# 怎么运行

1. 开启一个区块链结点, 进入 ```blockchain``` 目录，执行以下命令 :
```python blockchain.py -p 5000```
2. 你也可以增加一个节点，指定不同的端口号. 比如 ```python blockchain.py -p 5001```
3. 开启区块链客户端, 进入 ```blockchain_client``` 目录，执行以下命令:
```python blockchain_client.py -p 8080```
4. 现在你可以通过localhost:5000 访问区块链，通过localhost:8080访问客户端

