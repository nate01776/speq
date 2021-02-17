# What is SPEQ?
[SPEQ](https://speq.dev) (pronounced "speck") is an extensible, protocol-agnostic, and platform neutral specification for APIs and Services.

It is built upon the philosophy that every API, regardless of protocol has a number of common design patterns, that when leveraged appropriately can enable a universal specification

In addition the describing the APIs themselves, SPEQ can:

- Describe API Tests
- Describe Virtualized Services

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
- The specification you create isn't always the specification you want to share or distribute (e.g. internal notes, deprecated information)
- Versioning is a mess
  - No stance on versioning APIs vs. versioning of the specification which leads to confusion
  - No stance on how the specification should interact with version control (e.g. Git)
- They don't describe how to test the APIs or services
- They are more valuable for API clients rather than those interacting with the API server
- They don't take into account that some APIs store external schemas (e.g. gRPC protobufs or Confluent Schema Registry)
- [Schema Examples](https://phil.tech/2020/openapi-examples/) are fundamentally broken
- They've focused on compliance with JSON Schema and eachother which has made the specifications hard to learn

# How do I get syntax highlighting for SPEQ files in my IDE?
Currently SPEQ is 100% compliant with `.yaml` syntax highlighting. 

To avoid the potential for confusion with future extensions and improvements, we settled on a custom file extension for SPEQs. 

However, it's easy to add detection for SPEQ files in your applications!

## Git
### GitHub
Add the line `*.speq linguist-language=yaml` to `.gitattributes` file.

### GitLab
Add the line `*.speq gitlab-language=yaml` to `.gitattributes` file.

## Visual Studio Code
1. Go to Settings -> Text Editor -> Files -> Associations
2. In the table add `*.speq` and map it to `yaml`

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
