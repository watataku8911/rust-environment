# Rust-Environment

[参照](https://rust-lang.org/ja/tools/install)

- Rustとは

Rustは、性能、メモリ安全性、安全な並行性を目指して設計されたマルチパラダイムのプログラミング言語である。C言語、C++に代わるシステムプログラミング言語を目指しており、構文的にはC++に似ているが、「ボローチェッカー」 で参照の有効性を検証することによってメモリ安全性を保証できる。

- インストール

```
$ curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
$ export PATH="$HOME/.cargo/bin:$PATH"
```
インストール後にこのコマンドを叩いてバージョンが出ればインストール完了。

```
$ rustc --version
```

- アンインストール

```
$ rustup self uninstall
```

## Hello Would!!

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
