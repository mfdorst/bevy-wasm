# Bevy WASM
Scripts to setup, build and serve a bevy project in the browser.

## How to use

Copy `wasm-setup` and `wasm-build` into your bevy project.

## Setup WASM

Run
```sh
./wasm-setup
```
This will:
+ `cargo install` the following binaries if not already installed:
  + `wasm-bindgen-cli`
  + `basic-http-server`
  + `cargo-get`
+ Create a basic HTML file at `wasm/index.html` if one does not already exist
+ Add the rust cross-compilation target `wasm32-unknown-unknown`

## Build and serve your application

Run
```sh
./wasm-build
```

This will:
+ Build your application in `release` mode
+ Generate WASM bindings for your code with `wasm-bindgen`
+ Serve your application with `basic-http-server`

## Dependencies

It is assumed that you have `rustup` and `cargo` installed.

