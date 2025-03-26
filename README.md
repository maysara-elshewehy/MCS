# My Personal Naming Convention 📜

> **Why>**
>
> I simply work on libraries that contain hundreds of files with thousands of lines and hundreds of functions 😔, and because this has become my way of life, these are the rules I will follow when writing any code from now on **_(Damn the rules of the world that don't suit me 😶)_**.

- ## Rules

    - #### Sections

        > `padding = 2` _(1 line before content, 1 line after)_, `margin = 3` _(3 lines between sections)_

        ```zig
        // ╔══════════════════════════════════════ NAME ══════════════════════════════════════╗

            ...

        // ╚══════════════════════════════════════════════════════════════════════════════════╝
        ```

    - #### Sub-Sections

        > `padding = 2`, `margin = 2`

        ```zig
        // ┌──────────────────────────── NAME ────────────────────────────┐

            ...

        // └──────────────────────────────────────────────────────────────┘
        ```

    - #### Structures

        ```zig
        /// Desc.
        const MyStruct = struct {
            /// Desc.
            m_field,
            /// Desc.
            m_fieldTwo,
        };
        ```

    - #### Functions

        ```zig
        /// Desc.
        pub fn functionName(argument, argument_two) bool {
            var local;
            var local_variable;

            if(..) |res| {
                ...
            }

            return false;
        }
        ```

<br>
<div align="center">
    <img src="https://raw.githubusercontent.com/maysara-elshewehy/SuperZIG-assets/refs/heads/main/dist/img/md/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
</div>

<br>
<div align="center">
    <a href="https://github.com/maysara-elshewehy">
        <img src="https://img.shields.io/badge/Made with ❤️ by-Maysara-orange"/>
    </a>
</div>
