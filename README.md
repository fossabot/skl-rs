<div align="center">
<h1>SKL</h1>
</div>
<div align="center">



[<img alt="github" src="https://img.shields.io/badge/github-skl--rs-8da0cb?style=for-the-badge&logo=Github" height="22">][Github-url]
[<img alt="Build" src="https://img.shields.io/github/workflow/status/al8n/skl-rs/CI/main?logo=Github-Actions&style=for-the-badge" height="22">][CI-url]
[<img alt="codecov" src="https://img.shields.io/codecov/c/gh/al8n/skl-rs?style=for-the-badge&token=aek5JwyaAZ&logo=codecov" height="22">][codecov-url]

[<img alt="docs.rs" src="https://img.shields.io/badge/docs.rs-skl--rs-66c2a5?style=for-the-badge&labelColor=555555&logo=data:image/svg+xml;base64,PHN2ZyByb2xlPSJpbWciIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgdmlld0JveD0iMCAwIDUxMiA1MTIiPjxwYXRoIGZpbGw9IiNmNWY1ZjUiIGQ9Ik00ODguNiAyNTAuMkwzOTIgMjE0VjEwNS41YzAtMTUtOS4zLTI4LjQtMjMuNC0zMy43bC0xMDAtMzcuNWMtOC4xLTMuMS0xNy4xLTMuMS0yNS4zIDBsLTEwMCAzNy41Yy0xNC4xIDUuMy0yMy40IDE4LjctMjMuNCAzMy43VjIxNGwtOTYuNiAzNi4yQzkuMyAyNTUuNSAwIDI2OC45IDAgMjgzLjlWMzk0YzAgMTMuNiA3LjcgMjYuMSAxOS45IDMyLjJsMTAwIDUwYzEwLjEgNS4xIDIyLjEgNS4xIDMyLjIgMGwxMDMuOS01MiAxMDMuOSA1MmMxMC4xIDUuMSAyMi4xIDUuMSAzMi4yIDBsMTAwLTUwYzEyLjItNi4xIDE5LjktMTguNiAxOS45LTMyLjJWMjgzLjljMC0xNS05LjMtMjguNC0yMy40LTMzLjd6TTM1OCAyMTQuOGwtODUgMzEuOXYtNjguMmw4NS0zN3Y3My4zek0xNTQgMTA0LjFsMTAyLTM4LjIgMTAyIDM4LjJ2LjZsLTEwMiA0MS40LTEwMi00MS40di0uNnptODQgMjkxLjFsLTg1IDQyLjV2LTc5LjFsODUtMzguOHY3NS40em0wLTExMmwtMTAyIDQxLjQtMTAyLTQxLjR2LS42bDEwMi0zOC4yIDEwMiAzOC4ydi42em0yNDAgMTEybC04NSA0Mi41di03OS4xbDg1LTM4Ljh2NzUuNHptMC0xMTJsLTEwMiA0MS40LTEwMi00MS40di0uNmwxMDItMzguMiAxMDIgMzguMnYuNnoiPjwvcGF0aD48L3N2Zz4K" height="20">][doc-url]
[<img alt="crates.io" src="https://img.shields.io/crates/v/skl-rs?style=for-the-badge&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iaXNvLTg4NTktMSI/Pg0KPCEtLSBHZW5lcmF0b3I6IEFkb2JlIElsbHVzdHJhdG9yIDE5LjAuMCwgU1ZHIEV4cG9ydCBQbHVnLUluIC4gU1ZHIFZlcnNpb246IDYuMDAgQnVpbGQgMCkgIC0tPg0KPHN2ZyB2ZXJzaW9uPSIxLjEiIGlkPSJMYXllcl8xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIiB4PSIwcHgiIHk9IjBweCINCgkgdmlld0JveD0iMCAwIDUxMiA1MTIiIHhtbDpzcGFjZT0icHJlc2VydmUiPg0KPGc+DQoJPGc+DQoJCTxwYXRoIGQ9Ik0yNTYsMEwzMS41MjgsMTEyLjIzNnYyODcuNTI4TDI1Niw1MTJsMjI0LjQ3Mi0xMTIuMjM2VjExMi4yMzZMMjU2LDB6IE0yMzQuMjc3LDQ1Mi41NjRMNzQuOTc0LDM3Mi45MTNWMTYwLjgxDQoJCQlsMTU5LjMwMyw3OS42NTFWNDUyLjU2NHogTTEwMS44MjYsMTI1LjY2MkwyNTYsNDguNTc2bDE1NC4xNzQsNzcuMDg3TDI1NiwyMDIuNzQ5TDEwMS44MjYsMTI1LjY2MnogTTQzNy4wMjYsMzcyLjkxMw0KCQkJbC0xNTkuMzAzLDc5LjY1MVYyNDAuNDYxbDE1OS4zMDMtNzkuNjUxVjM3Mi45MTN6IiBmaWxsPSIjRkZGIi8+DQoJPC9nPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPC9zdmc+DQo=" height="22">][crates-url]
[<img alt="rustc" src="https://img.shields.io/badge/MSRV-1.56.0-fc8d62.svg?style=for-the-badge&logo=Rust" height="22">][rustc-url]

