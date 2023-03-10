### Golang 的优势

##### Go语言保证了既能到达静态编译语言的安全和性能，又达到了动态语言开发维护的高效率,使用一个表达式来形容Go语言：Go=C+Python，说明Go语言既有C静态语言程序的运行速度，又能达到Python动态语言的快速开发。

- 1）从C语言中继承了很多理念，包括表达式语法，控制结构，基础数据类型，调用参数传值，指针等等，也保留了和C语言一样的编译执行方式及弱化的指针。 
- 2）引入包的概念，用于組织程序结构，Go语言的一个文件都要归属于一个包，而不能单独存在。
- 3）垃圾回收机制，内存自动回收，不需开发人员管理。
- 4）天然并发
  - (1)从语言层面支持并发，实现简单 
  - (2)goroutine，轻量級线程，可实现大并发处理，高效利用多核。
  - (3)基于CPS并发模型(Communicating Sequential Processes)实现 
- 5）吸收了管道通信机制，形成Go语言特有的管道channel! 通过管道channel，可以实现不同的goroute之间的相互通信。
- 6）函数返回多个值
- 7）新的创新：比如切片、延时执行defer等

### Golang 执行流程分析
##### 说明：两种执行流程的方式区别

- 1）如果我们先編译生成了可执行文件，那么我们可以将该可执行文件拷贝到没有go开发环境的机器上，仍然可以运行
- 2）如果我们是直接 go run go源代码，那么如果要在另外一个机器上这么运行，也需要go 开发环境，否则无法执行。
- 3）在编译时，编译器会将程序运行依赖的库文件包含在可执行文件中，所以，可执行文件
变大了很多。

### Golang 快速开发入门
#### Go程序开发注意事项(重点）

- 1）Go源文件以"go”为扩展名。 
- 2）Go应用程序的执行入口是main()方法。 
- 3）Go语言严格区分大小写。 
- 4）G0方法由一条条语句构成，每个语句 后不需要分号(Go语言会在每行后自动加分号），这也体现出Golang的简洁性。 
- 5）Go編译器是一行行进行编译的，因此我们一行就写一条语句，不能把多条语句写在同一行，否则报错
- 6）Go语言定义的变量或者import的包如果没有使用到，代码不能編译通过。 
- 7）大括号都是成对出现的，缺一不可。

### Golang 转义字符
##### Golang常用的转义字符(escape char)

- 1）\t：一个制表位，实现对齐的功能
- 2）\n：换行符
- 3）\\：一个
- 4）\"：一个"
- 5）\r：一个回车

### Golang 注释

```golang
// 单行注释（推荐使用）
/*  多行注释 */
```
