# Contributing

First off, thank you for considering contributing to Rust GitHub Template.

If your contribution is not straightforward, please first discuss the change you
wish to make by creating a new issue before making the change.

## Reporting issues

Try to use a clear title, and describe your problem with complete sentences.

## Pull requests

Try to do one pull request per change.

## GitHub Actions

{% raw  %}

When we have to mix GitHub actions variables with the `{{ }}` liquid syntax,
GitHub actions variable are written in the format
`{{ "{{ github.variable " }}}}` instead of `{{ github.variable }}`.

Of course, when doing `cargo generate` the ugly version is replaced with the expected
one.

See [Continuous delivery](https://github.com/rust-github/template/blob/master/.github/workflows/cd.yml)
as an example.

{% endraw  %}
