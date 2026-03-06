# Orchid
This tool is a free, open source secure file and secrets manager primarily in local storage or on a self-hosted NAS.

This project is extremely new and is still in the planning phases.

## The Plan
There are limited options for password managers and secure file managers for those that want fine grained control over their security policies without creating their own tools. Orchid aims to offer a general minimum security policy while allowing users to freely customize their own policies on:
- encryption schemes and algorithms
- password generation algorithms, regeneration, and auditing
- tool logging
- salting
- database hosting, database versioning, database adapters
- more restrictive input sanitization and handling
- RNG sources
- levels of paranoia (-1 levels of trust)
- more when ideas become available

As well as choose between hosting this information locally, on a self-hosted NAS, or on the cloud (AWS, Azure, whatever).

The plan is to implement the core subsystems, local storage, and a fast, lightweight CLI as the minimum viable product (v0). Beginning in v1, the policy engine will be introduced as well as policy customization.

### Planned Features
1. Automated installation for Linux and Windows
1. Secure Username and Password Verification via a randomly salted Argon2 Password Hash offered by the Bouncy Castle JCA provider
3. AES Encrypted and Securely Random Password Generation via the JCA
4. Default MySQL Database Storage via JDBC
5. Secure Anti-SQL Injection techniques such as Input Verification with regex, Limited Views and Permissions, and Parameterized Queries
6. Custom Exception Handling
7. Maven Build in VS Code, which allows the addition of dependencies for Bouncy Castle and JDBC

#### Advanced User Features
1. Customizable UI
    1. Obscure passwords when logged in, update and delete password information
    2. Faster retrieval time for passwords
    3. Populated account tab for updating and deleting account data
    4. Populate settings/extensions tab for customizing UI look-and-feel
2. Customizable backend options:
    1. Expanded database hosting options for local, cloud, or self hosted databases
    2. Expanded security options/defaults/policies for different use cases or advanced customization
    3. Randomly generated environment variables used for database connection credentials. Generated on installation and can be regenerated according to security policies.
3. CLI/TUI lightweight option
    1. Using picocli, there will be a stripped down, light weight version of the project that can be interacted with via the CLI or a TUI. picocli as it has better security options and thread safety compared to Apache Commons CLI.
    2. Each function or subsystem in Orchid will have it's own CLI or subcommand, such that users can use specific tools like encryption, decryption, database read/write, password generation, and more whenever I think of it.

## Contributing
If this project sounds interesting to you and you'd like to contribute, please refer to our [contributors](contributing.md) page.

If you would like to be more involved in the community, you can join our discord (not set up yet - yeah we are that early in the project).