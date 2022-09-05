# zhuiwuxinzhiyimeng.github.io
抓包
1.只抓包头
一般能抓到的每个包（称为“帧”更准确，但是出于表达习惯，本书可能会经常用“包”代替“帧”和“分段”）的最大长度为1514字节，启用了Jumbo Frame（巨型帧）之后可达9000字节以上，而大多数时候我们只需要IP头或者TCP头就足够分析了。在Wireshark上可以这样抓到包头。

新版本的wireshark（2.x以后）的Options对话框变化比较大，限制单包的方法是：捕获->选项，找到要抓包的接口，选中它，找到列表标题中的捕获长度(B)，单击对应栏，发现变为可输出状态，在这里输入限制的单包大小即可（同旧版本的Limi each packet to）"Limit each packet to"的值。
