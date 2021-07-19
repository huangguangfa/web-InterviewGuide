## 基础
- 列举你所了解的计算机存储设备类型？
    - 【利用电能方式存储信息的设备 如】：各式存储器，如各式随机存取存储器（RAM内存条）、只读存储器（ROM硬盘）
    - 【利用磁能方式存储信息的设备 如】：硬盘、软盘、磁带、磁芯存储器、磁泡存储器
    - 【利用光学方式存储信息的设备 如】：CD或DVD
    - 【利用磁光方式存储信息的设备 如】：MO（磁光盘）
    - 【利用其他实体物如纸卡、纸带等存储信息的设备 如】：打孔卡、打孔带
- 一般代码存储在计算机的哪个设备中？代码在 CPU 中是如何运行的？
  
   - 计算机基本五个部分：【运算器】 【控制器】 【存储器】 【输入设备】 【输出设备】
    
   - 在计算机中 保存信息主要存储器、存储器又包括：【内部存储器】和【外部存储器】、内部存储器指的是内存、外部存储器指的就是硬盘、一般来说内存是给程序运行时候用的、用来开启进程和快速读写数据的、我们代码保存在硬盘中。
     ![关系图](https://user-gold-cdn.xitu.io/2020/1/20/16fbf1125bc64990?imageView2/0/w/1280/h/960/format/webp/ignore-error/1)
     
      数据的存取关系是、从硬盘中读取数据保存二进制文件到内存中、**对于CPU来说，必须要把数据读取到寄存器中才能做相应的运算**、所以在cpu进行计算的时候从内存中读取数据，然后放到寄存器中、然后执行指令取出寄存器的数据进行计算、
      然后把结果保存在寄存器;下面我们用前端代码来简单讲解下：
        
        ```js
        //test.js
        let a = 1;
        let b = 1;
        let sum = a + b;
        ``` 
      大概就是这样、首页我们的test.js文件存储在硬盘、然后我们启动我们的node服务、这时候因为使用到了test.js所以把这个文件已经加载到内存中了、然后我们运行执行cpu计算、这个时候因为我们并不能直接使用内存中的变量值、所以我们
      需要把内存的变量读取出来保存到cup的寄存器（cpu会有集成很多个寄存器）然后我们在执行计算指令进行a+b的操作、只后我们会把结果保存回寄存器！
     

- 什么是指令和指令集？
    - 指令：计算机程序发给计算机处理器的命令
    - 指令集：指令集是机器指令层面的一种分类，比如IA32指令集，Power指令集，ARM指令集等等，汇编语言对应着指令集里具体的每一条指令，不同的指令集差别很大，指令集一般是通过更底层的微代码（MicroCode）实现的，可以把微代码认为是机器语言的底层语言。常用的高级语言，比如C++，建立在各种指令集的语言之上，通过编译器去转换成机器语言执行

- 复杂指令集(CISC)和精简指令(RISC)集有什么区别？
    - CISC：数量多、使用频率差别大、可变长格式、寻址方式多、使用的是微程序控制技术
    - RISC：数量少、使用频率差别进、大部分为单周期指令、操作寄存器只要Load和Store操作内存、寻址方式少

- JavaScript 是如何运行的？解释型语言和编译型语言的差异是什么？
    - !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    - 差异
        - 解释型语言中，代码自上而下运行，且实时返回运行结果。代码在由浏览器执行前，不需要将其转化为其他形式。代码将直接以文本格式（text form）被接收和处理
        - 需要先将代码转化（编译）成另一种形式才能运行。比如 C/C++ 先被编译成汇编语言，然后才能由计算机运行。程序将以二进制的格式运行，这些二进制内容是由程序源代码产生的
- 简单描述一下 Babel 的编译过程？


- JavaScript 中的数组和函数在内存中是如何存储的？


- 浏览器和 Node.js 中的事件循环机制有什么区别？


- ES6 Modules 相对于 CommonJS 的优势是什么？


- 高级程序设计语言是如何编译成机器语言的？


- 编译器一般由哪几个阶段组成？数据类型检查一般在什么阶段进行？


- 编译过程中虚拟机的作用是什么？


- 什么是中间代码（IR），它的作用是什么？


- 什么是交叉编译？


- 发布 / 订阅模式和观察者模式的区别是什么？


- 装饰器模式一般会在什么场合使用？


- 谈谈你对大型项目的代码解耦设计理解？什么是 Ioc？一般 DI 采用什么设计模式实现？


- 列举你所了解的编程范式？


- 什么是面向切面（AOP）的编程？


- 什么是函数式编程？什么是响应式编程？什么是函数响应式编程？


- 响应式编程或者函数响应式编程的使用场景有哪些？

## 语法

- 如何实现一个上中下三行布局，顶部和底部最小高度是 100px，中间自适应?


- 如何判断一个元素 CSS 样式溢出，从而可以选择性的加 title 或者 Tooltip?


- 如何让 CSS 元素左侧自动溢出（... 溢出在左侧）？


- 什么是沙箱？浏览器的沙箱有什么作用？


- 如何处理浏览器中表单项的密码自动填充问题？


- Hash 和 History 路由的区别和优缺点？


- JavaScript 中的 const 数组可以进行 push 操作吗？为什么？


- JavaScript 中对象的属性描述符有哪些？分别有什么作用？


- JavaScript 中 console 有哪些 api ?


- 简单对比一下 Callback、Promise、Generator、Async 几个异步 API 的优劣？


- Object.defineProperty 有哪几个参数？各自都有什么作用？


- Object.defineProperty 和 ES6 的 Proxy 有什么区别？


- ES6 中 Symbol、Map、Decorator 的使用场景有哪些？或者你在哪些库的源码里见过这些 API 的使用？


- 为什么要使用 TypeScript ? TypeScript 相对于 JavaScript 的优势是什么？


- TypeScript 中 const 和 readonly 的区别？枚举和常量枚举的区别？接口和类型别名的区别？


- TypeScript 中 any 类型的作用是什么？


- TypeScript 中 any、never、unknown 和 void 有什么区别？


- TypeScript 中 interface 可以给 Function / Array / Class（Indexable）做声明吗？


- TypeScript 中可以使用 String、Number、Boolean、Symbol、Object 等给类型做声明吗？


- TypeScript 中的 this 和 JavaScript 中的 this 有什么差异？


- TypeScript 中使用 Unions 时有哪些注意事项？


- TypeScript 如何设计 Class 的声明？


- TypeScript 中如何联合枚举类型的 Key?


- TypeScript 中 ?.、??、!.、_、** 等符号的含义？


- TypeScript 中预定义的有条件类型有哪些？


- 简单介绍一下 TypeScript 模块的加载机制？


- 简单聊聊你对 TypeScript 类型兼容性的理解？抗变、双变、协变和逆变的简单理解？


- TypeScript 中对象展开会有什么副作用吗？


- TypeScript 中 interface、type、enum 声明有作用域的功能吗？


- TypeScript 中同名的 interface 或者同名的 interface 和 class 可以合并吗？


- 如何使 TypeScript 项目引入并识别编译为 JavaScript 的 npm 库包？


- TypeScript 的 tsconfig.json 中有哪些配置项信息？


- TypeScript 中如何设置模块导入的路径别名？

## 框架
- React Class 组件有哪些周期函数？分别有什么作用？


- React Class 组件中请求可以在 componentWillMount 中发起吗？为什么？


- React Class 组件和 React Hook 的区别有哪些？


- React 中高阶函数和自定义 Hook 的优缺点？


- 简要说明 React Hook 中 useState 和 useEffect 的运行原理？


- React 如何发现重渲染、什么原因容易造成重渲染、如何避免重渲染？


- React Hook 中 useEffect 有哪些参数，如何检测数组依赖项的变化？


- React 的 useEffect 是如何监听数组依赖项的变化的？


- React Hook 和闭包有什么关联关系？


- React 中 useState 是如何做数据初始化的？


- 列举你常用的 React 性能优化技巧？


- Vue 2.x 模板中的指令是如何解析实现的？


- 简要说明 Vue 2.x 的全链路运作机制？


- 简单介绍一下 Element UI 的框架设计？


- 如何理解 Vue 是一个渐进式框架？


- Vue 里实现跨组件通信的方式有哪些？


- Vue 中响应式数据是如何做到对某个对象的深层次属性的监听的？


- MVVM、MVC 和 MVP 的区别是什么？各自有什么应用场景？、


- 什么是 MVVM 框架？

## 工程

- Vue CLI 3.x 有哪些功能？Vue CLI 3.x 的插件系统了解？


- Vue CLI 3.x 中的 Webpack 是如何组装处理的？


- Vue 2.x 如何支持 TypeScript 语法？


- 如何配置环境使得 JavaScript 项目可以支持 TypeScript 语法？


- 如何对 TypeScript 进行 Lint 校验？ESLint 和 TSLint 有什么区别？


- Node.js 如何支持 TypeScript 语法？


- TypeScript 如何自动生成库包的声明文件？


- Babel 对于 TypeScript 的支持有哪些限制？


- Webpack 中 Loader 和 Plugin 的区别是什么？


- 在 Webpack 中是如何做到支持类似于 JSX 语法的 Sourcemap 定位？


- 发布 Npm 包如何指定引入地址？


- 如何发布开发项目的特定文件夹为 Npm 包的根目录？


- 如何发布一个支持 Tree Shaking 机制的 Npm 包？


- Npm 包中 peerDependencies 的作用是什么？


- 如何优雅的调试需要发布的 Npm 包？


- 在设计一些库包时如何生成版本日志？


- 了解 Git （Submodule）子模块吗？简单介绍一下 Git 子模块的作用？


- Git 如何修改已经提交的 Commit 信息？


- Git 如何撤销 Commit 并保存之前的修改？


- Git 如何 ignore 被 commit 过的文件？


- 在使用 Git 的时候如何规范 Git 的提交说明（Commit 信息）？


- 简述符合 Angular 规范的提交说明的结构组成？


- Commit 信息如何和 Github Issues 关联？


- Git Hook 在项目中哪些作用？


- Git Hook 中客户端和服务端钩子各自用于什么作用？


- Git Hook 中常用的钩子有哪些？


- pre-commit 和 commit-msg 钩子的区别是什么？各自可用于做什么？


- husky 以及 ghook 等工具制作 Git Hook 的原理是什么？


- 如何设计一个通用的 Git Hook ？


- Git Hook 可以采用 Node 脚本进行设计吗？如何做到？


- 如何确保别人上传的代码没有 Lint 错误？如何确保代码构建没有 Lint 错误？


- 如何在 Vs Code 中进行 Lint 校验提示？如何在 Vs Code 中进行 Lint 保存格式化？


- ESLint 和 Prettier 的区别是什么？两者在一起工作时会产生问题吗？


- 如何有效的识别 ESLint 和 Prettier 可能产生冲突的格式规则？如何解决此类规则冲突问题？


- 在通常的脚手架项目中进行热更新（hot module replacement）时如何做到 ESLint 实时打印校验错误信息？


- 谈谈你对 SourceMap 的了解？


- 如何调试 Node.js 代码？如何调试 Node.js TypeScript 代码？在浏览器中如何调试 Node.js 代码？


- 列举你知道的所有构建工具并说说这些工具的优缺点？这些构建工具在不同的场景下应该如何选型？


- VS Code 配置中的用户和工作区有什么区别？


- VS Code 的插件可以只对当前项目生效吗？


- 你所知道的测试有哪些测试类型？


- 你所知道的测试框架有哪些？


- 什么是 e2e 测试？有哪些 e2e 的测试框架？


- 假设现在有一个插入排序算法，如何对该算法进行单元测试？

## 网络
- CDN 服务如何实现网络加速？


- WebSocket 使用的是 TCP 还是 UDP 协议？


- 什么是单工、半双工和全双工通信？


- 简单描述 HTTP 协议发送一个带域名的 URL 请求的协议传输过程？（DNS、TCP、IP、链路）


- 什么是正向代理？什么是反向代理？


- Cookie 可以在服务端生成吗？Cookie 在服务端生成后的工作流程是什么样的？


- Session、Cookie 的区别和关联？如何进行临时性和永久性的 Session 存储？


- 设置 Cookie 时候如何防止 XSS 攻击？


- 简单描述一下用户免登陆的实现过程？可能会出现哪些安全性问题？一般如何对用户登录的密码进行加密？


- HTTP 中提升传输速率的方式有哪些？常用的内容编码方式有哪些？


- 传输图片的过程中如果突然中断，如何在恢复后从之前的中断中恢复传输？


- 什么是代理？什么是网关？代理和网关的作用是什么？


- HTTPS 相比 HTTP 为什么更加安全可靠？


- 什么是对称密钥（共享密钥）加密？什么是非对称密钥（公开密钥）加密？哪个更加安全？


- 你觉得 HTTP 协议目前存在哪些缺点？
 ## 插件
- Vue CLI 3.x 的插件系统是如何设计的？

- Webpack 中的插件机制是如何设计的？

\r\n（CRLF） 和 \n （LF）的区别是什么？(Vs Code 的右下角可以切换)

## 系统
\r\n（CRLF） 和 \n （LF）的区别是什么？(Vs Code 的右下角可以切换)


/dev/null 的作用是啥？


如何在 Mac 的终端中设置一个命令的别名？


如何在 Windows 中设置环境变量？


Mac 的文件操作系统默认区分文件路径的大小写吗？


编写 Shell 脚本时如何设置文件的绝对路径？

## 后端
- Session、Cookie 的区别和关联？如何进行临时性和永久性的 Session 存储？


- 如何部署 Node.js 应用？如何处理负载均衡中 Session 的一致性问题？


- 如何提升 Node.js 代码的运行稳定性？


- GraphQL 与 Restful 的区别，它有什么优点？


- Vue SSR 的工作原理？Vuex 的数据如何同构渲染？


- SSR 技术和 SPA 技术的各自的优缺点是什么？


- 如何处理 Node.js 渲染 HTML 压力过大问题？

## 通用性
- 如果让你设计一个通用的项目脚手架，你会如何设计？一个通用的脚手架一般需要具备哪些能力？


- 如果让你设计一个通用的工具库，你会如何设计？一个通用的工具库一般需要具备哪些能力？


- 假设你自己实现的 React 或 Vue 的组件库要设计演示文档，你会如何设计？设计的文档需要实现哪些功能？


- 在设计工具库包的时候你是如何设计 API 文档的？


## 业务
- 什么是单点登录？如何做单点登录？


- 如何做一个项目的国际化方案？


- 如何做一个项目的监控和埋点方案？


- 如何建设项目的稳定性（监控、灰度、错误降级、回滚...）？


- 一般管理后台型的应用需要考虑哪些性能方面的优化？


- 简述一些提升项目体验的案例和技术方案（骨架屏、Loading 处理、缓存、错误降级、请求重试...）？


- 假设需要对页面设计一个水印方案，你会如何设计？

## 数据结构

- 使用 TypeScript 语法将没有层级的扁平数据转换成树形结构的数据
```js
// 扁平数据
[{
  name: '文本1',
  parent: null,
  id: 1,
}, {
  name: '文本2',
  id: 2,
  parent: 1
}, {
  name: '文本3',
  parent: 2,
  id: 3,
}]

// 树状数据
[{
  name: '文本1',
  id: 1,
  children: [{
    name: '文本2',
    id: 2,
    children: [{
      name: '文本3',
      id: 3
    }]
  }]
}]

```

## 模板解析
- 实现一个简易的模板引擎
```js
const template = '嗨，{{ info.name.value }}您好，今天是星期 {{ day.value }}';

const data = {
  info: {
    name: {
      value: '张三'
    }
  },
  day: {
    value: '三'
  }
};
render(template, data); // 嗨，张三您好，今天是星期三

```

## 设计模式

- 简单实现一个发布 / 订阅模式