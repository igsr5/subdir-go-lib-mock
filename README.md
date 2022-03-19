# go でリポジトリ内のサブディレクトリ内をライブラリとして公開できるかの実験

### `github.com/igsr5/subdir-go-lib-mock/subdir`
いけた
```sh
/→  ~/github.com/igsr5/protosum  /→   [arm64] [master] []
  %: /→ go get github.com/igsr5/subdir-go-lib-mock/subdir
go: downloading github.com/igsr5/subdir-go-lib-mock v0.0.0-20220319053301-7ec988fd7f85
go: downloading github.com/igsr5/subdir-go-lib-mock/subdir v0.0.0-20220319053301-7ec988fd7f85
go get: added github.com/igsr5/subdir-go-lib-mock/subdir v0.0.0-20220319053301-7ec988fd7f85
```

### `github.com/igsr5/subdir-go-lib-mock`
ダメだった
```sh
/→  ~/github.com/igsr5/protosum  /→   [arm64] [master] []
  %: /→ go run main.go
main.go:6:2: no required module provides package github.com/igsr5/subdir-go-lib-mock; to add it:
        go get github.com/igsr5/subdir-go-lib-mock
/
```
