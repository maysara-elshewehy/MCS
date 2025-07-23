# Maysara Code Style 🔥
<br>
<div align="center">
    <p style="font-size: 24px;">
        <i>"Code as Art, Structure as Poetry"</i>
    </p>
</div>

<div align="center">
    <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    <br>
</div>

## Introduction

The Maysara Code Style represent a philosophy of software development that treats code not just as a functional tool, but as an artistic expression. These rules define a consistent approach to project structure, code organization, documentation, and testing that prioritizes both aesthetic beauty and technical excellence.

Developed by [Maysara Elshewehy](https://github.com/maysara-elshewehy) for the [SuperZIG](https://github.com/Super-ZIG) framework, these rules aim to create code that is not only efficient and reliable but also visually pleasing and intuitively organized.

- ### Core Principles

    1. **Aesthetic Harmony**: Code should be visually balanced and pleasing to read

    2. **Logical Hierarchy**: Project structure should follow a clear, intuitive organization

    3. **Self-Documentation**: Code should explain itself through structure and comments

    4. **Comprehensive Testing**: Every function deserves thorough testing

    5. **Performance Optimization**: Elegant code should also be efficient code

    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>

- ### Index

    - [Introduction](#introduction)
    - [Core Principles](#core-principles)
    - [1. Project Structure Rules](#1-project-structure-rules)
    - [1.1 Directory Hierarchy](#11-directory-hierarchy)
    - [1.2 Module Organization](#12-module-organization)
    - [1.3 File Naming Conventions](#13-file-naming-conventions)
    - [2. Code Structure Rules](#2-code-structure-rules)
    - [2.1 File Header](#21-file-header)
    - [2.2 Section Demarcation](#22-section-demarcation)
    - [2.3 Subsection Demarcation](#23-subsection-demarcation)
    - [2.4 Common Section Types](#24-common-section-types)
    - [2.5 Code Indentation](#25-code-indentation)
    - [3. Documentation Rules](#3-documentation-rules)
    - [3.1 Documentation Structure](#31-documentation-structure)
    - [3.2 Visual Elements](#32-visual-elements)
    - [3.3 Section Organization](#33-section-organization)
    - [3.4 Code Examples](#34-code-examples)
    - [4. Function Documentation Rules](#4-function-documentation-rules)
    - [4.1 Function Comment Structure](#41-function-comment-structure)
    - [4.2 Implementation Comments](#42-implementation-comments)
    - [5. Testing Rules](#5-testing-rules)
    - [5.1 Test Organization](#51-test-organization)
    - [5.2 Test Naming](#52-test-naming)
    - [5.3 Test Coverage](#53-test-coverage)
    - [5.4 Test Data](#54-test-data)
    - [6. Implementation Rules](#6-implementation-rules)
    - [6.1 Performance Optimization](#61-performance-optimization)
    - [6.2 Function Design](#62-function-design)
    - [6.3 Error Handling](#63-error-handling)
    - [7. Benchmarking Rules](#7-benchmarking-rules)
    - [7.1 Benchmark Organization](#71-benchmark-organization)
    - [7.2 Benchmark Reporting](#72-benchmark-reporting)
    - [Conclusion](#conclusion)

    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>

- ### 1. Project Structure Rules

    - ### 1.1 Directory Hierarchy

    The project follows a hierarchical structure that reflects the logical organization of functionality:

    ```
    lib/                          # Root directory for all library code
    ├── {module}.zig             # Main entry point for a module
    ├── {module}/                # Module-specific directory
    │   ├── {module}.zig         # Core module implementation
    │   ├── {module}.test.zig    # Module tests
    │   └── utils/               # Specialized utilities
    │       ├── {util}/          # Utility-specific directory
    │           ├── {util}.zig   # Utility implementation
    │           └── {util}.test.zig # Utility tests
    ```

    - ### 1.2 Module Organization

        - Each logical component gets its own directory

        - Implementation and tests are separated but adjacent

        - Utilities are grouped under a `utils` directory

        - Complex utilities may have their own subdirectories and submodules

    - ### 1.3 File Naming Conventions

        - All filenames use lowercase with underscores (`snake_case`)

        - Implementation files are named after their module/utility: `ascii.zig`

        - Test files append `.test` to the implementation name: `ascii.test.zig`

        - Documentation files use `index.md` within a directory named after the module

    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>

- ### 2. Code Structure Rules

    - ### 2.1 File Header

        Every source file begins with a standardized header:

        ```zig
        // {filename} — Brief description of the file's purpose
        //
        // repo   : https://github.com/Super-ZIG/io
        // docs   : https://super-zig.github.io/io/{path}
        // author : https://github.com/maysara-elshewehy
        //
        // Developed with ❤️ by Maysara.
        ```

    - ### 2.2 Section Demarcation

        Code is organized into logical sections with decorative borders:

        ```zig
        // ╔══════════════════════════════════════ SECTION ══════════════════════════════════════╗

            // Code goes here, indented by 4 spaces

        // ╚══════════════════════════════════════════════════════════════════════════════════════╝
        ```

    - ### 2.3 Subsection Demarcation

        Subsections within a section use lighter borders:

        ```zig
        // ┌──────────────────────────── SUBSECTION ────────────────────────────┐

            // Code goes here, indented by 4 spaces

        // └──────────────────────────────────────────────────────────────────┘
        ```

    - ### 2.4 Common Section Types

        - `PACK`: For imports and exports

        - `CORE`: For primary implementation code

        - `TEST`: For test functions

        - `INIT`: For initialization code and constants

    - ### 2.5 Code Indentation

        - All code within a section is indented by 4 spaces

        - This creates visual separation between section borders and code

    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>

- ### 3. Documentation Rules

    - ### 3.1 Documentation Structure

        Documentation files follow a consistent structure with HTML-style sections:

        ```html
        <!--------------------------------- SECTION --------------------------------->

        Content goes here

        <!--------------------------------------------------------------------------->
        ```

    - ### 3.2 Visual Elements

        - Use centered headings and badges

        - Include decorative separators between sections

        - Employ consistent styling with custom fonts when appropriate

    - ### 3.3 Section Organization

        Standard documentation sections include:
        1. Header with title and badges

        2. Features overview

        3. Quick start guide with examples

        4. API reference

        5. Implementation details

        6. Benchmarks

        7. Footer with attribution

    - ### 3.4 Code Examples

        - Include practical, runnable examples

        - Show expected output with emoji indicators (👉)

        - Group related examples under descriptive headings

    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>

- ### 4. Function Documentation Rules

    - ### 4.1 Function Comment Structure

        Every public function includes a standardized doc comment:

        ```zig
        /// Brief description of what the function does.
        ///
        /// More detailed explanation if needed.
        ///
        /// __Parameters__
        ///
        /// - `param`: Description of the parameter
        ///
        /// __Return__
        ///
        /// - Description of the return value
        ```

    - ### 4.2 Implementation Comments

        Implementation details are documented with regular comments:

        ```zig
        // Branch-free implementation:
        // - Step 1 explanation
        // - Step 2 explanation
        ```

    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>

- ### 5. Testing Rules

    - ### 5.1 Test Organization

        - Tests are organized in separate files with the same structure as implementation files

        - Test sections mirror implementation sections

        - Test constants are defined in an `INIT` section

    - ### 5.2 Test Naming

        Test functions are named after the function they test:

        ```zig
        test "functionName" {
            // Test code
        }
        ```

    - ### 5.3 Test Coverage

        - Test both positive and negative cases

        - Include edge case testing

        - Group related test cases with comments

    - ### 5.4 Test Data

        Define comprehensive test data at the beginning of the test file:

        ```zig
        const uppercase     = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
        const lowercase     = "abcdefghijklmnopqrstuvwxyz";
        // More test data...
        ```

    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>

- ### 6. Implementation Rules

    - ### 6.1 Performance Optimization

        - Prefer branch-free implementations where possible

        - Use bit manipulation for efficient operations

        - Mark performance-critical functions as `inline`

    - ### 6.2 Function Design

        - Functions should do one thing and do it well

        - Return types should be consistent and predictable

        - Parameter names should be descriptive but concise

    - ### 6.3 Error Handling

        - Use explicit error handling with descriptive error types

        - Document potential errors in function comments

        - Test error conditions thoroughly

    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>

- ### 7. Benchmarking Rules

    - ### 7.1 Benchmark Organization

        - Benchmarks are kept in a separate repository

        - Each module has its own benchmark file

        - Benchmarks compare against standard library and third-party alternatives

    - ### 7.2 Benchmark Reporting

        - Include both debug and release build results

        - Report total time, average time, and relative speed

        - Document benchmark environment and methodology

    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>

- ### Conclusion

    The Maysara Code Style represent more than just a coding standard—they embody a philosophy that code can be both functionally excellent and aesthetically beautiful. By following these rules, we create software that is not only efficient and reliable but also a pleasure to read, understand, and maintain.


    <div align="center">
        <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    </div>


<div align="center">
    <a href="https://github.com/maysara-elshewehy">
        <img src="https://img.shields.io/badge/Made with ❤️ by-Maysara-orange"/>
    </a>
</div>
