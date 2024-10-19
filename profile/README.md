# Leptos

<picture>
    <source srcset="logos/Leptos_logo_pref_dark_RGB.svg" media="(prefers-color-scheme: dark)">
    <img src="logos/Leptos_logo_RGB.svg" alt="Leptos Logo">
</picture>

[![crates.io](https://img.shields.io/crates/v/leptos.svg)](https://crates.io/crates/leptos)
[![docs.rs](https://docs.rs/leptos/badge.svg)](https://docs.rs/leptos)
[![Discord](https://img.shields.io/discord/1031524867910148188?color=%237289DA&label=discord)](https://discord.gg/YdRAhS7eQB)
[![Matrix](https://img.shields.io/badge/Matrix-leptos-grey?logo=matrix&labelColor=white&logoColor=black)](https://matrix.to/#/#leptos:matrix.org)

**Leptos** is a fine grained, reactive, full-stack web framework for building fast and interactive web applications in Rust. It leverages fine-grained reactivity to offer a highly efficient and modern development experience, drawing inspiration from frameworks like SolidJS, and Sycamore.

## Key Features:
- **Fine grained reactivity:** Leptos uses a fine-grained reactive system, enabling efficient updates and state management. This means that only the parts of the UI that changes are re-rendered, leading to a more efficient and performant application (No Virtual DOM!).
- **Rust-Based:** Built in Rust, offering Blazing Fast <sup>TM</sup> performance benefits of a low-level language through WebAssembly.
- **SSR & CSR:** Supports both Server-Side Rendering (SSR) and Client-Side Rendering (CSR), with seamless hydration. A user sees the rendered page immediately, and the client-side JavaScript takes over once it's fully loaded.
- **Full-Stack:** Leptos is a full-stack framework, with a built-in server and client-side framework. This means your frontend and backend are written in the same language. Bye-bye CORS, mismatched types, and other headaches!
- **Component-Based:** Structured around reusable, reactive components for building complex UIs.

## Sounds cool! How do I get started?

We recommend going through the [Leptos Book](https://book.leptos.dev) to get started with Leptos. The book covers everything from setting up a new project to building complex applications with Leptos. In case you are stuck somewhere, the book usually covers most of the common issues and solutions.

### Prerequisites

- **Rust:** Install Rust using [rustup](https://rustup.rs/).
- **Cargo Leptos:** Install `cargo leptos` using `cargo install cargo-leptos`. This greatly simplifies the process of running a project
- **Starter templates:** Use the `cargo leptos new` command to create a new project from a template. You can pick from either an [Actix](https://github.com/leptos-rs/start-actix) or [Axum](https://github.com/leptos-rs/start-axum) backend. If you prefer to have your frontend and backend in different projects, check out the [Axum Workspace Template](https://github.com/leptos-rs/start-axum-workspace) for an example.

## Ecosystem

No framework is complete without a rich ecosystem of libraries and tools. Here are some of the libraries and tools that are part of the Leptos ecosystem:

- [leptos-use](https://leptos-use.rs): A collection of hooks for building reusable logic in Leptos.
- [leptos-query](https://github.com/gaucho-labs/leptos-query): Async state management for Leptos, providing simplified data fetching, integrated reactivity, SSR support, and smart cache management, inspired by TanStack Query.
- [thaw-ui](https://thawui.vercel.app/): An easy to use leptos component library.
- [leptosfmt](https://github.com/bram209/leptosfmt): A formatter for the leptos view! macro.

You can find more libraries and tools in the [Leptos Awesome List](https://github.com/leptos-rs/awesome-leptos).

## Is it production ready?

People usually mean one of three things by this question.

1. **Are the APIs stable?** i.e., will I have to rewrite my whole app from Leptos 0.1 to 0.2 to 0.3 to 0.4, or can I write it now and benefit from new features and updates as new versions come?

The APIs are basically settled. We’re adding new features, but we’re very happy with where the type system and patterns have landed. I would not expect major breaking changes to your code to adapt to future releases, in terms of architecture.

2. **Are there bugs?**

Yes, I’m sure there are. You can see from the state of our issue tracker over time that there aren’t that _many_ bugs and they’re usually resolved pretty quickly. But for sure, there may be moments where you encounter something that requires a fix at the framework level, which may not be immediately resolved.

3. **Am I a consumer or a contributor?**

This may be the big one: "production ready" implies a certain orientation to a library: that you can basically use it, without any special knowledge of its internals or ability to contribute. Everyone has this at some level in their stack: for example I (@gbj) don’t have the capacity or knowledge to contribute to something like `wasm-bindgen` at this point: I simply rely on it to work.

There are several people in the community using Leptos right now for many websites at work, who have also become significant contributors. There may be missing features that you need, and you may end up building them! But, if you're willing to contribute a few missing pieces along the way, the framework is most definitely usable, especially given the ecosystem of libraries that have sprung up around it.

## Come hang out with us!

- **Discord:** Join our [Discord server](https://discord.gg/leptos) to chat with the community and the core team. We're a friendly bunch, and we're always happy to help out!
- **GitHub:** Found a bug? Want to contribute? Head over to our [GitHub repository](https://github.com/leptos-rs/leptos) and open an issue or a pull request.
- **Matrix:** We also have a [Matrix room](https://matrix.to/#/#leptos:matrix.org) if you prefer that over Discord.
