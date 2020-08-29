# Introduction

Creating a new Rust project is as easy as typing `cargo new <project_name>`,
but often you need more than what `cargo new` gives you.

This is when [cargo generate](https://github.com/ashleygwilliams/cargo-generate)
comes into play:

> cargo-generate is a developer tool to help you get up and running quickly
  with a new Rust project by leveraging a pre-existing git repository as a template.

[Rust GitHub Template](https://github.com/rust-github/template) (this project)
is a template for `cargo generate` that aims to be a starting point suitable for
the vast majority of rust projects that will be hosted on GitHub.

Stop copy pasting tons of markdown and yaml files each time you start a new
rust project. Let's create them only once, together!

## Template content

### GitHub Actions

* [security checks](https://github.com/rust-github/template/blob/master/.github/workflows/audit.yml)
* [continuous integration](https://github.com/rust-github/template/blob/master/.github/workflows/ci.yml):
  * tests
  * rustfmt
  * clippy
  * code coverage update
* [continuous delivery](https://github.com/rust-github/template/blob/master/.github/workflows/cd.yml):
  * publish release for mac, linux and windows
  * publish to cargo

### Documentation

* Installation instructions
* README badges
  * crates.io
  * docs.rs
  * GitHub Actions CI
  * Test coverage
* Licenses (MIT or APACHE)
* [Changelog](https://github.com/rust-github/template/blob/master/CHANGELOG.md)
* [Contributing guidelines](https://github.com/rust-github/template/blob/master/CONTRIBUTING.md)
* [Code of conduct](https://github.com/rust-github/template/blob/master/CODE_OF_CONDUCT.md)
* [Issue templates](https://github.com/rust-github/template/tree/master/.github/ISSUE_TEMPLATE)
* [Pull request template](https://github.com/rust-github/template/blob/master/.github/PULL_REQUEST_TEMPLATE.md)

## Instructions

* create a [new](https://github.com/new) empty repository (do not initialize it
  with a README, a `.gitignore` or a license).
* clone the repository on your machine and `cd` into it.
* Install `cargo generate`

  ```sh
  cargo install cargo-generate
  ```

* create your project with this template

  ```sh
  cargo generate --git https://github.com/rust-github/template.git
  ```

* replace all occurences of `{[username]}` with your GitHub username.
  This is required until [#164](https://github.com/ashleygwilliams/cargo-generate/pull/164)
  isn't merged.
  For example if you use [sd](https://github.com/chmln/sd), from the project
  root directory run the command:

  ```sh
  sd {[username]} MyUsername
  ```

* edit your project: this is just a template, edit your project according to
  your own needs by adding what's necessary and removing what you don't like.

### Crates.io

Set up your crates.io token in a
[GitHub secret](https://docs.github.com/en/actions/configuring-and-managing-workflows/creating-and-storing-encrypted-secrets)
called `CARGO_API_KEY`.

For more info about the crates.io toeken, see
[The Cargo Book](https://doc.rust-lang.org/cargo/reference/publishing.html).

### Code coverage

* [sign up](https://coveralls.io/sign-up) to coveralls
* [add](https://coveralls.io/repos/new) your repo

## Supporting Rust Github Template

The best way to support the project is to contribute to it either by reporting
problems, ideas or sending pull requests.

If you created your project by using Rust GitHub Template, and you want to show
it, you can use our badge:
[![Rust GitHub template](https://img.shields.io/badge/Rust%20GitHub-Template-blue)](https://rust-github.github.io/)

* For Markdown:

  ```markdown
  [![Rust GitHub Template](https://img.shields.io/badge/Rust%20GitHub-Template-blue)](https://rust-github.github.io/)
  ```

* For HTML:

  ```html
  <a href="https://rust-github.github.io/"><img alt="Rust GitHub Template" src="https://img.shields.io/badge/Rust%20GitHub-Template-blue" /></a>
  ```

Thank you! 🙏

## Links

* [choices explanation](choices.md)
* [credits](credits.md)
* [contributing](contrib.md)
