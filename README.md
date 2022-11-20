# hellocontainer
yum install golang

mkdir ~/github/hellocontainer

cd ~/github/hellocontainer

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin git@github.com:aleberkn/hellocontainer.git

git push -u origin main

#failed - github no longer allows passwords.  follow instructions on creating and using an ssh key for github authentication

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

steps to create an ssh key for github

Create a new SSH key using your github email as a label.
ssh-keygen -t ed25519 -C "aleberkn@gmail.com"

add the new SSH key to the ssh-agent to manage your keys
$ eval "$(ssh-agent -s)"
> Agent pid 59566

add you ssh key to the ssh agent
ssh-add ~/.ssh/id_ed25519

touch hello.go

vi hello.go

package main
import "fmt"

func main() {

        fmt.Println("hello, Go!")
}

go build hello.go

