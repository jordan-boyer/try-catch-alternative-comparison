# Try Catch Alternative Comparison

✨ This [Nx workspace](https://nx.dev) is dedicated to comparing different approaches to error handling in TypeScript, as alternatives to traditional `try-catch` blocks. We'll be focusing on `effect-ts`, `ts-result`, and `neverthrow`. ✨

[Learn more about this workspace setup and its capabilities](https://nx.dev/nx-api/js?utm_source=nx_project&amp;utm_medium=readme&amp;utm_campaign=nx_projects) or run `npx nx graph` to visually explore what was created.

## Purpose of this Project

The goal is to provide clear, practical examples of how to use `effect-ts`, `ts-result`, and `neverthrow`. We will define common error-handling scenarios in a dedicated `scenarios` package, and then implement solutions for these scenarios using each of the target libraries. This approach aims to highlight their APIs, usage patterns, and help developers choose the right tool for their needs.

## Libraries Under Comparison

We will be exploring the following libraries by implementing solutions for the common scenarios:

- **[Effect](https://effect.website/)**: A comprehensive functional effect system for TypeScript.
- **[ts-result](https://github.com/badrap/ts-result)**: A simple, light-weight `Result` type implementation for TypeScript.
- **[Neverthrow](https://github.com/supermacro/neverthrow)**: A type-safe error handling library for TypeScript and JavaScript.

## Core Scenarios

The `packages/scenarios` library will define the specifics (interfaces, mock functions, etc.) for the following common use cases. The other libraries will then implement solutions based on these definitions:

1. **Fetching Data from an API**: Handling potential network errors, timeouts, and parsing successful or error responses.
2. **Data Validation**: Validating input (e.g., user-provided data, configuration) and signaling validation errors.
3. **Sequential Operations**: Performing a chain of operations where any step can fail, and subsequent steps depend on the success of prior ones (e.g., read file, parse content, transform data).
4. **Combining Multiple Results**: Aggregating results from several independent operations that can each succeed or fail.
5. **Error Type Handling**: Demonstrating how each library allows for typed errors and how to handle different error types defined within the scenarios.
