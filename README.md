# Interview
- JS有哪些数据类型，怎么判断数据类型
    数据类型有 null,undefined,boolean,string,number,symbol
  判断数据类型
    typeof only for 基础数据类型 null和普通对象都返回object
    instanceof only for 复杂数据类型 是谁的实例 可用于自定义对象
    constructor可用于自定义对象 constructor可能会被修改
    Object.prototype.toString.call()
-请求可以中断吗，怎么做
  中断请求 abortcontroller 通过监听controller.signal配合fetch中断请求/超时可配合promise.race
原型和原型链
  原型是构造函数的一个属性，构造函数new一个实例时会将新对象的__proto__指向构造函数的prototype。原型也有自己的原型，构成了原型链，可以实现继承

  —— “步入（Step into）”，快捷键 F11。
和“下一步（Step）”类似，但在异步函数调用情况下表现不同。如果你刚刚才开始学 JavaScript，那么你可以先忽略此差异，因为我们还没有用到异步调用。

至于之后，只需要记住“下一步（Step）”命令会忽略异步行为，例如 setTimeout（计划的函数调用），它会过一段时间再执行。而“步入（Step into）”会进入到代码中并等待（如果需要）。详见 DevTools 手册。

 —— “步出（Step out）”：继续执行到当前函数的末尾，快捷键 Shift+F11。
继续执行当前函数内的剩余代码，并暂停在调用当前函数的下一行代码处。当我们使用  偶然地进入到一个嵌套调用，但是我们又对这个函数不感兴趣时，我们想要尽可能的继续执行到最后的时候是非常方便的。
