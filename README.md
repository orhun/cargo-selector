# cargo-selector

[![Crate Status](https://img.shields.io/crates/v/cargo-selector.svg)](https://crates.io/crates/cargo-selector)

Cargo subcommand to select and execute binary/example targets

<img src="./img/demo.gif" width=600>

(This demo uses [Ratatui](https://github.com/ratatui-org/ratatui) as an example!)

## Installation

```
$ cargo install cargo-selector
```

## Usage

```
$ cargo selector
```

Then, target list will be displayed, and you can execute the following command by selecting it.

```sh
# if the target is bin
$ cargo run --bin xyz [--features "foo bar"]

# if the target is example
$ cargo run --example xyz [--features "foo bar"]
```

### Keybindings

| Key                               | Description                                  |
| --------------------------------- | -------------------------------------------- |
| <kbd>Down</kbd> <kbd>Ctrl+n</kbd> | cursor down                                  |
| <kbd>Up</kbd> <kbd>Ctrl+p</kbd>   | cursor up                                    |
| <kbd>Enter</kbd>                  | execute `cargo run --bin/example <selected>` |
| <kbd>Esc</kbd> <kbd>Ctrl+c</kbd>  | quit                                         |

## License

MIT