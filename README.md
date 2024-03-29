# My place of slides

## Slides

- [AWSドキュメント自動化のススメ](https://yusabana.github.io/slides/docs/20170714-lt_sgdoc/)

## Building

Use live-server.

```
$ yarn run live-server
```

You can access `http://localhost:8888/SLIDE_DIRECTORY/`

## Generate pdf(using decktape)

I use decktape as a git-submodule.  
you can use update git-submodule as a below.  
[Git submoduleの抑えておきたい理解ポイントのまとめ - Qiita](http://qiita.com/kinpira/items/3309eb2e5a9a422199e9)

```
$ git submodule            # check for submodule status
$ git submodule update -i  # update submodule
```

Generate pdf and screenshots. Rename use slides directory at [SLIDE_DIRECTORY].

```
$ yarn run decktape -- http://127.0.0.1:8888/slides/[SLIDE_DIRECTORY]/index.html slides.pdf
```

## Thanks

- [ahomu/Talkie: Simple slide presentation library. Responsive scaling & markdown ready.](https://github.com/ahomu/Talkie)
- [astefanutti/decktape: PDF exporter for HTML presentation frameworks](https://github.com/astefanutti/decktape)
