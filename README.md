# slug

`slug` is a package that sanitizes and normalizes strings for use in things like
URLs:

```go
package main

import github.com/stvp/slug

func main() {
  slug.Clean("L'école 24") // "l_ecole_24"
  slug.Clean("\x00\x08clean") // "clean"
}
```

You can also customize the replacement string:

```go
package main

import github.com/stvp/slug

func main() {
  slug.Replacement = '-'
  ...
}
```

[API docs](http://go.pkgdoc.org/github.com/stvp/slug).

