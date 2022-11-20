# hellocontainer
yum install golang

mkdir ~/go/src/hello_world

touch hello.go

vi hello.go

package main
import "fmt"

func main() {

        fmt.Println("hello, Go!")
}

go build hello.go

