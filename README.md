## TODO PLANNING PROJECT : https://github.com/mkaganm/todo-planning

#### SET GO ENVIRONMENT
```bash
export PATH="$PATH:$(go env GOPATH)/bin"
```

#### GENERATE CODE FROM PROTO FILES
```bash
protoc --go_out=. --go_opt=paths=source_relative \
    --go-grpc_out=. --go-grpc_opt=paths=source_relative \
    provider.proto
```