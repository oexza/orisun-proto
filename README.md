# Orisun Protocol Buffer Definitions

This repository contains the shared Protocol Buffer definitions for the Orisun Event Store.

## Contents

- `eventstore.proto` - Event Store service definitions
- `admin.proto` - Admin service definitions

## Usage

### Go

Generate Go code from proto files:

```bash
protoc --go_out=. --go_opt=paths=source_relative \
       --go-grpc_out=. --go-grpc_opt=paths=source_relative \
       *.proto
```

### Java

The proto files are used by the Java client's Gradle build process. See [orisun-client-java](https://github.com/oexza/orisun-client-java) for usage.

### Node.js

The Node.js client has its own copy of the proto files. See [orisun-node-client](https://github.com/oexza/orisun-node-client).

## License

MIT License - see [LICENSE](LICENSE) for details.

## Repository

https://github.com/oexza/orisun-proto