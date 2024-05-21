```bash
cd ninegua/ic-nix
which dfx
nix-shell -A ic.binaries

cd dfinity/ic
cargo build --bin replica --release
sudo mv target/release/replica /nix/store/8gb2ikhz7c1qqgsppr4vjw1i5bahsv5n-dfx-env/bin/
sudo chown root:wheel /nix/store/8gb2ikhz7c1qqgsppr4vjw1i5bahsv5n-dfx-env/bin/replica
```

```bash
nix-shell dfx-env
dfx start --clean
```
