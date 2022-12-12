# hellocontainer
yum install golang

touch hello.go

vi hello.go

## source to say hello

package main
import "fmt"

func main() {

        fmt.Println("hello, Go!")
}

go build hello.go

