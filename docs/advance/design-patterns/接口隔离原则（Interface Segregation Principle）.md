接口隔离原则的具体含义如下。
1. 一个类对另外一个类的依赖性应当是建立在最小的接口上的。
2. 一个接口代表一个角色，不应当将不同的角色都交给一个接口。没有关系的接口合并在一起，形成一个臃肿的大接口，这是对角色和接口的污染。因此使用多个专门的接口比使用单一的总接口要好。
3. 不应该强迫客户依赖于它们不用的方法。接口属于客户，不属于它所在的类层次结构，即不要强迫客户使用它们不用的方法，否则这些客户就会面临由于这些不使用的方法的改变所带来的改变。

接口隔离强调接口的单一性。强调对于实现的分离。只提供调用者需要的方法，屏蔽不需要的方法。

分离的手段主要有以下两种：

1、委托分离，对于已有的接口只提供调用者需要的方法，屏蔽不需要的方法。通过增加一个新的类型来委托客户的请求，隔离客户和接口的直接依赖。

2、多重继承分离，胖接口分离，通过接口多继承来实现客户的需求。
