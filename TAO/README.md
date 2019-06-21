# TAO of Rust

p.10

+ https://github.com/RustStudy/tao_of_rust_docs
+ https://github.com/ZhangHanDong/tao-of-rust-codes
+ https://github.com/ZhangHanDong/tao-of-rust-fix

不需要有垃圾回收这样的系统，不能为了内存安全而引入性能负担。(世界暂停/不确定性性能延迟)


## rust 三条设计哲学
+ 内存安全
    * 所有权系统
        - 每个被分配的内存都有一个独占其所有权的指针
        - 只有当该指针被销毁时，其对应的内存才能随之被释放
        - 所有权系统还包括了从现代 c++ 那里借鉴的 RAII 机制，这是 Rust no GC 但是可以安全管理内存的基石
    * 借用和生命周期
        - 每个变量都有其生命周期， 一旦超出生命周期，变量就会被自动释放
        - 如果是借用，则可以通过标记生命周期参数供编译器检查的方式，防止出现悬垂指针，也就是释放后使用的情况
+ 零成本抽象
    * 基石是泛型和 trait
+ 实用性