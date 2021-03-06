title: 元界区块链测试网
comments: false
---

## 测试网
MVS的测试网(Test Net)是官方提供的，专供用户来开发、调试和测试的。
测试网上面的系统费用是测试网中的 ETP，并非真实的 ETP，测试网的 ETP 可以在官网上免费申请。

测试网的所有区块数据都是独立于主网的。如果开发简单的功能或者尝试注册资产的话，用测试网就足够了，待开发完成后可以迁移到主网上运行。
元界的官网进行了更新，为了方便广大用户体验元界钱包的功能，元界官网<https://mvs.org>新增了”测试节点按钮”。

或直接访问[在线测试网钱包](http://test4.metaverse.live:8820)。

## 测试网的特点
1. 用户不必消耗真正属于他们ETP即可真实体验元界钱包应用场景。
2. 不需同步大量区块，节省时间。
3. 体验资产转移、资产发行、资产增发等功能。
4. 页面性能兼容性强，平台兼容性强。
5. 钱包进程优化，极大减少了对系统资源的占用。
6. 新增多重签名地址的创建、多重签名交易发送模块。
7. 钱包的UI 进一步优化和调整。


## 以测试网模式启动全节点钱包
* 您需要使用您的终端启动钱包。
```bash
mvsd -t
```
* 创建账户
```bash
mvs-cli getnewaccount testaccout testpasswd
```

* 开始CPU挖矿
```bash
mvs-cli start testaccount testpasswd
```
