---
title: 以太坊 Web3.js 开发基础
date: 2019-01-19 16:19:24
tags:
 - web3js
categories:
 - 区块链
---
简介
web3.js 是一个通过RPC 调用 和本地以太坊节点进行通信的js库。web3.js可以与任何暴露了RPC接口的以太坊节点连接。
web3中提供了eth对象 - web3.eth来与以太坊区块链进行交互。
<!--more--> 
在github上获得代码
安装 Testrpc
安装Ethereum客户端来支持JSON RPC API调用开发环境，推荐使用EthereumJS。
安装命令：
sudo npm install -g ethereumjs-testrpc

启动 testrpc
在命令行执行
testrpc
EthereumJS TestRPC v6.0.3 (ganache-core: 2.0.2)

Available Accounts
==================
(0) 0x1abb473c627e690c048dbf7a9f9cc54b25dea42a
(1) 0xd50fadba656c8f78916f9c1a1b78fd3d35dad0aa
(2) 0x69e0159cf8e6fc81e8e71479aea0e8984d7daf48
(3) 0x5f1ebce982445a02ff4530f4d53cd09cb2a6addf
(4) 0x746f6a0192cf42001ded53a55932a6dff754e143
(5) 0x685dcca08e5efc905a300eff68bf2e8a81989966
(6) 0x08eed3a1a801be6af543105cb9bfc27b6401c020
(7) 0xc8fd99bde94fbfab654c8cffda6047b16306cc07
(8) 0xc28e0b677883f809faa1eaf563a5f4b794dcbaeb
(9) 0xd02b16bbaa70b2cba4ea173009f2fdf829a8ffba

Private Keys
==================
(0) d233ec4635ed0fe5c61977c9442d6233c599cd3591107b9a017f7ea6077da3bc
(1) a02a88b2c04aed72b55cdd6f6212e1f560dd02767f0a03627fac97b64b64086d
(2) 833dd28ab15388ba162862c365313978dabb96d209c311bca7d9a7bfdb2ecb6f
(3) 47c7ae2635fed1b4f5e442496fd364cdaa91ae6e950b45f36aa4ac6c172cffb5
(4) 4b8ee2ee44eab299cbeff51bbf6fb74572e493409556e728a385dcf9e4dc4f84
(5) 50cdb8a14babddcbb79f14ad7b5cc55e95a0b8ce72659eec1c9b8d798ff52369
(6) becc6dd7a41564aaf3f2f1711eb102032ace0c4e4b561fc7c922ea92f1a81c5a
(7) cc82c2ad095b32bd23e33bc9c3ef6b69ad8b76de07a9e02714760d2fd843efa5
(8) 44f9c35f62ffe1aa3b85bb6e557569beb396ced7d5ab8a75345d9a8ab1283bca
(9) 3d7ec84ed3253366f744a754ccdc2187d65856c2b264e9fbd651c59896aac229

HD Wallet
==================
Mnemonic:      tilt oyster obtain car venture party power exclude fire price senior blue
Base HD Path:  m/44'/60'/0'/0/{account_index}

Listening on localhost:8545

会自动创建10个账户，每个账户默认有100个以太币。
安装和和获取web3对象
安装
npm: npm install web3
bower: bower install web3
metor: meteor add ethereum:web3
vanilla: dist./web3.min.js
获得web3实例
if (typeof web3 !== 'undefined') {
  web3 = new Web3(web3.currentProvider);
} else {
  // set the provider you want from Web3.providers
  web3 = new Web3(new Web3.providers.HttpProvider("http://localhost:8545"));
}

使用实例
一、账户操作：
获取账户
web3.eth.getAccounts(function(error, result){
        res.send(result)
  })

创建新账户
web3.eth.accounts.create();
> {
    address: "0xb8CE9ab6943e0eCED004cDe8e3bBed6568B2Fa01",
    privateKey: "0x348ce564d427a3311b6536bbcff9390d69395b06ed6c486954e971d960fe8709",
    signTransaction: function(tx){...},
    sign: function(data){...},
    encrypt: function(password){...}
}

web3.eth.accounts.create('2435@#@#@±±±±!!!!678543213456764321§34567543213456785432134567');
> {
    address: "0xF2CD2AA0c7926743B1D4310b2BC984a0a453c3d4",
    privateKey: "0xd7325de5c2c1cf0009fac77d3d04a9c004b038883446b065871bc3e831dcd098",
    signTransaction: function(tx){...},
    sign: function(data){...},
    encrypt: function(password){...}
}

