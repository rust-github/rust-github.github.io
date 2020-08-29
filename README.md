# Rust Github Template Website

Rust Github Template [Website](https://rust-github.github.io) repository.

## Build locally

If you want to build this website locally:

* clone this repository:

  ```sh
  git clone https://github.com/rust-github/rust-github.github.io
  ```

* go inside the directory:

  ```sh
  cd rust-github.github.io
  ```

At this point you can either use docker or not:

### Docker

* run the [github-pages](https://github.com/Starefossen/docker-github-pages) container:

  ```sh
  docker run -it --rm -v "$PWD":/usr/src/app -p "4000:4000" starefossen/github-pages
  ```

* Open the link `http://localhost:4000` in your web browser

### Manuale

* Install ruby
* Install bundler: `$ gem install bundler`
* Install Jekyll and the other dependencies: `$ bundle install`
* Run the server locally: `$ bundle exec jekyll serve`
* Open the link `http://localhost:4000` in your web browser
