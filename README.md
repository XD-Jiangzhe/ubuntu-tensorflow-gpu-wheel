# ubuntu-tensorflow-gpu-wheel
## 蛋疼的环境 gpu 纯小白开始折腾

1. 折腾了一白天，早上9点-11点半，15点到19点，几乎从0开始搞，实验室装的cuda版本比较鸡肋，9.1，本来以为一个pip3 就搞定了， 结果官网不支持9.1，只有9.0，但是又不能改cuda版本，怎么办呢。。。

2. 于是发现网上有不少轮子，别的大神编译出来的wheel，然后我很高兴，因为可以拿来直接用啊，然后我发现服务器上只有py3.5，没有3.6，这怎么可能难得了我，于是，apt-get 敲起来，然后开始下轮子，一个轮子一两百兆，结果，下好了，pip3 install敲起来，结果，发现实验室 服务器的 显卡的算力只有3.5，别的大神的轮子最少的算力要3.7，被秒杀了，后来发现3.5 的算力比我的笔记本电脑还低。。。1060都6.0的算力了不用说2080ti了，10系的都很高，难怪都 被人拉过去挖矿了。。。

3. 此时的我巨绝望，想了想，要不我自己买一块1060装上自己跑，然后我拆开自己的台式，准备看下主板接口买一块1060插在上面自己跑的时候，又发现了电源只有280w。。。是的你没看错，在这个最低450w电源的年代，竟然还有280w的电源，怕不是从博物馆偷来的吧。。。插块显卡还要换电源，此时的我绝望max

4. 最后，我也不知道从哪里找到了这个网站，https://www.python36.com/install-tensorflow141-gpu/ 然后我照着这个装了bazel,然后编译了不少时间，自己编译了一个wheel，环境：cuda 9.1 cudnn：7.0.5 py 3.5 不用谢我，call me uncle lei !
