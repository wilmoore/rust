# Rust
> opinionated Rust reference

## **Table of Contents**

- [Installation](#installation)

## Installation
> **OS**:`macOS`, **$SHELL**:`fish`

###### safe as possible install
```
~$ git clone https://github.com/rust-lang/rustup.rs.git $TMPDIR/rustup
~$ cd $TMPDIR/rustup
~$ ./rustup-init.sh --no-modify-path -y
```

###### add cargo to `$fish_user_paths`
```
~$ echo 'set -g fish_user_paths "$HOME/.cargo/bin" $fish_user_paths' > ~/.config/fish/conf.d/rust.fish
~$ source ~/.config/fish/conf.d/rust.fish
```

###### updates and components
```
~$ rustup self update
~$ rustup update
~$ rustup component add rust-src
~$ rustup component add rust-docs
```

###### completions
```
~$ mkdir -p ~/.config/fish/completions
~$ rustup completions fish > ~/.config/fish/completions/rust.fish
~$ source ~/.config/fish/completions/rust.fish
```

###### uninstall
```
~$ rm ~/.config/fish/completions/rust* ~/.config/fish/conf.d/rust*
~$ rm -rf ~/.cargo ~/.rustup
```
