# hellocontainer
yum install golang

mkdir ~/go/src/hello_world.go

touch hello_container.go

vi hello_container.go

package main
import "fmt"

func main() {

        fmt.Println("hello, Go!")
}

go build hello.go

