计算机181 张志坤 2018310741

# java的字符串的处理和应用，以及抛出异常。


## 一、实验目的 
掌握字符串String及其方法的使用，提供用户查询《长恨歌》中的字符的功能，同时返回给用户所查询的字符出现的次数。 掌握异常处理结构，抛出用户输入的空字符引用异常。

## 二、实验要求
利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能函数，并运行。达到如下功能：

1.每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。” 

2.允许提供输入参数，统计古诗中某个字或词出现的次数 3.考虑操作中可能出现的异常，在程序中设计异常处理程序。

3.考虑操作中可能出现的异常，在程序中设计异常处理程序。

输入：汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸一笑百媚生六宫粉黛无颜色春寒赐浴华清池温泉水滑洗凝脂侍儿扶起娇无力始是新承恩泽时云鬓花颜金步摇芙蓉帐暖度春宵春宵苦短日高起从此君王不早朝承欢侍宴无闲暇春从春游夜专夜后宫佳丽三千人三千宠爱在一身金屋妆成娇侍夜玉楼宴罢醉和春姊妹弟兄皆列士可怜光采生门户遂令天下父母心不重生男重生女骊宫高处入青云仙乐风飘处处闻缓歌慢舞凝丝竹尽日君王看不足渔阳鼙鼓动地来惊破霓裳羽衣曲九重城阙烟尘生千乘万骑西南行<未完，待续>

输出：
汉皇重色思倾国，御宇多年求不得。
杨家有女初长成，养在深闺人未识。
天生丽质难自弃，一朝选在君王侧。
回眸一笑百媚生，六宫粉黛无颜色。
春寒赐浴华清池，温泉水滑洗凝脂。
侍儿扶起娇无力，始是新承恩泽时。
云鬓花颜金步摇，芙蓉帐暖度春宵。
春宵苦短日高起，从此君王不早朝。
…………

## 三、实验过程:
首先创造一个Chg的类，首先建立String和Stringbuffer用来对字符串处理。运用insert和equal进行对字符串特定位置的添加标点符号。再用String Tokenizer字符分析器来进行对某个字符的查找。查找过程为，通过用户输入的字符来将字符串分段，运用countToken来进行对分段的计数。如果字符在中间的话那么有一个字符的话，计数就为2.这时减一即可。如果在开头和结尾的话，那么久通过if来确定用户输入的字符，如果是在开头和结尾，那么次数不减一。
新建一个类来作为测试类。再建一个Yc的类来定义自己的异常，用来处理用户输入的空字符。

## 四、流程图：[image text](https://github.com/zhangqieyan/-/blob/master/%E9%95%BF%E6%81%A8%E6%AD%8C.png)

## 五、核心代码注释：
int last = s.length();//last代表的是字符串s的长度
 s.insert(i,'。');//在i出插入句号
  StringTokenizer a = new StringTokenizer(d,c);//建立一个字符分析器，
   while(a.hasMoreTokens()) //查看a字符串里还有没有字符串c中的字符
    String k = a.nextToken();//对a这个字符串进行c的分割
    countToken//来计数nextToken用了几次。
    throw new Yc("不能输入空字符");//抛出异常不能输入空字符
    e.printStackTrace();//出现的异常

## 六、运行截图 [image text](https://github.com/zhangqieyan/-/blob/master/1a3ecf31077006e4388eff0e01b01a0.png)
[image text](https://github.com/zhangqieyan/-/blob/master/1eaa2bea26c4c50e3959ce4b4e7ea45.png)
## 七、编程感想：
了解了处理字符串的方法和如何在字符串中进行查找字符。了解了自定义异常的处理。学习到了如何在书中寻找自己不会用的东西来学以致用。