[<img alt="license-apache" src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=for-the-badge&logo=Apache" height="22">][license-apache-url]
[<img alt="license-mit" src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge&fontColor=white&logoColor=f5c076&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMzZweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMzZweCIgZmlsbD0iI2Y1YzA3NiI+PHBhdGggZD0iTTAgMGgyNHYyNEgwVjB6IiBmaWxsPSJub25lIi8+PHBhdGggZD0iTTEwLjA4IDEwLjg2Yy4wNS0uMzMuMTYtLjYyLjMtLjg3cy4zNC0uNDYuNTktLjYyYy4yNC0uMTUuNTQtLjIyLjkxLS4yMy4yMy4wMS40NC4wNS42My4xMy4yLjA5LjM4LjIxLjUyLjM2cy4yNS4zMy4zNC41My4xMy40Mi4xNC42NGgxLjc5Yy0uMDItLjQ3LS4xMS0uOS0uMjgtMS4yOXMtLjQtLjczLS43LTEuMDEtLjY2LS41LTEuMDgtLjY2LS44OC0uMjMtMS4zOS0uMjNjLS42NSAwLTEuMjIuMTEtMS43LjM0cy0uODguNTMtMS4yLjkyLS41Ni44NC0uNzEgMS4zNlM4IDExLjI5IDggMTEuODd2LjI3YzAgLjU4LjA4IDEuMTIuMjMgMS42NHMuMzkuOTcuNzEgMS4zNS43Mi42OSAxLjIuOTFjLjQ4LjIyIDEuMDUuMzQgMS43LjM0LjQ3IDAgLjkxLS4wOCAxLjMyLS4yM3MuNzctLjM2IDEuMDgtLjYzLjU2LS41OC43NC0uOTQuMjktLjc0LjMtMS4xNWgtMS43OWMtLjAxLjIxLS4wNi40LS4xNS41OHMtLjIxLjMzLS4zNi40Ni0uMzIuMjMtLjUyLjNjLS4xOS4wNy0uMzkuMDktLjYuMS0uMzYtLjAxLS42Ni0uMDgtLjg5LS4yMy0uMjUtLjE2LS40NS0uMzctLjU5LS42MnMtLjI1LS41NS0uMy0uODgtLjA4LS42Ny0uMDgtMXYtLjI3YzAtLjM1LjAzLS42OC4wOC0xLjAxek0xMiAyQzYuNDggMiAyIDYuNDggMiAxMnM0LjQ4IDEwIDEwIDEwIDEwLTQuNDggMTAtMTBTMTcuNTIgMiAxMiAyem0wIDE4Yy00LjQxIDAtOC0zLjU5LTgtOHMzLjU5LTggOC04IDggMy41OSA4IDgtMy41OSA4LTggOHoiLz48L3N2Zz4=" height="22">][license-mit-url]

A lock-free thread-safe skiplist implementation (no_std) for writing memery table, SST table or something else.
skl-rs is a pure Rust implementation for https://github.com/dgraph-io/badger/tree/master/skl


English | [简体中文][zh-cn-url]

</div>

## Installation
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fal8n%2Fskl-rs.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fal8n%2Fskl-rs?ref=badge_shield)

```toml
[dependencies]
skl = "0.2"
```

## Support Platforms
| targets                       |   status  |
|:-----------------------------:|:---------:|
| aarch64-linux-android         |  &#9989;  |
| aarch64-unknown-linux-gnu     |  &#9989;  |
| aarch64-unknown-linux-musl    |  &#9989;  |
| i686-pc-windows-gnu           |  &#9989;  |
| i686-linux-android            |  &#9989;  |
| i686-unknown-linux-gnu        |  &#9989;  |
| mips64-unknown-linux-gnuabi64 |  &#9989;  |
| powerpc64-unknown-linux-gnu   |  &#9989;  |
| riscv64gc-unknown-linux-gnu   |  &#9989;  |
| wasm32-unknown-unknown        |  &#9989;  |
| wasm32-unknown-emscripten     |  &#9989;  |
| x86_64-unknown-linux-gnu      |  &#9989;  |
| x86_64-pc-windows-gnu         |  &#9989;  |
| x86_64-linux-android          |  &#9989;  |

## Example
```rust
use skl::FixedSKL;

fn main() {
    const N: usize = 1000;
    let l = FixedSKL::new(1 << 20);
    let wg = Arc::new(());
    for i in 0..N {
        let w = wg.clone();
        let l = l.clone();
        std::thread::spawn(move || {
            l.insert(key(i), new_value(i));
            drop(w);
        });
    }
    while Arc::strong_count(&wg) > 1 {}
    for i in 0..N {
        let w = wg.clone();
        let l = l.clone();
        std::thread::spawn(move || {
            assert_eq!(
                l.get(key(i)).unwrap().as_value_ref(),
                new_value(i).as_value_ref(),
                "broken: {i}"
            );
            drop(w);
        });
    }
}
```

## TODO (help wanted)
- [ ] make the crate test cases pass `cargo miri`

Thanks in advance for your helps!

#### License

`skl-rs` is under the terms of both the MIT license and the
Apache License (Version 2.0).

See [LICENSE-APACHE](LICENSE-APACHE), [LICENSE-MIT](LICENSE-MIT) for details.

Copyright (c) 2022 Al Liu.

[Github-url]: https://github.com/al8n/skl-rs/
[CI-url]: https://github.com/al8n/skl-rs/actions/workflows/ci.yml
[doc-url]: https://docs.rs/skl-rs
[crates-url]: https://crates.io/crates/skl-rs
[codecov-url]: https://app.codecov.io/gh/al8n/skl-rs/
[license-url]: https://opensource.org/licenses/Apache-2.0
[rustc-url]: https://github.com/rust-lang/rust/blob/master/RELEASES.md
[license-apache-url]: https://opensource.org/licenses/Apache-2.0
[license-mit-url]: https://opensource.org/licenses/MIT
[zh-cn-url]: https://github.com/al8n/skl-rs/tree/main/README-zh_CN.md


[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fal8n%2Fskl-rs.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fal8n%2Fskl-rs?ref=badge_large)