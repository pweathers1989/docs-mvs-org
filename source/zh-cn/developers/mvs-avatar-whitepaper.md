title: 元界数字身份白皮书(简版)
comments: false
---

## 数字身份的本质
  元界的数字身份是独特的，身份识别模块将被内置于协议中，并开发有辅助支持它的应用程序。用户具有确定的自主身份，即用户可以完全控制自己的身份，这就意味着不必依赖中央实体或第三方进行身份验证。用户拥有真正意义上的自主身份，可以创建、签署、验证，同时与用户进行交互的人也能够证明其身份。此外，这些拥有自主数字身份的用户能够选择性地披露他们的信息。 数字身份是虚拟世界不可分割的一部分。就其本身而言，数字身份可以采取任一形式，如个人或价值中介（机构和实体）。 因此，个人在不同的场所可以拥有不同的数字身份，如职场身份和家庭身份，但这些最终都是以用户的现实身份为基础。 
  用户可以通过数字身份在元界建立自己的声誉，同时这也会改进我们交换价值的方式。它可以通过数字签名、验证要求和交易来实现这一目的，并逐步树立起可以被市场上其他数字身份和价值中介检查和验证的声誉基础。对于一些中心化实体，如果他们的服务器崩溃，那么它们多年树立的身份和声誉将永远消失。元界则不同，用户的数字身份及其声誉将受到区块链的保护。

## 适用案例
  在区块链协议中嵌入一个身份系统，这样的适用案例有很多。
拥有许多不同的数字身份，例如一个数字身份可以向乙银行说明某用户已经在甲银行开设了帐户，正由于此，乙银行将授权用户开立一个银行帐户，理由是该用户已经在甲银行开设了一个帐户。在同一法律管辖内，这一案例可以在银行间进行复制。 
除此之外，数字身份也适用于数字版权等领域，终端用户将能够使用他们的数字身份来声明版权或其他资产，除了授权他们的认证信息外，用户也能够授权他人访问私有数据如声誉、信用等数据。

## 数字身份的操作流程
* **创建**
  任何用户都可以创建数字身份，并与自己的主私钥绑定。
  如果用户创建完数字身份，并未绑定任何主私钥，那么该DID相当于一个未经认证的账号，无法使用数字身份的任何功能与应用。
已在元界区块链上登记资产的主私钥持有者也可以选择不关联绑定任何数字身份，这是一个主动的过程，元界不会为用户自动创建数字身份，数字身份的关联权掌握在主私钥持有者手中。

* **验证**
  Profile能够提供有效的证明链，该证明链能够提供该数字身份下的客观事实。对于用户来说，首先需要证明的即该数字身份属于我：通过把交易绑定到DID上即可（交易域包含DID信息）。

* **授权**
  首先需要弄清楚授权的场景，授权往往是和交易相关的。授权过程往往是伴随着下述场景的：假设A请求B的数字身份信息：资产信息。目的是核对B的资产，然后才能提供服务。这样会出现两种可能：
第一种是B的链上资产非常多，ETP有100万个，那么B在收到请求时，直接授权ETP资产信息给A即可。
第二种是B的链上资产不多，但是链下资产比较多，传统的做法是B需要将资产转换成ETP进行授权，目前元界推荐的做法是发行自己的资产，并让Oracle对资产进行证明，这之后该资产也作为有效资产进入数字身份的信息中。
-   授权过程：
A向B发送一个验证资产的请求，该请求触发一个脚本，脚本去验证目标账户的资产信息，随后返回一个结果，该结果是A加密的结果，B并不知道哪个结果是对应验证通过的信息。并且请求也是一个加密信息，B并不知道A的具体请求，但是知道请求哪一项信息。而对于个人交易记录、资产记录，只需链上进行授权访问，原理相同。
    对于个人自定义字段，与资产的Oracle证明类似，（没有经过Oracle认证的字段信息也可以授权，但是不推荐）。
如果个人定义的字段是非公示信息，比方说邮箱手机号，则无需进行Oracle认证，如果是证明类信息如学历证明，则需要Oracle认证。
-   认证过程：
    *个人自定义信息认证*
    使用Oracle Data-feed进行背书。引入第三方Oracle, 该Oracle在链上公示所有Profile，供公众查询监督，并且Oracle通常是机构，机构也应当在官网公示自己的Profile和DID信息。
    B首先在自定义字段处填写需要证明的信息，Oracle需要使用自己的主私钥匙对其签名，并动用一个比较大额的币天对该字段进行背书。
    A可在链上请求该字段的信息，包含Oracle背书信息，则A可认为B的信息有效，A可继续对B提供服务。

* **查询**
由于数字身份一开始已经引进DID标识的概念，因此，可以把DID标识作为在场外交易的主体，具备在交易市场中创建交易的功能。
通过在交易市场中的地址查询栏中输入DID，我们可以查询到该DID正在发布哪些交易请求，以及公开市场中的历史交易记录。反过来，某一DID在市场上的交易行为和记录，同样可以用作构建数字身份的数据。

