# In-Bitcoin-We-Rust.github.io

## Why Rust for blockchain?

+ no GC, no runtime
    * which made memory safety, and integrates with other languages easily.
    * 防止GC时性能的不稳定，世界暂停。
+ Reliability
    * The ownership model
+ Productivity
    * editor support
    * type inspections
    * better formatter
    * friendly error warning
+ 并发模型
+ Rust 具有出色的C ++性能和使您可以像Go一样轻松编程的出色编译器。
+ 性能
    * cpp ~ rust > Go (因为 GC)
        - C可以​​实现非凡的性能，但抽象程度较低，并且容易导致人为错误。
        - 函数式编程语言，例如Haskell，Idris，在可靠性方面是可靠的，但是性能低。
            + "Rust 的美妙之处在于其为如此底层的语言注入了如此高级的吸收了大量 Haskell 精髓的类型系统。""
                * monad，monoid，senigroup，sum type，product type
                    - https://zhuanlan.zhihu.com/p/69223872
                        + "围绕着编程语言是否需要 exception，exception 是良药还是毒药，有诸多争议，java / python 是建制派，C++ / haskell 是骑墙派，rust / go 是反对派，erlang / elixir 是无政府主义者，这里便不展开。你问我支持谁？我喜欢尤达大师对卢克说的那句经典台词：do or do not, there’s no try。这句话也蕴含了 erlang 的哲理：let it crash。""
+ 内存安全性
    * rust > Go > cpp
        - Go 只需要保证 single thread 的 memory safety
+ 有 MIR
    * static analysis 方便
    * 方便验证代码正确性
        - consensus protocol
        - vm
+ 资源管理
    * 直接控制资源管理（包括内存，文件，网络和线程等），没有任何抽象
    * 避免资源泄漏，重复发布和数据竞争等问题
+ rust 最令人兴奋的是所有权的概念，零成本抽象的能力，以及通过合适的约束巧妙解决内存安全和线程安全两大难题的优雅
    * linux kernel 里面这两类 bug 占据了 1/2。
    * 也就是说，你只要学会了 rust，就躺着消弭了 50% 的难啃的让 kernel developer 都闻之变色的 bug。

## Libra
[Libra 中使用的库。用途&用法。](libra/libra.md)

原文链接： https://github.com/tyrchen/unchained/blob/master/code/libra.md


## TRPL

[TRPL 学习笔记](TRPL/README.md)

## TAO

[TAO 学习笔记](TAO/README.md)

## Drawback

[Drawback](drawback.md)

## Miscellaneous

[Miscellaneous](misc.md)

