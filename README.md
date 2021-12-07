# 🎄 Go cover to Treemap

_Useful when you have large project with lots of files and packages_

```
$ go install github.com/nikolaydubina/go-cover-treemap@latest
$ go test -coverprofile cover.out ./...
$ go-cover-heatmap -coverprofile cover.out > out.svg
```

`github.com/gohugoio/hugo`
![example-hugo](docs/hugo.svg)

`github.com/gin-gonic/gin`
![example-gin](docs/gin.svg)

`github.com/go-chi/chi`
![example-chi](docs/chi.svg)

`github.com/nikolaydubina/treemap`
![example-treemap](docs/go-cover-treemap.svg)

`github.com/nikolaydubina/go-featureprocessing`
![example-go-featureprocessing](docs/go-featureprocessing.svg)

## Disclaimer

In all examples above I run `go test -coverprofile <my-file> ./...`.
I did not do any special setup.
Some projects may reuqire additional steps to properly run tets and generate full coverprofile.
What you see is "lower bound" of coverage for those projects.
All profiles generated on `main` branch of each project in GitHub on 2021-12-07.

## Contributions

Welcomed! Add pretty color palettes! Add interesting examples!

## Reference

* Official Go tool to make HTML from cover profile: https://github.com/golang/go/blob/master/src/cmd/cover/html.go#L97
* Official Go parser of cover profile `golang.org/x/tools/cover`: https://github.com/golang/tools/tree/master/cover
* Go SVG Treemap renderer with heatmap: github.com/nikolaydubina/treemap