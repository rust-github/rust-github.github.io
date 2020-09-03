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

At the moment GitHub actions have variables with a strange syntax:
`{{ "{{ github.variable " }}}}` instead of `{{ github.variable }}`.

This is because the `{{ }}` syntax is the one used by liquid, and so there is a conflict.
Of course, when doing `cargo generate` the ugly version is replaced with the expected
one.

When a version > 0.5.0 of `cargo generate` is released, we will be able to use
[raw](https://shopify.github.io/liquid/tags/raw/) tags, in order to make the
actions cleaner.

{% endraw  %}
