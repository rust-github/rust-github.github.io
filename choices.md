# Choices

In the following we give the reasoning behind some of the choices taken by this
project.

## License

License related choices follow the
[api-guidelines](https://rust-lang.github.io/api-guidelines/necessities.html#crate-and-its-dependencies-have-a-permissive-license-c-permissive).

## Continuous delivery

In order to cross-compile for i686 and arm64 architectures on linux, we use
[cross](https://github.com/rust-embedded/cross) thanks to the
[actions-rs/cargo](https://github.com/actions-rs/cargo) GitHub action.

These architectures were chosen because they are
[tier 1](https://doc.rust-lang.org/nightly/rustc/platform-support.html).
Feel free to add other architectures in your project if you need them.
