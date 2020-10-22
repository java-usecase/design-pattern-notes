# Gof 23 设计模式使用手册

参考：https://blog.csdn.net/darling757267/article/details/7433278



[面向对象设计模式与原则](http://blog.163.com/swl_job/blog/static/8223854120085194262528/)

[设计模式总结](http://blog.163.com/swl_job/blog/static/82238541200861784346239/)

|            | 创建型                                                       | 结构型                                                       | 行为型                                                       |
| ---------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 模式名称   | [Singleton](http://blog.163.com/swl_job/blog/static/82238541200861854821962/#Singleton) [Abstract Factory](http://blog.163.com/blankEditor.html#AbstractFactory) [Builder](http://blog.163.com/blankEditor.html#Builder) [Factory Method](http://blog.163.com/blankEditor.html#FactoryMethod)[ Prototype](http://blog.163.com/blankEditor.html#Prototype) | [Adapter](http://blog.163.com/blankEditor.html#Adapter) [Bridge](http://blog.163.com/blankEditor.html#Bridge) [Composite](http://blog.163.com/blankEditor.html#Composite) [Decorator](http://blog.163.com/blankEditor.html#Decorator) [Facade](http://blog.163.com/blankEditor.html#Facade) [Flyweight](http://blog.163.com/blankEditor.html#Flyweight) [Proxy](http://blog.163.com/blankEditor.html#Proxy) | [Template Method](http://blog.163.com/blankEditor.html#TemplateMethod) [Command](http://blog.163.com/blankEditor.html#Command) [Interpreter](http://blog.163.com/blankEditor.html#Interpreter) [Mediator](http://blog.163.com/blankEditor.html#Mediator) [Iterator](http://blog.163.com/blankEditor.html#Iterator) [Observer](http://blog.163.com/blankEditor.html#Observer) [Chain of Responsibility](http://blog.163.com/blankEditor.html#ChainOfResponsibility) [Memento](http://blog.163.com/blankEditor.html#Memento) [State](http://blog.163.com/blankEditor.html#State) [Strategy](http://blog.163.com/blankEditor.html#Strategy) [Visitor](http://blog.163.com/blankEditor.html#Visitor) |
| 模式关系图 | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/MoWvs-l3qgxfndMAkgd2Tg==/5067675480699104525.jpg)](http://img.blog.163.com/photo/MoWvs-l3qgxfndMAkgd2Tg==/5067675480699104525.jpg) |                                                              |                                                              |



| 名称   | [单件模式（Singleton）](http://blog.163.com/swl_job/blog/static/82238541200851943625765/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/uyR64cL5LNxTw6npILX3lw==/629659522902175942.jpg)](http://img.blog.163.com/photo/uyR64cL5LNxTw6npILX3lw==/629659522902175942.jpg) |
| 意图   | 保证一个类仅有一个实例，并提供一个该实例的全局访问点。       |
| 适用性 | 当类只能有一个实例而且客户可以从一个众所周知的访问点访问它时。当这个唯一实例应该是通过子类化可扩展的，并且客户应该无需更改代码就能使用一个扩展的实例时。 |



| 名称   | [抽像工厂模式（Abstract Factory）](http://blog.163.com/swl_job/blog/static/8223854120085189503890/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/Ilpl7MY9QFunzrJfvtVZUQ==/3697455294071591636.jpg)](http://img.blog.163.com/photo/Ilpl7MY9QFunzrJfvtVZUQ==/3697455294071591636.jpg) |
| 意图   | 提供一个接口，让该接口负责创建一系列“相关或者相互依赖的对象”，无需指定它们具体的类。 |
| 适用性 | 一个系统要独立于它的产品的创建、组合和表示时。一个系统要由多个产品系列中的一个来配置时。当你要强调一系列相关的产品对象的设计以便进行联合使用时。当你提供一个产品类库，而只想显示它们的接口而不是实现时。 |



| 名称   | [生成器模式（Builder）](http://blog.163.com/swl_job/blog/static/82238541200852051531691/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/f5TM4vA2QysfQpZY50gZpw==/5120311301344456251.jpg)](http://img.blog.163.com/photo/f5TM4vA2QysfQpZY50gZpw==/5120311301344456251.jpg) |
| 意图   | 将一个复杂对象的构建与其表示相分离，使得同样的构建过程可以创建不同的表示。 |
| 适用性 | 当创建复杂对象的算法应该独立于该对象的组成部分以及它们的装配方式时。当构造过程必须允许被构造的对象有不同的表示时。 |



| 名称   | [工厂方法模式（Factory Method）](http://blog.163.com/swl_job/blog/static/82238541200852051715813/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/Td3UjsDE0oYohnqehOgYDg==/2004101834180385482.jpg)](http://img.blog.163.com/photo/Td3UjsDE0oYohnqehOgYDg==/2004101834180385482.jpg) |
| 意图   | 定义一个用于创建对象的接口，让子类决定实例化哪一个类。Factory Method使得一个类的实例化延迟到子类。 |
| 适用性 | 当一个类不知道它所必须创建的对象的类的时候。当一个类希望由它的子类来指定它所创建的对象的时候。当类将创建对象的职责委托给多个帮助子类中的某一个，并且你希望将哪一个帮助子类是代理者这一信息局部化的时候。 |



| 名称   | [原型模式（Prototype）](http://blog.163.com/swl_job/blog/static/82238541200852052027635/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/czXI5VHOfj7a39rmK4p9kQ==/2326390682514345292.jpg)](http://img.blog.163.com/photo/czXI5VHOfj7a39rmK4p9kQ==/2326390682514345292.jpg) |
| 意图   | 使用原型实例指定创建对象的种类，然后通过拷贝这些原型来创建新的对象。 |
| 适用性 | 当要实例化的类是在运行时刻指定时，例如，通过动态装载；为了避免创建一个与产品类层次平行的工厂类层次时；当一个类的实例只能有几个不同状态组合中的一种时。建立相应数目的原型并克隆它们可能比每次用合适的状态手工实例化该类更方便一些。 |



| 名称   | [适配器模式（Adapter）](http://blog.163.com/swl_job/blog/static/822385412008521470868/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/iPc9jnmFvCIkzGKglwgP9g==/4810125877008863057.jpg)](http://img.blog.163.com/photo/iPc9jnmFvCIkzGKglwgP9g==/4810125877008863057.jpg) |
| 意图   | 将一个类的接口转换成客户希望的另一个接口。Adapter模式使得原本由于接口不兼容而不能一起工作的那些类可以一起工作。 |
| 适用性 | 你想使用一个已经存在的类，而它的接口不符合你的需求。你想创建一个可以复用的类，该类可以与其他不相关的类或不可预见的类（即那些接口可能不一定兼容的类）协同工作。（仅适用于对象A d a p t e r ）你想使用一些已经存在的子类，但是不可能对每一个都进行子类化以匹配它们的接口。对象适配器可以适配它的父类接口。 |



| 名称   | [桥接模式（Bridge）](http://blog.163.com/swl_job/blog/static/8223854120085214947252/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/7tz4rq6lWUnPprPY3iupgw==/4810125877008863072.jpg)](http://img.blog.163.com/photo/7tz4rq6lWUnPprPY3iupgw==/4810125877008863072.jpg) |
| 意图   | 将抽象部分与实现部分分离，使它们都可以独立地变化。           |
| 适用性 | 你不希望在抽象和它的实现部分之间有一个固定的绑定关系。例如这种情况可能是因为，在程序运行时刻实现部分应可以被选择或者切换。类的抽象以及它的实现都应该可以通过生成子类的方法加以扩充。这时B r i d g e 模式使你可以对不同的抽象接口和实现部分进行组合，并分别对它们进行扩充。对一个抽象的实现部分的修改应对客户不产生影响，即客户的代码不必重新编译。（C + +）你想对客户完全隐藏抽象的实现部分。在C + +中，类的表示在类接口中是可见的。有许多类要生成。这样一种类层次结构说明你必须将一个对象分解成两个部分。R u m b a u g h 称这种类层次结构为“嵌套的普化”（nested generalizations ）。你想在多个对象间共享实现（可能使用引用计数），但同时要求客户并不知道这一点。一个简单的例子便是C o p l i e n 的S t r i n g 类[ C o p 9 2 ]，在这个类中多个对象可以共享同一个字符串表示（S t r i n g R e p ）。 |



| 名称   | [组合模式（Composite）](http://blog.163.com/swl_job/blog/static/82238541200852384246975/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/DCDo4IHNvrUfEji6OnCTIQ==/5112711476972974805.jpg)](http://img.blog.163.com/photo/DCDo4IHNvrUfEji6OnCTIQ==/5112711476972974805.jpg) |
| 意图   | 将对象组合成树形结构以表示“部分－整体”的层次结构。Composite使得用户对单个对象和组合对象的使用具有一致性。 |
| 适用性 | 你想表示对象的部分-整体层次结构。你希望用户忽略组合对象与单个对象的不同，用户将统一地使用组合结构中的所有对象。 |



| 名称   | [装饰模式（Decorator）](http://blog.163.com/swl_job/blog/static/82238541200852472338859/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/UCnboZczbvTWRufM82Z-Mw==/582934676768351654.jpg)](http://img.blog.163.com/photo/UCnboZczbvTWRufM82Z-Mw==/582934676768351654.jpg) |
| 意图   | 动态地给一个对象增加一些额外的职责（功能）。就增加功能而言，Decorator模式比生成子类更为灵活。 |
| 适用性 | 在不影响其他对象的情况下，以动态、透明的方式给单个对象添加职责。处理那些可以撤消的职责。当不能采用生成子类的方法进行扩充时。一种情况是，可能有大量独立的扩展，为支持每一种组合将产生大量的子类，使得子类数目呈爆炸性增长。另一种情况可能是因为类定义被隐藏，或类定义不能用于生成子类。 |



| 名称   | [外观模式（Facade）](http://blog.163.com/swl_job/blog/static/82238541200852591412841/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/s44mBeZPvFciD6ybsqA37Q==/583497626721772938.jpg)](http://img.blog.163.com/photo/s44mBeZPvFciD6ybsqA37Q==/583497626721772938.jpg) |
| 意图   | 为子系统的一组接口提供一个一致的界面，Facade模式定义了一个高层接口，这个接口使得这一子系统更加容易使用。 |
| 适用性 | 当你要为一个复杂子系统提供一个简单接口时。子系统往往因为不断演化而变得越来越复杂。大多数模式使用时都会产生更多更小的类。这使得子系统更具可重用性，也更容易对子系统进行定制，但这也给那些不需要定制子系统的用户带来一些使用上的困难。F a c a d e 可以提供一个简单的缺省视图，这一视图对大多数用户来说已经足够，而那些需要更多的可定制性的用户可以越过f a c a d e 层。客户程序与抽象类的实现部分之间存在着很大的依赖性。引入f a c a d e 将这个子系统与客户以及其他的子系统分离，可以提高子系统的独立性和可移植性。当你需要构建一个层次结构的子系统时，使用f a c a d e 模式定义子系统中每层的入口点。如果子系统之间是相互依赖的，你可以让它们仅通过f a c a d e 进行通讯，从而简化了它们之间的依赖关系。 |



| 名称   | [享元模式（Flyweight）](http://blog.163.com/swl_job/blog/static/82238541200852691222960/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/XEiDLA2nW0GkqJXmPb4-uw==/5097511828230391531.jpg)](http://img.blog.163.com/photo/XEiDLA2nW0GkqJXmPb4-uw==/5097511828230391531.jpg) |
| 意图   | 运用共享技术有效地支持大量细粒度的对象。                     |
| 适用性 | 一个应用程序使用了大量的对象。完全由于使用大量的对象，造成很大的存储开销。对象的大多数状态都可变为外部状态。如果删除对象的外部状态，那么可以用相对较少的共享对象取代很多组对象。应用程序不依赖于对象标识。由于F l y w e i g h t 对象可以被共享，对于概念上明显有别的对象，标识测试将返回真值。 |



| 名称   | [代理模式（Proxy）](http://blog.163.com/swl_job/blog/static/8223854120085271100476/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/IWq7wraZcY4kLWmEnFC_Ww==/4566087072200569504.jpg)](http://img.blog.163.com/photo/IWq7wraZcY4kLWmEnFC_Ww==/4566087072200569504.jpg) |
| 意图   | 为其他对象提供一种代理以控制对这个对象的访问。               |
| 适用性 | 在需要用比较通用和复杂的对象指针代替简单的指针的时候，使用P r o x y 模式。下面是一 些可以使用P r o x y 模式常见情况： 1) 远程代理（Remote Proxy ）为一个对象在不同的地址空间提供局部代表。 NEXTSTEP[Add94] 使用N X P r o x y 类实现了这一目的。Coplien[Cop92] 称这种代理为“大使” （A m b a s s a d o r ）。 2 )虚代理（Virtual Proxy ）根据需要创建开销很大的对象。在动机一节描述的I m a g e P r o x y 就是这样一种代理的例子。 3) 保护代理（Protection Proxy ）控制对原始对象的访问。保护代理用于对象应该有不同 的访问权限的时候。例如，在C h o i c e s 操作系统[ C I R M 9 3 ]中K e m e l P r o x i e s 为操作系统对象提供 了访问保护。 4 )智能指引（Smart Reference ）取代了简单的指针，它在访问对象时执行一些附加操作。 它的典型用途包括：对指向实际对象的引用计数，这样当该对象没有引用时，可以自动释放它(也称为S m a r tP o i n t e r s[ E d e 9 2 ] )。当第一次引用一个持久对象时，将它装入内存。在访问一个实际对象前，检查是否已经锁定了它，以确保其他对象不能改变它。 |



| 名称   | [模板方式模式（Template Method）](http://blog.163.com/swl_job/blog/static/82238541200852793144743/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/4MF475Ar3WVFr_cOjd6zmQ==/889460926406476710.jpg)](http://img.blog.163.com/photo/4MF475Ar3WVFr_cOjd6zmQ==/889460926406476710.jpg) |
| 意图   | 定义一个操作中的算法的骨架，而将一些步骤延迟到子类中。Template Method使得子类可以不改变一个算法的结构即可重定义该算法的某些特定步骤。 |
| 适用性 | 一次性实现一个算法的不变的部分，并将可变的行为留给子类来实现。各子类中公共的行为应被提取出来并集中到一个公共父类中以避免代码重复。这是O p d y k e 和J o h n s o n 所描述过的“重分解以一般化”的一个很好的例子[ O J 9 3 ]。首先识别现有代码中的不同之处，并且将不同之处分离为新的操作。最后，用一个调用这些新的操作的模板方法来替换这些不同的代码。控制子类扩展。模板方法只在特定点调用“h o o k ”操作（参见效果一节），这样就只允许在这些点进行扩展。 |



| 名称   | [命令模式（Command）](http://blog.163.com/swl_job/blog/static/82238541200852823548358/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/0Ld8xj4ZTxARWWPu3TCdtw==/2266999462428365285.jpg)](http://img.blog.163.com/photo/0Ld8xj4ZTxARWWPu3TCdtw==/2266999462428365285.jpg) |
| 意图   | 将一个请求封装为一个对象，从而使你可用不同的请求对客户进行参数化；对请求排队或记录请求日志，以及支持可撤销的操作。 |
| 适用性 | 像上面讨论的M e n u I t e m 对象那样，抽象出待执行的动作以参数化某对象。你可用过程语言中的回调（c a l l b a c k ）函数表达这种参数化机制。所谓回调函数是指函数先在某处注册，而它将在稍后某个需要的时候被调用。C o m m a n d 模式是回调机制的一个面向对象的替代品。在不同的时刻指定、排列和执行请求。一个C o m m a n d 对象可以有一个与初始请求无关的生存期。如果一个请求的接收者可用一种与地址空间无关的方式表达，那么就可将负责该请求的命令对象传送给另一个不同的进程并在那儿实现该请求。支持取消操作。C o m m a n d 的E x c u t e 操作可在实施操作前将状态存储起来，在取消操作时这个状态用来消除该操作的影响。C o m m a n d 接口必须添加一个U n e x e c u t e 操作，该操作取消上一次E x e c u t e 调用的效果。执行的命令被存储在一个历史列表中。可通过向后和向前遍历这一列表并分别调用U n e x e c u t e 和E x e c u t e 来实现重数不限的“取消”和“重做”。支持修改日志，这样当系统崩溃时，这些修改可以被重做一遍。在C o m m a n d 接口中添加装载操作和存储操作，可以用来保持变动的一个一致的修改日志。从崩溃中恢复的过程包括从磁盘中重新读入记录下来的命令并用E x e c u t e 操作重新执行它们。用构建在原语操作上的高层操作构造一个系统。这样一种结构在支持事务( t r a n s a c t i o n )的信息系统中很常见。一个事务封装了对数据的一组变动。C o m m a n d 模式提供了对事务进行建模的方法。C o m m a n d 有一个公共的接口，使得你可以用同一种方式调用所有的事务。同时使用该模式也易于添加新事务以扩展系统。 |



| 名称   | [解释器模式（Interpreter）](http://blog.163.com/swl_job/blog/static/82238541200852902122631/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/6MmFKsyY2wpl9zTLDShGvw==/2266999462428365313.jpg)](http://img.blog.163.com/photo/6MmFKsyY2wpl9zTLDShGvw==/2266999462428365313.jpg) |
| 意图   | 给定一个语言，定义它的文法的一种表示，并定义一种解释器，这个解释器使用该表示来解释语言中的句子。 |
| 适用性 | 当当有一个语言需要解释执行, 并且你可将该语言中的句子表示为一个抽象语法树时，可使用解释器模式。而当存在以下情况时该模式效果最好：该文法简单对于复杂的文法, 文法的类层次变得庞大而无法管理。此时语法分析程序生成器这样的工具是更好的选择。它们无需构建抽象语法树即可解释表达式, 这样可以节省空间而且还可能节省时间。效率不是一个关键问题最高效的解释器通常不是通过直接解释语法分析树实现的, 而是首先将它们转换成另一种形式。例如，正则表达式通常被转换成状态机。但即使在这种情况下, 转换器仍可用解释器模式实现, 该模式仍是有用的。 |



| 名称   | [中介者模式（Mediator）](http://blog.163.com/swl_job/blog/static/822385412008529103538823/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/NM5T6LL_WCE4Rqnv7kK05w==/2814749767107154555.jpg)](http://img.blog.163.com/photo/NM5T6LL_WCE4Rqnv7kK05w==/2814749767107154555.jpg) |
| 意图   | 用一个中介对象来封装一系列对象交互。中介者使各对象不需要显式的相互引用，从而使其耦合松散，而且可以独立地改变它们之间的交互。 |
| 适用性 | 一组对象以定义良好但是复杂的方式进行通信。产生的相互依赖关系结构混乱且难以理解。一个对象引用其他很多对象并且直接与这些对象通信,导致难以复用该对象。想定制一个分布在多个类中的行为，而又不想生成太多的子类。 |



| 名称   | [迭代器模式（Iterator）](http://blog.163.com/swl_job/blog/static/82238541200863454413/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/W0jwGV9qpKhzv9zdFZ1i0Q==/2814749767107154576.jpg)](http://img.blog.163.com/photo/W0jwGV9qpKhzv9zdFZ1i0Q==/2814749767107154576.jpg) |
| 意图   | 提供一种方法顺序访问一个聚合对象中的各个元素，而又不暴露该对象的内部表示。 |
| 适用性 | 访问一个聚合对象的内容而无需暴露它的内部表示。支持对聚合对象的多种遍历。为遍历不同的聚合结构提供一个统一的接口(即, 支持多态迭代)。 |



| 名称   | [观察者模式（Observer）](http://blog.163.com/swl_job/blog/static/8223854120086864335350/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/lf81GNDMU_FI3ZoqsGUUig==/3390366094480658676.jpg)](http://img.blog.163.com/photo/lf81GNDMU_FI3ZoqsGUUig==/3390366094480658676.jpg) |
| 意图   | 定义对象间的一种一对多的依赖关系，以便当一个对象的状态发生改变时，所有的依赖于它的对象都得到通知并自动更新。 |
| 适用性 | 当一个抽象模型有两个方面, 其中一个方面依赖于另一方面。将这二者封装在独立的对象中以使它们可以各自独立地改变和复用。当对一个对象的改变需要同时改变其它对象, 而不知道具体有多少对象有待改变。当一个对象必须通知其它对象，而它又不能假定其它对象是谁。换言之, 你不希望这些对象是紧密耦合的。 |



| 名称   | [职责链模式（Chain of Responsibility）](http://blog.163.com/swl_job/blog/static/82238541200861085747685/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/W6OEOQEwUpNwTPwZRoivJQ==/3390366094480658700.jpg)](http://img.blog.163.com/photo/W6OEOQEwUpNwTPwZRoivJQ==/3390366094480658700.jpg) |
| 意图   | 使多个对象都有机会处理请求，从而避免请求的发送者和接收者之间的耦合关系。将这些对象连成一条链，并沿着这条链传递请求，直到有一个对象处理它为止。 |
| 适用性 | 有多个的对象可以处理一个请求，哪个对象处理该请求运行时刻自动确定。你想在不明确指定接收者的情况下，向多个对象中的一个提交一个请求。可处理一个请求的对象集合应被动态指定。 |



| 名称   | [备忘录模式（Memento）](http://blog.163.com/swl_job/blog/static/82238541200861165811121/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/s0ZpPfzVDgU75UDPIjc_gQ==/2050545205337785487.jpg)](http://img.blog.163.com/photo/s0ZpPfzVDgU75UDPIjc_gQ==/2050545205337785487.jpg) |
| 意图   | 在不破坏封装性的前提下，捕获一个对象的内部状态，并在该对象之外保存这个状态。这样以后就可以将该对象恢复到原先保存的状态。 |
| 适用性 | 必须保存一个对象在某一个时刻的(部分)状态, 这样以后需要时它才能恢复到先前的状态。如果一个用接口来让其它对象直接得到这些状态，将会暴露对象的实现细节并破坏对象的封装性。 |



| 名称   | [状态模式（State）](http://blog.163.com/swl_job/blog/static/82238541200861352133651/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/YcrKAan-Akw4SQRpeUhhKg==/4020025617382542713.jpg)](http://img.blog.163.com/photo/YcrKAan-Akw4SQRpeUhhKg==/4020025617382542713.jpg) |
| 意图   | 允许一个对象在其内部状态改变时改变它的行为。从而使对象看起来似乎修改了其行为。 |
| 适用性 | 一个对象的行为取决于它的状态, 并且它必须在运行时刻根据状态改变它的行为。一个操作中含有庞大的多分支的条件语句，且这些分支依赖于该对象的状态。这个状态通常用一个或多个枚举常量表示。通常, 有多个操作包含这一相同的条件结构。S t a t e模式将每一个条件分支放入一个独立的类中。这使得你可以根据对象自身的情况将对象的状态作为一个对象，这一对象可以不依赖于其他对象而独立变化。 |



| 名称   | [策略模式（Strategy）](http://blog.163.com/swl_job/blog/static/82238541200861352258895/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/xAW3zvvdKNaJqJjzwQeWPg==/2565925887694760203.jpg)](http://img.blog.163.com/photo/xAW3zvvdKNaJqJjzwQeWPg==/2565925887694760203.jpg) |
| 意图   | 定义一系列算法，把它们一个个封装起来，并且使它们可以互相替换。该模式使得算法可独立于使用它的客而变化。 |
| 适用性 | 许多相关的类仅仅是行为有异。“策略”提供了一种用多个行为中的一个行为来配置一个类的方法。需要使用一个算法的不同变体。例如，你可能会定义一些反映不同的空间/时间权衡的算法。当这些变体实现为一个算法的类层次时[ H O 8 7 ] ,可以使用策略模式。算法使用客户不应该知道的数据。可使用策略模式以避免暴露复杂的、与算法相关的数据结构。一个类定义了多种行为, 并且这些行为在这个类的操作中以多个条件语句的形式出现。将相关的条件分支移入它们各自的S t r a t e g y 类中以代替这些条件语句。 |



| 名称   | [访问者模式（Visitor）](http://blog.163.com/swl_job/blog/static/8223854120086140215752/)   [返回顶部](http://blog.163.com/blankEditor.html#top) |
| ------ | ------------------------------------------------------------ |
| 结构   | [![设计模式应用手册 - wing - 朋友们](http://img.blog.163.com/photo/aLufc51KJ1_TGRcXLYyYvg==/2565925887694760230.jpg)](http://img.blog.163.com/photo/aLufc51KJ1_TGRcXLYyYvg==/2565925887694760230.jpg) |
| 意图   | 表示一个作用于某对象结构中的各元素的操作。它可以在不改变各元素的类的前提下定义作用于这些元素的新的操作。 |
| 适用性 | 一个对象结构包含很多类对象，它们有不同的接口，而你想对这些对象实施一些依赖于其具体类的操作。需要对一个对象结构中的对象进行很多不同的并且不相关的操作，而你想避免让这些操作“污染”这些对象的类。Vi s i t o r 使得你可以将相关的操作集中起来定义在一个类中。当该对象结构被很多应用共享时，用Vi s i t o r 模式让每个应用仅包含需要用到的操作。定义对象结构的类很少改变，但经常需要在此结构上定义新的操作。改变对象结构类需要重定义对所有访问者的接口，这可能需要很大的代价。如果对象结构类经常改变，那么可能还是在这些类中定义这些操作较好。 |