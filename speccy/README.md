# DRAFT STATE

# What is Speccy?
[Speccy](https://speccy.dev) (pronounced "specky") is a runtime for SPEQ files.

At minimum, Speccy resolves all `.speq` imports, resolves references and outputs `.speq` files. Optionally, one `.speq` for each version defined.

Additionally, Speccy provides the ability to run tests and deploy virtualized services given a

# How do I use Speccy?

`npm install speccy`

# What commands does Speccy support?

| Command | Description  |
|--|--|
|`speccy --version` |Check the version of speccy|
|`speccy --package [.meta.speq file]` |Resolve all imports and generate a single `.speq`  |
|`speccy --test [.meta.speq file] [api] [version] [url] [options]` |Send test configuration to remote URL.|
|`speccy --virt [.meta.speq file] [api] [version] [url] [options]` |Send virtual service configuration to remote URL.|