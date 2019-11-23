# articles

## stdlib
+ https://ehsanmkermani.com/2019/06/18/rust-std-study-series-interior-mutability/
+ https://blog.yoshuawuyts.com/std-time/

## rustc? rust-os?
* https://robert.ocallahan.org/2018/09/more-realistic-goals-for-c-lifetimes-10.html
    - http://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines
    - https://github.com/isocpp/CppCoreGuidelines/blob/master/docs/Lifetime.pdf
* https://rust-lang.github.io/rustc-guide/
* https://doc.rust-lang.org/nightly/nightly-rustc/rustc/index.html
* https://os.phil-opp.com/
    - writing-an-os-in-rust
    * https://github.com/rustcc/writing-an-os-in-rust
+ http://web.eecs.utk.edu/~smarz1/osblog/
    * Making a RISC-V Operating System using Rust
* https://fy.blackhats.net.au/blog/html/2019/07/16/cpu_atomics_and_orderings_explained.html
* https://github.com/lizhuohua/linux-kernel-module-rust
    * Writing Linux Kernel Module in Rust
>>>>>>> fb6f9ecbf864e0b460f4a0a08f6f8c69a21142af
* https://medium.com/@richardanaya/a-journey-through-rust-lifetimes-5a08782c7091
* https://matklad.github.io/2019/07/16/perils-of-constructors.html
* https://www.reddit.com/r/rust/comments/c66dtz/async_parallelize_your_shell_commands/
* https://www.reddit.com/r/rust/comments/c6hbc5/neqo_mozillas_rust_quic_implementation/
* https://medium.com/@richardanaya/a-journey-through-rust-lifetimes-5a08782c7091
* https://blog.x5ff.xyz/blog/easy-programming-with-rust-macros/
    - https://github.com/azriel91/proc_macro_roids
        +  make writing proc macros more easy
* https://medium.com/journey-to-rust/rust-type-language-48e1c43b1ef4
* https://www.ibm.com/developerworks/cn/opensource/os-developers-know-rust/
* https://zhuanlan.zhihu.com/p/73921538
* https://www.redox-os.org/news/rsoc-ptrace-2/
    - 为Redox OS实现ptrace Part 2
* https://blog.ryanlevick.com/DMG-01/public/book/
    - 使用Rust从零开始制作任天堂GameBoy模拟器
* https://github.com/whoiscc/shattuck
* https://estada.ch/2019/6/7/rusts-hidden-talents/
* https://m.aliyun.com/yunqi/articles/62505
* https://www.zhihu.com/question/31038569
* https://www.zhihu.com/question/30407715
* https://mgattozzi.com/turning-github-into-your-own-registry/
* https://blog.sentry.io/2019/06/13/building-a-sentry-symbolicator
* https://zhuanlan.zhihu.com/p/69269688
* https://ngoldbaum.github.io/posts/project-euler/
* https://www.reddit.com/r/rust/comments/c33u9m/the_typestate_pattern_in_rust/
* https://content.riscv.org/wp-content/uploads/2019/06/14.05-building_secure_systems-1.pdf
* https://medium.com/swlh/on-memoization-291fd1dd924
* https://ngoldbaum.github.io/posts/helpful-rust-cli-crates/
* https://chilimatic.hashnode.dev/experiment-with-streams-reading-files-with-futures-cjx1q0gmo001eurs1pt0c27kz
* https://www.linuxjournal.com/content/getting-started-rust-working-files-and-doing-file-io
* https://medium.com/apolitical-engineering/how-do-you-impl-display-for-vec-b8dbb21d814f
* http://kmdouglass.github.io/posts/a-simple-plugin-interface-for-the-rust-ffi/
* https://gregoryszorc.com/blog/2019/06/24/building-standalone-python-applications-with-pyoxidizer/
* https://gist.github.com/edmundsmith/855fcf0cb35dd467c29a9350481f0ecf
    - Rust中模拟高阶类型的方法
        + 该文作者提出了一种方法，通过类型参数向下转换泛型trait来模拟当前Rust中的高阶类型/泛型关联类型，并且提供了使用该方法在Rust中创建Functors，Applicatives和Monads的简单示例。
+ https://amos.me/blog/2019/rust-modules-vs-files/
+ https://ehsanmkermani.com/2019/07/03/rust-std-study-series-alloc/
+ http://rust-lang.github.io/compiler-team
+ https://www.forrestthewoods.com/blog/should-small-rust-structs-be-passed-by-copy-or-by-borrow/
+ https://iolivia.me/posts/6-months-of-rust-game-dev/
+ https://rfdonnelly.github.io/posts/using-tree-sitter-parsers-in-rust/
    * https://tree-sitter.github.io/tree-sitter/
+ https://parallel-rust-cpp.github.io/introduction.html

## web
+ https://book.async.rs/introduction.html
+ https://huangjj27.github.io/async-book/index.html
+ https://www.steadylearner.com/blog/read/How-to-write-Full-Stack-Rust-code
+ https://medium.com/nearprotocol/rust-parallelism-for-non-c-c-developers-ec23f48b7e56
+ https://www.reddit.com/r/rust/comments/c7292d/asyncawait_simple_http_server_with_epoll/
    * https://github.com/murphysean/betarustasyncawait
* https://github.com/brson/basic-http-server
* async
    - https://github.com/rust-lang/async-book
    - https://www.reddit.com/r/rust/comments/c71f03/im_a_phd_student_building_a_fast_research/
    - https://github.com/jonhoo
    - https://www.youtube.com/watch?v=9_3krAQtD2k
    - https://community.libra.org/t/async-await-in-libra-core/1566
    - https://github.com/lrlna/sketchin/blob/master/zines/async-rust.md
    - http://fitzgeraldnick.com/2019/08/27/async-stacks-in-rust.html
    - https://ragona.com/posts/clobber_async_await
