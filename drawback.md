# Drawback
+ https://iovxw.net/p/ugly-rust/
* https://www.reddit.com/r/rust/comments/c4nb27/what_are_the_things_you_hate_about_rust/
+ https://www.reddit.com/r/rust/comments/c0xwjd/all_i_hear_about_is_how_great_rust_is_what_isnt/
    * Compile times for large projects
    * Crate ecosystem is still very young, volatile and sparse
    * Because the community is young and still largely curiosity-driven, some essential crates have inconsistent maintenance since there aren't many maintainer organizations yet
    * Orphan rules make the glue-package approach (like Java uses) intractable and thus it's difficult to combine different parts of the ecosystem or factor libraries as much as one would like
    * Related to the above, we're probably still several years or editions away from a good dynamic linking/plugin story (but for good reason, related to the below)
    * The language's real potential still always seems one unimplemented RFC away (e.g., async, const generics, GATs, unsized rvalues, etc.)
    * A lot of the features really essential to write libraries of the quality one would like are still unstable (e.g., specialization)
    * Many crates have not yet reached version 1.0. This can make them more "scary" to use, as the API could change at any point.
    * std::net is quite lacking. For example, you can't perform a non-blocking connect. There is net2, but it has its own set of issues. Then there's socket2 to address net2's issues, but its API is a bit clunky. It's also not very popular, so it remains to be seen for how long it will stick around.
    * I think only recently was mirroring of crates.io introduced in a more sane way, though I don't remember exactly in what state.
    * Async IO is still clunky. MIO seeks to provide a nice API, but it's not zero-cost by any means. It also has some issues with Windows. I ended up having to use my own wrappers for epoll and kqueue, and used wepoll for Windows.
    * No crate namespacing, so you end up with crates like "yorickpeterse-socket2", "billy-bob-socket2", etc. This also means name squatting is more annoying.
    * This is not an issue with Rust itself, but is worth mentioning: I really can't stand Clippy. More often than not I upgrade it, and it introduces really annoying lints. For example, if you define len it will complain if you don't also define is_empty. This makes sense for a library, but when writing a self-contained application where you'd never use this it's annoying. Of course you can disable it, but I don't want to sprinkle Clippy directives all over the place.
    * No (computed) goto, or something that is guaranteed to compile down to it. This means interpreters won't be able to make use of them, slowing them down a bit (depending on the hardware)
