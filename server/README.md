== SERVER TERMINAL ==
go get google.golang.org/protobuf/cmd/protoc-gen-go
go get google.golang.org/grpc/cmd/protoc-gen-go-grpc
go install google.golang.org/protobuf/cmd/protoc-gen-go
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest

== PROTO TERMINAL ==
protoc calculator.proto --go_out=../server
protoc calculator.proto --go-grpc_out=../server
protoc calculator.proto --go_out=../server --go-grpc_out=../server
chmod +x gen.sh
./gen.sh

== SERVER TERMINAL ==
go get google.golang.org/grpc

== CLIENT TERMINAL ==
go get google.golang.org/protobuf/cmd/protoc-gen-go
go get google.golang.org/grpc

CODEBANGKOK
https://www.youtube.com/watch?v=_F7qqth3WWw