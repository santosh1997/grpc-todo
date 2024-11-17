## Proto Generation

protoc --proto_path=protos \
    --go_out=./server/generated --go_opt=paths=source_relative \
    --go-grpc_out=./server/generated --go-grpc_opt=paths=source_relative \
    protos/**/*.proto

