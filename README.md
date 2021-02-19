![SPEQ Logo](https://i.imgur.com/y6RsoEy.png)

# What is SPEQ?
[SPEQ](https://speq.dev) (pronounced "speck") is a universal, protocol-agnostic specification for any API.

SPEQ:
- Provides centralized documentation of every API, Database, and Service within your organization and how they relate to each other
- Can enforce best practices within your organization with its rules engine
- Can replace or complement your existing specifications or schemas
- Provides a framework for virtualizing and testing your APIs, Services and Databases

# What APIs does SPEQ support?
The goal of SPEQ is to support any client/server based service. Examples of supported APIs include:

- REST
- Webhooks
- SOAP
- GraphQL
- gRPC
- SQL DBs
- Websockets
- Apache Kafka
- JDBC
- ODBC
- MQTT
- AMQP
- JMS
- HTTP
- STOMP
- NATS
- coAP
- XML-RPC
- JSON-RPC
- AWS SNS
- AWS SQS
- Google Pub/Sub
- Many more...

# What about edge cases?
Every API, Database and Service has unique implementations, but what makes SPEQ unique is that it's built around an architecture that is protocol-agnostic:

![agnostic-architecture](https://i.imgur.com/JVYo97T.png)

With this base implementation, the key metadata documenting the API is consistent and rules can be put in place for protocol-specific logic or even organization-specific logic with custom extensions. 

# What about other specifications or schema descriptions?
Depending on your needs, SPEQ can replace or act as a meta-schema for:
- OpenAPI
- AsyncAPI
- API Blueprint
- WSDL
- WADL
- Thrift

However, you may have schema descriptions that may be core to the your current development workflow that are hosted externally on a Git repository or schema server. For example:
- SQL DDLs
- Protobufs
- Avro

SPEQ allows you to reference these schemas where they are typically maintained with the goal of eventually providing tools to compile these schemas into SPEQ when updated.

# What's wrong with other specifications / schemas? 
- Other specifications aren't protocol-agnostic, which means one could minimize total specifications by consolidating on SPEQ.
- There often isn't enough justification to keep a non-authoritative specifiation updated, SPEQ tries to resolve this by providing value via its rules engine and auto-generated documentation
- Many specifications have significant drift due to issues with versioning
- Schemas like Avro and Protobuf are kept up-to-date but in many organizations describing where they are stored or how they relate to each other is not. 

# What do we need help with?
- General Feedback
- `speccy` Utility
- Converters (OpenAPI, AsyncAPI, protobuf, Avro, SQL DDL)
- Rules Engine
- Documentation Generator

# Roadmap
- Finalize 1.0.0-alpha Specification
- Launch https://docs.speq.dev
- Launch https://speq.dev
- `speccy --generate`
- `speccy --validate *.meta.speq`
- `speccy --compile *.meta.speq`
- Release Validator
- OpenAPI `speccy --compile *.meta.speq --import-external-schemas`
- Documentation Generator `speccy --docs *.speq`
- Protobuf
- Avro
- SQL DDL
- AsyncAPI
- Add changelog to `speccy --compile`
