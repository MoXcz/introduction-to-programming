---
weight: 4
title: "1.4 Why Go?"
---
# Why Go?

There's really no reason or justification for why Go is chosen to explain programming. I don't think there's any content in the book that would require using an *"easier"* language or specific language.

I like using Go and it's easy to read and to write with an abundant standard library, so I don't see any reason *not* to use Go. See the below example, it's an *HTTP server* that you can run with just having a basic Go installation and a few lines of code that are quite easy to read.

{{% hint info %}}
An HTTP server is some kind of device (in this case a program) that can listen to *requests* `http.Request` and *respond to them* `http.ResponseWriter` through HTTP
{{% /hint %}}

```go
package main

import (
	"fmt"
	"net/http"
	"time"
)

func handler(w http.ResponseWriter, r *http.Request) {
	fmt.Fprintf(w, "Hello World! %s", time.Now())
}

func main() {
	http.HandleFunc("/", handler)
	http.ListenAndServe(":8080", nil)
}
```

[> Next](/go/)
