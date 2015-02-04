Neo
====

Go Web Framework

## Installation

```bash
# framework
go get github.com/ivpusic/neo

# CLI tool
go get github.com/ivpusic/neo
```

# Documentation
[Project Site](http://ivpusic.github.io/neo)

[API Documentation](http://godoc.org/github.com/ivpusic/neo)

## Example

Create Neo application
```bash
neo new myapp
cd myapp
```

```Go
package main

import (
    "github.com/ivpusic/neo"
)

func main() {
    app := neo.App()

    app.Get("/", func(this *neo.Ctx) {
        this.Res.Text("I am Neo Programmer", 200)
    })

    app.Start()
}
```

Run it!
```bash
neo run main.go
```

## License
*MIT*
