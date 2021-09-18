# Rust-Environment

- Rustとは


- インストール

```
$ curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
$ export PATH="$HOME/.cargo/bin:$PATH"
```

- プロジェクト作成

```
$ cargo new hello(プロジェクト名) --bin
$ cd hello
```

- コンパイル

コンパイルだけ行うには** build ** を、コンパイルして実行するには** run **を行います。

```
$ cargo build		// コンパイルだけ行う
$ cargo run		// コンパイルして実行する
```

上記のコンパイルはデバッグ機能を含めた、開発用のコンパイルになっています。
**--release** をつけることで、リリース用のコンパクトで高速なバイナリを作成することができます。

```
$ cargo build --release
```
