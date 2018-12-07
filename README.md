# JavaAssistCglibJdkTree
jdk,JavaAssist,Cglib动态代理技术研究


![](https://i.imgur.com/A52Ya8P.png)

<pre>
代理：
        代理是一种常用的设计模式，其目的就是为其它对象提供一个代理以控制对某个对象的访问。
     代理类负责为委托类预处理消息，过滤消息并转发消息。

        为了保持行为的一致性，代理类和委托类通常会实现相同的接口。通过代理类这中间这一层，能
     有效控制对委托类对象的直接访问，可以很好的隐藏和保护委托类对象，同时也为实施不同控制
     策略预留了空间，从而在设计上获得更大的灵活性。
</pre>

<pre>
静态代理：
     在编译期确定代理对象；

     缺点：
         1）代理类和委托类实现了相同的接口，代理类通过委托类实现了相同的方法。这样就出现了
            大量的代码重复。如果接口增加一个方法，除了所有实现类需要实现这个方法外，所有代
            理类也需要定义这个接口，增加了代码维护的复杂性。
         2）代理对象只服务于一种类型的对象，如果要服务于多类型的对象。势必要为每一种对象都
            进行代理，静态代理在程序程序规模稍大时就无法胜任了。
</pre>

<pre>
动态代理：
     在运行时才能确定代理对象；
</pre>