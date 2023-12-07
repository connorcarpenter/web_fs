# web_fs

On native platforms, this crate just re-exports the [`std::fs`] module.

On wasm32-unknown-unknown, this crate provides equivalent functionality, using the [`Origin Private File System`] of the File System API.

Basically, the intention of this crate is to make [`std::fs`] functional on wasm32-unknown-unknown.

[`std::fs`]: https://doc.rust-lang.org/std/fs/index.html
[`Origin private file system`]: https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system.