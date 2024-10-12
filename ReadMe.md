# Security
_Author:Oracle Yuan_

_如果分享，请注明作者并放上链接_

我没有想好这个repo的具体的题目，但我知道，我只是想在这里记录一下我自己对于我想做的安全方向的定义和理解，简单记录一下

--------------------
> LLM就像是电子云，它不太确定，大部分时候集中在一个区域内，而我想做的，就是做一个框，让他无论如何，都被框在这个框里
* 我希望在博士期间，随着我的工作越来越深入，这个框能越来越精确，越来越小
* 但无论如何，我希望它是一个框，而不是另一个电子云
  * 当然啦，我可能也会做一些让LLM这个电子云更靠谱的工作
> 安全并不是提高准确率，更不是让LLM的回答更符合人的期望。安全，是减少最坏事情发生的可能和程度

严格的定义上来说，假设LLM的输出是一个分布，$X$ 

准确率的定义是是$argmax_{P(x)} x=\hat{y}$，即LLM最终的输出等于标准答案

LLM的输出更“好”通常被定义为$ E(x) $的增加，即平均回答质量的增加

但是安全的目标应该是$ \int_{-\infty}^{threshold}xP(x)dx$的减少，即在安全treshold下，减少结果的严重程度，和减少严重结果发生的概率！

> 最安全的是他们能担保，如果出了问题他们能担责
>
> 第二安全的是，他们虽然担不了责，但是能在可能有问题的时候询问用户，我们是否真的要这么做
> 
> 最不安全的是，他们从来不说谁担责，也不问用户该怎么办，但是嘴上一直说自己最安全

如果我做不到最安全的，那么我希望我们至少能做到第二安全