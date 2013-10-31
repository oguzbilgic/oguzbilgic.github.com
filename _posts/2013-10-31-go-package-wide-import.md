---
layout: post 
title: Proposal for Package-wide Imports
---

# Proposal for Package-wide Imports

_October 2013_

In `go` language, you have to specify every single external or std package on top of each 
`.go` file they will be used. Here is an example usage of `import` statement from popular
docker linux conatier project.

```go
import (
        "encoding/binary"
        "errors"
        "fmt"
        "github.com/dotcloud/docker/iptables"
        "github.com/dotcloud/docker/netlink"
        "github.com/dotcloud/docker/proxy"
        "github.com/dotcloud/docker/utils"
        "log"
        "net"
        "strconv"
        "sync"
)
```

This explicit import statements make code very readable, since you can immediatly follow which 
function/struct/interface comes from which external package. However, having explicit import 
statement with the urls of external pacakges in each source code file in you packages sometimes 
becomes diffucult to maintain.

My proposal for this problem is creating some sort of global or package-wide import statement. Let's
call it `gimport` for now. So either in your package's `main.go` file or `import.go` file you specify 
the external dependencies once and those packages become available for all the `.go` files in your pacages.

Here is an example `import.go` file, for docker example above:

```go
gimport (
        "github.com/dotcloud/docker/iptables"
        "github.com/dotcloud/docker/netlink"
        "github.com/dotcloud/docker/proxy"
        "github.com/dotcloud/docker/utils"

)
```

Such a statement would decrease the code duplication, decouple the source code files and paths' of 
the external packages, and finally would make it more readable and maintainable since most of the 
required external packages are just listed in just one file.
