# create date

- date

```bash
date
Sa 17. Aug 2024
```

- rustc --version

``` bash
rustc --version
rustc 1.80.1 (3f5fd8dd4 2024-08-06)
cargo --version
cargo 1.80.1 (376290515 2024-07-16)
```

## create rust project folder

```bash
cd 
cd workspace_rust
RUST_PROJECT_NAME="rust_test"
mkdir $RUST_PROJECT_NAME && cd $_
```

## init project

```bash
touch README.md \
&& ln -s README.md README \
&& cargo init "." \
&& cargo add rustfmt \
&& rustup component add rustfmt \
&& mkdir examples \
&& cp src/main.rs examples/example.rs \
&& sed -i -e 's/world/example/g' examples/example.rs \
&& rustup  show \
&& rustup  check \
&& rustup toolchain uninstall stable \
&& rustup toolchain install stable \
&& rustup update  --force \
&& rustup show \
&& cargo add rustfmt \
&& rustup component add rustfmt \
&& rustup show \
&& touch FROM_HERE.md \
&& cargo --version \
&& rustc --version
```

## build plain project

```bash
cargo build
```
