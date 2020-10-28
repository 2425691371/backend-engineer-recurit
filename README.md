# 双链科技java后台工程师招聘

因为业务发展需要，双链科技正在招聘工程师。但每天收到大量内容非常相似的简历，简历筛选让我们头痛不已，而软件工程师还是要靠代码说话的，所以不如看代码直接一些。


请完成下列函数，从一个List中取得最大整型值：

```java

pulic static Integer getMaxValue(List valueList){
    return  null;
}

```

## 要求：

* Java 8可编译通过并运行
* 把您这样做的原因写下来
* **严谨**! **严谨**! **严谨**! 设想这段代码需要在航天器上运行

## 提示：
* 这是一个公用函数，请考虑这个函数的安全性，健壮性，在小规模数据量下10000条的性能；
* 不要使用Collections.max等函数来实现
* 函数命名对于长期维护非常重要，就像希腊语之于数学，英语是计算机的母语，故请使用美式英语命名变量；
* 本考题看似简单，但是考到的知识点非常多，我们需要基础知识扎实并且严谨的软件工程师；
* 请在**一个小时内完成**本函数，不同水平的程序员做到的程度会不一样，这很正常；
* 您可以fork本项目，在您自己的github账号的本页面完成，您的答案属于您；
* 完成之后，请使用您在github的账号邮箱（可能您需要把该邮箱设置为公开)发送通知到 zhangxilai#doublechaintech.com，通知中请包含你的github repo地址和您的答案(方便我查看）
* 可以封装额外的函数
* 错误消息友好

## 邮件要求

* 邮件标题中格式如下  渠道-Java工程师-姓名
* 函数实现直接写到邮件正文中，**不要**使用附件来写答案，也**不要**发送链接，以便于在移动环境中查看
* 您这么做的理由

```
//在您自己的READ.md中，答案写到下面的位置

public static void main(String[] args) {
        List li=new ArrayList<>();
        li.add(1);
        li.add("牛奶");
        li.add(1.234);
        li.add('a');
        li.add(true);
        li.add(1);
        li.add(132423);
        li.add(1);
        li.add(143534532);
        System.out.println(li);
        List<Integer> res = new ArrayList<>();
        for (int i = 0; i < li.size(); i++) {
            if(li.get(i) instanceof Integer){
                res.add((Integer) li.get(i));
            }
        }
        Object[] array = res.toArray();
        Arrays.sort(array);
        System.out.println(array[array.length-1]);

//这样做的原因写到下面

答：原因是根据需求是从一个List中取得最大整型值，首先判断运用了List容器，就会用到对应的方法及函数，其次题中并未提及List容器中存储什么类型的数据，所以需要判断并筛选符合整数类型的值存入新的List容器中，再根据Java类库的对应工具类及方法将其进行排序处理，最终取出最大值。
```