web3.eth.accounts.create(web3.utils.randomHex(32));
> {
    address: "0xe78150FaCD36E8EB00291e251424a0515AA1FF05",
    privateKey: "0xcc505ee6067fba3f6fc2050643379e190e087aeffe5d958ab9f2f3ed3800fa4e",
    signTransaction: function(tx){...},
    sign: function(data){...},
    encrypt: function(password){...}
}

使用私钥创建账户
web3.eth.accounts.privateKeyToAccount(privateKey);
web3.eth.accounts.privateKeyToAccount('0x348ce564d427a3311b6536bbcff9390d69395b06ed6c486954e971d960fe8709');
> {
    address: '0xb8CE9ab6943e0eCED004cDe8e3bBed6568B2Fa01',
    privateKey: '0x348ce564d427a3311b6536bbcff9390d69395b06ed6c486954e971d960fe8709',
    signTransaction: function(tx){...},
    sign: function(data){...},
    encrypt: function(password){...}
}

web3.eth.accounts.privateKeyToAccount('0x348ce564d427a3311b6536bbcff9390d69395b06ed6c486954e971d960fe8709');
> {
    address: '0xb8CE9ab6943e0eCED004cDe8e3bBed6568B2Fa01',
    privateKey: '0x348ce564d427a3311b6536bbcff9390d69395b06ed6c486954e971d960fe8709',
    signTransaction: function(tx){...},
    sign: function(data){...},
    encrypt: function(password){...}
}

使用私钥签名一个交易
web3.eth.accounts.signTransaction(tx, privateKey [, callback]);
web3.eth.accounts.signTransaction({
    to: '0xF0109fC8DF283027b6285cc889F5aA624EaC1F55',
    value: '1000000000',
    gas: 2000000
}, '0x4c0883a69102937d6231471b5dbb6204fe5129617082792ae468d01a3f362318')
.then(console.log);
> {
    messageHash: '0x88cfbd7e51c7a40540b233cf68b62ad1df3e92462f1c6018d6d67eae0f3b08f5',
    v: '0x25',
    r: '0xc9cf86333bcb065d140032ecaab5d9281bde80f21b9687b3e94161de42d51895',
    s: '0x727a108a0b8d101465414033c3f705a9c7b826e596766046ee1183dbc8aeaa68',
    rawTransaction: '0xf869808504e3b29200831e848094f0109fc8df283027b6285cc889f5aa624eac1f55843b9aca008025a0c9cf86333bcb065d140032ecaab5d9281bde80f21b9687b3e94161de42d51895a0727a108a0b8d101465414033c3f705a9c7b826e596766046ee1183dbc8aeaa68'
}

web3.eth.accounts.signTransaction({
    to: '0xF0109fC8DF283027b6285cc889F5aA624EaC1F55',
    value: '1000000000',
    gas: 2000000,
    gasPrice: '234567897654321',
    nonce: 0,
    chainId: 1
}, '0x4c0883a69102937d6231471b5dbb6204fe5129617082792ae468d01a3f362318')
.then(console.log);
> {
    messageHash: '0x6893a6ee8df79b0f5d64a180cd1ef35d030f3e296a5361cf04d02ce720d32ec5',
    r: '0x9ebb6ca057a0535d6186462bc0b465b561c94a295bdb0621fc19208ab149a9c',
    s: '0x440ffd775ce91a833ab410777204d5341a6f9fa91216a6f3ee2c051fea6a0428',
    v: '0x25',
    rawTransaction: '0xf86a8086d55698372431831e848094f0109fc8df283027b6285cc889f5aa624eac1f55843b9aca008025a009ebb6ca057a0535d6186462bc0b465b561c94a295bdb0621fc19208ab149a9ca0440ffd775ce91a833ab410777204d5341a6f9fa91216a6f3ee2c051fea6a0428'
}

哈希一个消息
web3.eth.accounts.hashMessage(message);
web3.eth.accounts.hashMessage("Hello World")
> "0xa1de988600a42c4b4ab089b619297c17d53cffae5d5120d82d8a92d0bb3b78f2"

// the below results in the same hash
web3.eth.accounts.hashMessage(web3.utils.utf8ToHex("Hello World"))
> "0xa1de988600a42c4b4ab089b619297c17d53cffae5d5120d82d8a92d0bb3b78f2"

