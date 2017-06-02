# pointer
[![GoDoc](https://godoc.org/github.com/morikuni/pointer?status.svg)](https://godoc.org/github.com/morikuni/pointer)

pointer is a library to create a pointer value for primitive types.

## Usage

```go
package main

import (
	"fmt"

	"github.com/morikuni/pointer"
)

func main() {
	var i *int = pointer.Int(1)
	var u *uint8 = pointer.Uint8(2)
	var p *uintptr = pointer.Uintptr(0xabcdef)
	var f *float64 = pointer.Float64(3.14)
	var s *string = pointer.String("hello")
	var r *rune = pointer.Rune('a')
	var b *bool = pointer.Bool(true)
	var x *byte = pointer.Byte(0xfe)
	var c *complex128 = pointer.Complex128(3 + 4i)

	fmt.Println(*i, *u, *p, *f, *s, *r, *b, *x, *c)
}

```
