这里面是记录我对Python的学习理解应用---(一) Python 中关于正则表达式re 模块的使用
关于正则表达式 其实就是利用一系列表达式的规则来书写你想要获取的内容 对于正则表达式
是Python基础中比较重要的一个内容，对于字符串的解析很有帮助，可以获取我们需要的信息
下面就介绍下在正则表达式里面re模块的使用：
  1、re.match :用来匹配一串字符串的开头字符
  2、re.search :用于匹配一串字符串中所要寻找的字符
  3、re.
  
 一、search(pattern, string, flags=0)
   pattern :是需要获取内容的正则表达式的公式
   string  :表示需要提取内容所在的字符串
   flags   :表示正则表达式的匹配方式
   
   name="Hello,My name is kuangl,nice to meet you..."
   k=re.search(r'k(uan)gl',name)
   if k:
      print(group(),group(1))
   else:
      print("NOt Found")