* https://blog.yoshuawuyts.com/async-log/
* https://www.snoyman.com/blog/2018/12/rust-crash-course-07-async-futures-tokio
* https://speakerdeck.com/_rvidal/concurrency-in-rust-is-boring
* https://www.reddit.com/r/rust/comments/c326e0/rust_streams/
* https://medium.com/swlh/writing-a-proxy-in-rust-and-why-it-is-the-language-of-the-future-265d8bf7c6d2
    - https://github.com/sozu-proxy/sozu
* https://github.com/tokio-rs/tracing
+ https://github.com/mozilla/application-services
+ https://github.com/mozilla/neqo
+ https://gill.net.in/posts/auth-microservice-rust-actix-web1.0-diesel-complete-tutorial/
+ https://github.com/Byron/github-star-counter
    * 供学习 Rust异步编程

## oop
- https://oribenshir.github.io/afternoon_rusting/blog/rust-for-oop
- https://oribenshir.github.io/afternoon_rusting//blog/project-management
- https://oribenshir.github.io/afternoon_rusting/blog/enum-and-pattern-matching-part-1
- https://oribenshir.github.io/afternoon_rusting/blog/enum-and-pattern-matching-part-2
- https://chilimatic.hashnode.dev/threads-in-rust-cjwmbxw9e003pzjs19n7pa0bt

## lock
- https://preshing.com/20120612/an-introduction-to-lock-free-programming
- https://preshing.com/20120625/memory-ordering-at-compile-time
- https://preshing.com/20120710/memory-barriers-are-like-source-control-operations
- https://preshing.com/20120913/acquire-and-release-semantics
- https://preshing.com/20120930/weak-vs-strong-memory-models
- https://preshing.com/20121019/this-is-why-they-call-it-a-weakly-ordered-cpu
- https://mtak-blog.github.io/are-we-lock-free-yet
* https://cfsamson.gitbook.io/green-threads-explained-in-200-lines-of-rust/

## closure
+ https://medium.com/swlh/understanding-closures-in-rust-21f286ed1759
- https://oribenshir.github.io/afternoon_rusting/blog/closures

## GUI
+ https://www.reddit.com/r/rust/comments/c9l2ow/speedy_desktop_apps_with_gtk_and_rust/

## misc
+ https://zhuanlan.zhihu.com/p/87922545
    * 从openresty谈到rust
    * 人生苦短，我用rust。
+ https://github.com/rust-unofficial/patterns
+ https://francismurillo.github.io/2019-07-31-Understanding-Rust-Through-AVL-Trees/
+ A closer look at Ownership in Rust
    * https://blog.thoughtram.io/ownership-in-rust/
+ https://raphaelgomes.dev/blog/articles/2019-07-01-sharing-references-between-python-and-rust.html
    * https://heptapod.octobus.net/gracinet/rust-cpython-shared-ref/tree/topic/default/lock_explicit_count
    * 在Python和Rust之间共享引用
+ https://gist.github.com/edmundsmith/855fcf0cb35dd467c29a9350481f0ecf
    * 通过类型参数向下转换泛型trait来模拟当前Rust中的高阶类型/泛型关联类型，并且提供了使用该方法在Rust中创建Functors，Applicatives和Monads的简单示例。
+ https://www.reddit.com/r/rust/comments/cethae/introducing_abscissa_a_securityoriented_rust/
+ https://rniczh.github.io/blog/lifetimes-intro/
+ https://medium.com/@jondot/my-key-learnings-after-30-000-loc-in-rust-a553e6403c19
+ https://github.com/SerhiiBilyk/Battleship
    * 一个 rust 小游戏，适合 rust 入门学习
* https://wiki.alopex.li/ActuallyUsingCrev
* https://www.joshmcguigan.com/blog/coverage-reports-code-reading-tool/
* 提高编译速度
    - http://antoyo.ml/compilation-time-dependencies
* 节省编译工程文件体积
    - https://medium.com/@edouard.oger/rust-caching-on-circleci-using-sccache-c996344f0115
    - https://llogiq.github.io/2018/10/17/space.html
        + https://www.reddit.com/r/rust/comments/9owc1o/more_space_for_cargo/
    - 静态链接导致太多重复东西, 各种test全都链一遍一个crate
    + 其实可以每六周升级Rust的时候删一次，反正不删也是要重新编译的
        * 只编译不替换
            - 所以要清理
                + cargo clean 就全都删除了, 要重新编译，花费时间久
                + 写脚本清理一个月前生成的文件？可能会误伤
                + 由 systemd 清理?
    + CI 的cache？
        + bin 的可以 cache, lib 的 cache 没有意义
        + 用sscache来做CI 上的 cache 就不怕爆炸了 
    - 用「同一个target 文件夹」来勉强省空间和编译时间
        + 把 target 目录人为指定, 设成共享target
        + ~/.cargo/config 里的 build.target-dir
        + 或 export CARGO_TARGET_DIR=$HOME/.cache/cargo
    - 有个cargo的工具可以自动删长期没用过的?


## OJ-related
__OJ__

+ https://github.com/bhuztez/porus
+ codewars

__solutions__

+ https://github.com/aylei/leetcode-rust
+ https://github.com/Aloxaf/LeetCode-Rust
+ https://github.com/Armavica/99-Problems-Rust
+ https://github.com/MaskRay/99-problems-rust

__算法/DS 库__

TODO