sign 给任意一个内容使用私钥签名
web3.eth.accounts.sign(data, privateKey);
web3.eth.accounts.sign('Some data', '0x4c0883a69102937d6231471b5dbb6204fe5129617082792ae468d01a3f362318');
> {
    message: 'Some data',
    messageHash: '0x1da44b586eb0729ff70a73c326926f6ed5a25f5b056e7f47fbc6e58d86871655',
    v: '0x1c',
    r: '0xb91467e570a6466aa9e9876cbcd013baba02900b8979d43fe208a4a4f339f5fd',
    s: '0x6007e74cd82e037b800186422fc2da167c747ef045e5d18a5f5d4300f8e1a029',
    signature: '0xb91467e570a6466aa9e9876cbcd013baba02900b8979d43fe208a4a4f339f5fd6007e74cd82e037b800186422fc2da167c747ef045e5d18a5f5d4300f8e1a0291c'
}

使用web3.eth.personal 新建账户
web3.eth.personal.newAccount(password, [callback])
web3.eth.personal.newAccount('!@superpassword')
.then(console.log);
> '0x1234567891011121314151617181920212223456'

获得账户余额
web3.eth.getBalance('0xe70c4835b29e2fd35bd3f60c0a76413f70f17115').then(function(balance){
     console.log('balance:',balance)
     balance = new BigNumber(balance)
     console.log('balance:',balance)
})

这里使用了BigNumber.js 处理余额显示，参考我另一片博文。
utils工具函数
web3.utils.toHex   将任何值转为HEX 16进制
String|Number|Object|Array|BigNumber - 需要转化为HEX的值。如果是一个对象或数组类型，将会先用JSON.stringify1进行转换成字符串。如果传入的是BigNumber2，则将得到对应的Number的HEX
var str = "abcABC";
var obj = {abc: 'ABC'};
var bignumber = new BigNumber('12345678901234567890');

var hstr = web3.utils.toHex(str);
var hobj = web3.utils.toHex(obj);
var hbg = web3.utils.toHex(bignumber);

console.log("Hex of Sring:" + hstr);
console.log("Hex of Object:" + hobj);
console.log("Hex of BigNumber:" + hbg);

web3.utils.isHex(hex) 判断输入是不是16进制
web3.utils.isHex('0xc1912');

判断输入是不是一个地址
web3.utils.isAddress('0xc1912fee45d61c87cc5ea59dae31190fffff232d');

把金额单位换成wei
web3.utils.toWei(number [, unit])
web3.utils.toWei('1', 'ether');
> "1000000000000000000"

web3.utils.toWei('1', 'finney');
> "1000000000000000"

web3.utils.toWei('1', 'szabo');
> "1000000000000"

web3.utils.toWei('1', 'shannon');
/> "1000000000"

把单位为wei的以太币换成 ether
web3.utils.fromWei(number [, unit])
web3.utils.fromWei('1', 'ether');
> "0.000000000000000001"

web3.utils.fromWei('1', 'finney');
> "0.000000000000001"

web3.utils.fromWei('1', 'szabo');
> "0.000000000001"

web3.utils.fromWei('1', 'shannon');
> "0.000000001"

判断给定的数据是否是 BigNumber
web3.utils.isBigNumber(bignumber)
var number = new BigNumber(10);
web3.utils.isBigNumber(number);

sha3算法
// web3.utils.sha3(string)
// web3.utils.keccak256(string) // ALIAS
web3.utils.sha3('234'); // taken as string
> "0xc1912fee45d61c87cc5ea59dae311904cd86b84fee17cc96966216f811ce6a79"

web3.utils.sha3(new BN('234'));
> "0xbc36789e7a1e281436464229828f817d6612f7b477d66591ff96a9e064bcc98a"

web3.utils.sha3(234);
> null // can't calculate the has of a number

web3.utils.sha3(0xea); // same as above, just the HEX representation of the number
> null

web3.utils.sha3('0xea'); // will be converted to a byte array first, and then hashed
> "0x2f20677459120677484f7104c76deb6846a2c071f9b3152c103bb12cd54d1a4a"

[在github上获得代码] https://github.com/cooleye/web3tutorial

作者：孔德健
链接：https://www.jianshu.com/p/f3f36447546e
來源：简书
简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。