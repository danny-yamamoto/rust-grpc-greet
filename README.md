# rust-grpc-greet
Rewrite go-connect-greet with Rust.

```bash
# install asdf
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.13.1
asdf
. "$HOME/.asdf/asdf.sh"
asdf
# install grpcrl
asdf plugin add grpcurl
asdf list all grpcurl
asdf install grpcurl 1.8.8
asdf local grpcurl 1.8.8
# check api
grpcurl -plaintext localhost:50051 list
grpcurl -plaintext -d '{"name": "World"}' localhost:50051 hello.HelloService/SayHello
```
