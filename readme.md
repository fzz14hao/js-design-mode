设计模式是一套被反复使用的、多数人知晓的、经过分类编目的、代码设计经验的总结。使用设计模式是为了重用代码、让代码更容易被他人理解、保证代码可靠性。



### 面向对象
    * 封装、继承、多态
    * 数据结构化

### 封装三要素
    * public完全开放
    * protected对子类开放
    * private对自己开放

###  5大设计原则
    * 单一职责
    * 开放封闭
    * 李氏置换
    * 接口独立
    * 依赖倒置


###  设计模式类型
    * 创建型
    * 结构型
    * 行为型


### 常用设计模式对比
<table>
<tr>
 <th width="120">模式类型</th>
 <th>特点</th>
  <th>应用场景</th>
</tr>
<tr>
  <td>工厂模式</td>
  <td>将new操作单独封装</td>
  <td>jQuery - $('div)<br>
      React.createElement<br>
      vue 异步组件<br></td>
</tr>
<tr>
  <td>单例模式</td>
  <td> 系统中被唯一使用, 一个类只有一个实例</td>
  <td>登录框<br>
          购物车</td>
</tr>
<tr>
  <td>适配器模式</td>
  <td>旧接口格式和使用者不兼容，中间加一个适配转换接口  </td>
  <td>封装旧接口<br>
           vue computed</td>
</tr>
<tr>
  <td>装饰器模式</td>
  <td>   为对象添加新功能，不改变原有的结构和功能</td>
  <td>     ES7装饰器 （babel-plugin-transform-decorators-legacy）<br>
         core-decorators</td>
</tr>
<tr>
  <td>代理模式</td>
  <td> 使用者无权访问目标对象，中间加代理，通过代理做授权和控制 </td>
  <td> 网页事件代理<br>
                 $.proxy<br>
                 ES6 Proxy</td>
</tr>
<tr>
  <td>外观模式</td>
  <td>为子系统中的一组接口提供一个高层接口，使用者使用这个高层接口</td>
  <td></td>
</tr>
<tr>
  <td>观察者模式</td>
  <td>   发布 & 订阅， 一对多</td>
  <td>  网页事件绑定<br>
               Promise<br>
               jQuery Callbacks<br>
               nodejs 自定义事件、处理http请求、多进程通讯<br>
               vue和React组件生命周期触发<br>
               vue watch</td>
</tr>
<tr>
  <td>迭代器</td>
  <td>  顺序访问一个集合，使用者无须知道集合内部构造</td>
  <td> jQuery each<br>
              ES6 Iterator [Symbol.iterator]属性（函数，执行返回迭代器）</td>
</tr>
<tr>
  <td>状态模式</td>
  <td> 一个对象有状态变化，每次变化会触发一个逻辑
  </td>
  <td>  有限状态机 收藏、取消（javascript-state-machine）<br>
         promise实现</td>
</tr>
</table>

   


  

### 其他设计模式

    * 原型模式
        * clone自己，生成一个新对象
        * Object.create()
    
    * 桥接模式
        * 抽象和实现分离
    
    * 组合模式
        * 生成树形结构，将整体和单个节点的操作抽象出来
        * 虚拟DOM中的vnode
    
    * 享元模式
        * 共享内存
        * 相同的数据，共享使用
    
    * 策略模式
        * 不同策略分开处理
        * 避免 if...else...
    
    * 模板模式

    * 职责链模式
        * 一步操作可以分为多个职责角色来完成
        * 角色都分开，然后用一个链串起来
        * 将发起者和各个处理者隔离

    * 命令模式
        * 发送者 -》 命令对象 -》 接收者
        
        * 网页富文本编辑器操作，浏览器封装了一个命令对象（document.execCommand('bold')）

    * 备忘录模式
        * 随时记录一个对象的状态变化
        * 随时可以回复之前的某个状态（如撤销功能）
        
        * 备忘录，备忘列表，编辑器

    * 中介者模式

    * 访问者模式
        * 将数据操作和数据结构进行分离
