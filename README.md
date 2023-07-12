Implementation following the proto bufs tutorial here:
[https://protobuf.dev/getting-started/gotutorial/](https://protobuf.dev/getting-started/gotutorial/)  

As the tutorial doesn't go through the whole domain problem and supporting code in the same way the Java tutorial does I've lifted code from here [https://github.com/protocolbuffers/protobuf/blob/main/examples/go/](https://github.com/protocolbuffers/protobuf/blob/main/examples/go/)

## Generating code
From the project root:
```
protoc --go_out=.  ./addressbook.proto
```
* `--go_out` indicates you want go language files as the output

## Writing to a file
See [cmd/add_person/add_person.go](cmd/add_person/add_person.go).  
* Build the application `go build -o add_person cmd/add_person/add_person.go`
* Run `./add_person <address_book_file>`
* Answer the questions to have your person added to the file.

## Reading from a file  
See [cmd/list_people/list_people.go](cmd/list_people/list_people.go)
* Build the application go build -o list_people cmd/list_people/list_people.go
* Run `./list_people <address_book_file>`
* Answer the questions to have your person added to the file.