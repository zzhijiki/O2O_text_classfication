# README

这是一个文本分类练习赛 https://www.datafountain.cn/competitions/370

- rank：156/3592

- 构建 TF-IDF + Bigram的语言模型和SVM的分类模型，利用beyes-optimization寻找分类器最优超参数（baseline：0.88）。里面的dict是我偷过来的，应该用文件造一个dict，这里做的不太好，当然也会造成很多未登录词的问题，所以暂且就不改了。
- 构建paddle框架的Ernie语义模型。（score：0.932）里面包括很多自定义reader ，定义配置这种很烦很复杂的操作，静态图实在是用不来啊，不过还好被我调出来了。
- 也尝试利用LSTM 和TEXTCNN，但是paddle的静态图对我难度过大，我最后还是放弃了。
- 那段时间还没买新电脑，所以没有用pytorch，旧电脑显卡不行，负重练习。

## 2020-04-07更新

- 更新了word2vec两种naive（就是没有用trick的）的实现，但是我觉得skipgram可能写错了，应该用多标签BCEloss可能会好点

- 更新了word2vec的negative sampling for skipgram

- 更新了用word2vec 作为word represetation 来完成这个O2O文本分类任务的几个简易demo

  语料库是小型语料库，不足挂齿

- textcnn和lstm还没完成，下次更新

