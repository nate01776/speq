# What is SPEQ?
[SPEQ](https://speq.dev) (pronounced "speck") is a universal and protocol-agnostic specification for APIs and Services.

It is built upon the idea that every API, regardless of protocol has a number of common design patterns, that enables a universal specification.

In addition the describing the APIs themselves, SPEQ can:

- Describe functional test
- Describe integration tests
- Describe virtualized services
- , security and performance as well as virtualized instances of your services.

# What APIs does SPEQ support?
The goal of SPEQ is to support any client/server based service. Examples of supported APIs include:

- REST
- Webhooks
- SOAP
- GraphQL
- gRPC
- Websockets
- Kafka
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

# What about OpenAPI (Swagger) & AsyncAPI?
Specifications like OpenAPI and AsyncAPI have a number of problems:
- They aren't protocol-agnostic
- Versioning is a mess
  - No stance on versioning APIs vs. versioning of the specification which leads to confusion
  - No stance on how the specification should interact with version control (e.g. Git)
- They don't describe how to test the APIs or services
- They are more valuable for API clients rather than those interacting with the API server
- They don't take into account that some APIs store external schemas (e.g. gRPC protobufs or Confluent Schema Registry)
- [Schema Examples](https://phil.tech/2020/openapi-examples/) are fundamentally broken
- They've focused on compliance with JSON Schema and eachother which has made the specifications hard to learn

# What do we need help with?
Everything! Reach out if you're interested in contributing!

# Roadmap
- [ ] Finalize 1.0.0-alpha Specification
- [ ] TypeScript Definitions
- [ ] Finalize 1.0.0 Specification
- [ ] Release Validator
- [ ] OpenAPI Converter
- [ ] AsyncAPI Converter
- [ ] Data-Driven Testing
- [ ] More Security Profiles (e.g. Kerberos, LDAP)
