# Hyperledger Fabric gRPC Service Definitions

This repository contains the [grpc] service and [protocol buffer][protobuf]
definitions for the Hyperledger Fabric project. Tools like `protoc` can
transform these definitions into code that can be used by clients and
libraries to interact with Fabric.

We welcome contributions to the Hyperledger Fabric project in many forms.
There’s always plenty to do! Check the documentation on
[how to contribute][contributing] to this project for the full details.

## Community

- [Hyperledger Community](https://www.hyperledger.org/community)
- [Hyperledger mailing lists and archives](http://lists.hyperledger.org/)
- [Hyperledger Chat](http://chat.hyperledger.org/channel/fabric)
- [Hyperledger Fabric Issue Tracking (JIRA)](https://jira.hyperledger.org/secure/Dashboard.jspa?selectPageId=10104)
- [Hyperledger Fabric Wiki](https://wiki.hyperledger.org/display/Fabric)
- [Hyperledger Wiki](https://wiki.hyperledger.org/)
- [Hyperledger Code of Conduct](https://wiki.hyperledger.org/display/HYP/Hyperledger+Code+of+Conduct)

## License <a name="license"></a>

Hyperledger Project source code files are made available under the Apache License, Version 2.0 (Apache-2.0), located in the [LICENSE](LICENSE) file. Hyperledger Project documentation files are made available under the Creative Commons Attribution 4.0 International License (CC-BY-4.0), available at http://creativecommons.org/licenses/by/4.0/.

[contributing]: https://hyperledger-fabric.readthedocs.io/en/latest/CONTRIBUTING.html
[grpc]: https://grpc.io/docs/guides/
[protobuf]: https://github.com/protocolbuffers/protobuf/
[rocketchat-image]: https://open.rocket.chat/images/join-chat.svg
[rocketchat-url]: https://chat.hyperledger.org/channel/fabric

## How to build fabric-protos-go lib

1. using file ci/Dokcerfile to build docker image which provides isolated environment and relative tools to build lib
2. In directory fabric-protos, making directory build/fabric-protoc-go and running docker container to execute file ci/compile_go_protos.sh
3. now, get your lib in build/fabric-protoc-go
