# TRRL

+ https://github.com/killercup/trpl-ebook
+ https://github.com/KaiserY/trpl-zh-cn

## 所有权
+ 值有且只有一个所有者
+ 当所有者（变量）离开作用域，这个值将被丢弃。
+ 所有权的转移


### 栈（Stack）与堆（Heap）
+ 栈
    * 后进先出
    * 快
        - 数据存取的位置总是在栈顶而不需要寻找一个位置存放或读取数据
        - 栈中的所有数据都必须占用已知且固定的大小


### 内存与分配
+ GC
    *  记录并清除不再使用的内存
+ rust
    * 内存在拥有它的变量离开作用域后就被自动释放
        - drop/RAII

#### move
浅拷贝（shallow copy）&& drop

Rust 永远也不会自动创建数据的 “深拷贝”

####  clone
deep copy

####  copy
+ 像整型这样的在编译时已知大小的类型被整个存储在 __栈__ 上，所以拷贝其实际的值是快速的
    * 没有深浅拷贝的区别
+ Copy trait
    + 一个旧的变量在将其赋值给其他变量后仍然可用。
    + 规则
        * 任何简单标量值的组合/不需要分配内存或某种形式资源的类型
            - 所有整数类型，比如 u32。
            - 布尔类型，bool，它的值是 true 和 false。
            - 所有浮点数类型，比如 f64。
            - 字符类型，char。
            - 元组，当且仅当其包含的类型也都是 Copy 的时候。
                + 比如，(i32, i32) 是 Copy 的，但 (i32, String) 就不是。
    + Rust 不允许自身或其任何部分实现了 Drop trait 的类型使用 Copy trait。
        * 如果我们对其值离开作用域时需要特殊处理的类型使用 Copy 注解，将会出现一个编译时错误。


### 引用、借用
+ 允许使用值但不获取其所有权
+ 引用默认不允许修改引用的值。
+ 可变引用
    * 在特定作用域中的特定数据有且只有一个可变引用。
        - 避免数据竞争
            + 数据竞争
                * 两个或更多指针同时访问同一数据。
                * 至少有一个指针被用来写入数据。
                * 没有同步数据访问的机制。
+ 在任意给定时间，要么 只能有一个可变引用，要么 只能有多个不可变引用。
+ 引用必须总是有效。
    * 悬垂引用（Dangling References）
        - 当 dangle 的代码执行完毕后，变量将被释放
        - `this function's return type contains a borrowed value, but there is no valuefor it to be borrowed from.`

## 泛型

##  生命周期

## 智能指针
+ 区别于常规结构体: 实现了 `Deref` 和 `Drop` trait
+ 区别于引用: 所有权
    * 引用是一类只借用数据的指针, 智能指针 拥有 他们指向的数据。

### Box
用于在堆上分配值，并且可确定大小

### Rc
数据有多个所有者。

记录总共有多少个所有者，当没有任何所有者时负责清理数据。

### RefCell

## 并发

### 线程

### 消息传递
golang, Do not communicate by sharing memory; instead, share memory by communicating.

### 共享状态


###  send
线程间转移所有权


### sync
多线程访问

&T（T 的引用）是 Send 的话 T 就是 Sync 的，这意味着其引用就可以安全的发送到另一个线程。
