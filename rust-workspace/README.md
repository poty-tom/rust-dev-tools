# cargo workspace
cargoの`workspace`機能

## メンバーの定義

- Cargo.toml
```
[workspace]
members = ["member1", "member2", "member3"]

```

## 依存管理
- Cargo.toml
```
[workspace.dependecies]
member1 = { path = "./member1" }
member2 = { path = "./member2" }
member3 = { path = "./member3" }
その他一元管理したいクレートなど

[dependencies]
member1.workspace = true
member2.workspace = true
member3.workspace = true
共通のクレート.workspace = true
```
