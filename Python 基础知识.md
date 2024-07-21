# 闯关任务:Python实现wordcount
代码实现如下

    import string
      def worldcount(words):
        dicts =  {}
        words = words.lower().translate(str.maketrans('','',string.punctuation))
        word_list = words.strip().split()
        for word in word_list:
          if word in dicts:
            dicts[word] += 1
        else:
            dicts[word] = 1
        return dicts
        print(worldcount(input('请输入:')))

测试输入
    Got this panda plush toy for my daughter's birthday,
    who loves it and takes it everywhere. It's soft and
    super cute, and its face has a friendly look. It's
    a bit small for what I paid though. I think there
    might be other options that are bigger for the
    same price. It arrived a day earlier than expected,
    so I got to play with it myself before I gave it
    to her.

输出
    {'got': 2, 'this': 1, 'panda': 1, 'plush': 1, 'toy': 1, 'for': 3, 'my': 1, 'daughters': 1, 'birthday': 1, 'who': 1, 'loves': 1, 'it': 5, 'and': 3, 'takes': 1, 'everywhere': 1, 'its': 3, 'soft': 1, 'super': 1, 'cute': 1, 'face': 1, 'has': 1, 'a': 3, 'friendly': 1, 'look': 1, 'bit': 1, 'small': 1, 'what': 1, 'i': 4, 'paid': 1, 'though': 1, 'think': 1, 'there': 1, 'might': 1, 'be': 1, 'other': 1, 'options': 1, 'that': 1, 'are': 1, 'bigger': 1, 'the': 1, 'same': 1, 'price': 1, 'arrived': 1, 'day': 1, 'earlier': 1, 'than': 1, 'expected': 1, 'so': 1, 'to': 2, 'play': 1, 'with': 1, 'myself': 1, 'before': 1, 'gave': 1, 'her': 1}
    

# 闯关任务：Vscode连接InternStudio debug笔记
如图进行代码调试

![](图片/调试中.png "图片1")
