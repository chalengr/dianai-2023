学习理解了mha，mqa，gqa
多头注意力就是把qkv分成head份，每一份与每一份对应相乘
![image](https://github.com/chalengr/dianai-2023/assets/92655725/a8d8f7c6-0f3c-4a25-b501-69b33cbcc3ef)
写MHA的时候一开始先去看了源码https://github.com/google-research/bert/blob/master/modeling.py

没看懂但是后来我个人的理解就是一个embed size的linear可以相当于训练了head块矩阵，加快效率

MQA和MHA的区别就是k,v现在都一样，只有query分多个头

了解了pytorch的广播机制可以维度匹配
