# In-Bitcoin-We-Rust.github.io

## Why Rust for blockchain?

+ no GC, no runtime
    * which made memory safety, and integrates with other languages easily.
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

## TRPL

## Tao


