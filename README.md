Implementation following the proto bufs tutorial here:
[https://protobuf.dev/getting-started/gotutorial/](https://protobuf.dev/getting-started/gotutorial/)

## Generating code
From the project root:
```
protoc --go_out=.  ./addressbook.proto
```
* `--go_out` indicates you want go language files as the output