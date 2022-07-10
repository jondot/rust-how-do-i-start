# Rust :crab:. How do I start?

A collaborative advice for this casual question that gets asked many times, so here it is as a Github repo anyone can contribute to and improve!

* 👁️ Before you start, watch this repo (Github watch button) so you can get updates when we add stuff
* 👷‍♀️ While you're working your way through, feel free to ask questions about ways to start in Rust in [Discussions](https://github.com/jondot/rust-how-do-i-start/discussions)
* 🎊 Feel free to add suggestions and PRs of your own https://github.com/jondot/rust-how-do-i-start#contributing

## 🐱 What to expect?

_Some hand-selected articles to give you a feeling of what's the journey like._

* [My own key learnings after 30k LOC in Rust](https://jondot.medium.com/my-key-learnings-after-30-000-loc-in-rust-a553e6403c19) - I can say that today the experience is much greater than back then. There's so much more to learn from, and the ecosystem is huge. Still, the core ideas in the article are relevant.

# 🚜 Main track

_This is largely the learn path you should follow. It is hand-selected, minimal, and high-value, highly effective content only_

* 📚 Reading (code or text)
* 🏋️‍♀️ Exercise
* 🏗️ Building

1. 🦀 The 📚[Rust Book](https://doc.rust-lang.org/book/). You can read it cover to cover, or skim it. What ever you do, make sure you have a pet project idea to experiment with. You can pick 📚[any of the core utils you like](https://github.com/uutils/coreutils/tree/main/src/uu). The advantage of just re-implementing a core util is that you are probably familiar with one of those, they're just CLI apps and you're not biting more than you can chew, and you do have the source code in that repo for reference.
2. 🏋️‍♀️ If you like exercises as a learning aid, you can swap "building a small project" while reading the Rust book, with 🏋️‍♀️[rustlings](https://github.com/rust-lang/rustlings)
3. 🧰 Pick a hobby project that's useful for you. Something more than trivial that includes data passing and a few modules (just so you get to experience the borrow checker and data modeling) something in the scope of 🏗️[bat](https://github.com/sharkdp/bat/tree/master/src). Work on it and go back to the Rust book from time to time (as well as, well - StackOverflow). Repeat, rinse.
* 🤷‍♀️ Don't have an idea for a hobby project? 🏋️‍♀️[PNGMe](https://picklenerd.github.io/pngme_book/introduction.html) is a good project to build + it's a book and exercise format. Look at the [project idea list](https://github.com/jondot/rust-how-do-i-start#-project-ideas) too.
* 🎩 Don't want to work on a project at all? the 🏋️‍♀️[too many lists](https://rust-unofficial.github.io/too-many-lists/index.html) minibook will have you building linked-lists of all kinds and is quite good
6. 🤝 Asking for feedback is highly encouraged to get better at writing idiomatic, readable and performant Rust. You can ask for feedback in [the Rust Subreddit](https://reddit.com/r/rust) or in [the Rust Programming Language Community Discord Server](https://discord.gg/rust-lang-community).
7. 📐 The 📚[Rust API Guidelines](https://rust-lang.github.io/api-guidelines/) for why things are the way they are. E.g. why `into`, and why the `_mut` postfix. For understanding the Rust-"isms" around you when reading people's code.
9. 🌱 You're now ready for 🏋️‍♀️[Rust by example](https://github.com/rust-lang/rust-by-example) and 🏋️‍♀️[Rust by practice](https://github.com/sunface/rust-by-practice)
10. ⏫ 📚[Rust patterns](https://rust-unofficial.github.io/patterns/intro.html) is a great intro to idioms in Rust
11. 🚀 Next, 📚[Zero to Production in Rust](https://www.zero2prod.com/) will give you some service-ish, production-ish use cases which will round off your experience
12. 🤔 When you feel curious about the "why's", pick up 📚[Rust for Rustaceans](https://nostarch.com/rust-rustaceans). Skim it and read what's interesting to you, cover-to-cover is a hard read, unless you have the focus & time.

From here, since everyone have their own taste, visit 📚[Rust Books](https://lborb.github.io/book/) from time to time to pick up a resource that you feel can move you forward to the next step.

## 📦 Starter libraries - save me from choosing 🤦‍♀️!
_These are opinionated but popular choices. The goal is to avoid [paradox of choice](https://en.wikipedia.org/wiki/The_Paradox_of_Choice) while learning._

* [anyhow](https://docs.rs/anyhow/latest/anyhow/) for error handling
* [clap](https://docs.rs/clap/latest/clap/) for CLI building
* [serde](https://serde.rs/) for serialization, including [serde_json](https://github.com/serde-rs/json) and [serde_yaml](https://github.com/dtolnay/serde-yaml)
* [dialoguer](https://docs.rs/dialoguer/latest/dialoguer/) for CLI prompts and [console](https://crates.io/crates/console) for ANSI colors and handling
* [env_logger](https://docs.rs/env_logger/latest/env_logger/) for logging and [log](https://docs.rs/log/latest/log/) for facade
* [lazy_static](https://docs.rs/lazy_static/latest/lazy_static/) for declaring static variables that have nontrivial initialization
* [rayon](https://github.com/rayon-rs/rayon) for easy concurrency for data, vectors, arrays based workloads
* [reqwest](https://docs.rs/reqwest/latest/reqwest/) and [reqwest-middleware](https://crates.io/crates/reqwest-middleware) for HTTP calls
* [actix-web](https://docs.rs/actix-web/latest/actix_web/) as a web/API server
* [nom](https://crates.io/crates/nom) (parser combinators) or [pest](https://pest.rs/) (peg) for building custom parsers
* [insta](https://crates.io/crates/insta), [wiremock](https://crates.io/crates/wiremock), and [fake](https://crates.io/crates/fake) for testing
* [tap](https://crates.io/crates/tap) for utility

## :ok_hand: Thinking in Rust
_Hand picked material to give you context, reasons, and history of how Rust evolved. Some of it is historical._

* [Rust Programming Techniques (youtube)](https://www.youtube.com/watch?v=vqavdUGKeb4) - a talk from 2018 which is more about "thinking in Rust", and will encourage using more Rust constructs.

## 💡 Project ideas
_These are easy starter project ideas, not full-blown projects, just to get you up and running._

* `cat`, `grep`, `uniq`, `wc`, `find` + more. [in this repo](https://github.com/kyclark/command-line-rust) from the _Command line Rust_ book. -- `Practice` CLI, stdlib, data. `Difficulty` easy.
* [A beefed up calculator](https://crates.io/crates/eva) -- `Practice` CLI, parsing, data. `Difficulty` easy.
* [SMTP Protocol in Go - but implement in Rust](https://notes.eatonphil.com/handling-email-from-gmail-smtp-protocol-basics.html) and build a simple TCP server from scratch -- `Practice` CLI, parsing, services. `Difficulty` easy
* [CloudFormation parser](https://rtoch.com/posts/advanced-serde/). -- `Practice` CLI, serde, errors, data. `Difficulty` medium.
* [Realworld](https://github.com/gothinkster/realworld) implementation in Rust. See [realworld-axum-sqlx](https://github.com/launchbadge/realworld-axum-sqlx). -- `Practice` Web, services, SQL, data. `Difficulty` medium.
* [QR code generator](https://github.com/madprops/qool) -- `Practice` CLI, modules, data. `Difficulty` medium.
* [Redis protocol parser (RESP)](https://redis.io/docs/reference/protocol-spec/) -- `Practice` parsing, TDD, creating Rust libraries, data. `Difficulty` medium.
* [Add a lint to Clippy](https://github.com/rust-lang/rust-clippy/blob/master/doc/adding_lints.md). Clippy is the Rust linter, and you might be using it all day long. How about add stuff to it?. `Practice` real world Rust, parsing, compilers. `Difficulty` hard.
* [JSON log viewer, CLI](https://github.com/gistia/json-log-viewer) -- `Practice` CLI, TUI, modules, data, parsing. `Difficulty` hard.


## 🤾‍♂️ Hold on! I want to just play around before deciding to start

_Some links to give you a feeling of Rust, if you're not ready to make the jump yet, or need some convincing to invest the time_

* Try the [tour of rust](https://tourofrust.com/index.html)
* [A gentle intro to Rust](https://stevedonovan.github.io/rust-gentle-intro/readme.html)
* [Take your first steps with Rust](https://docs.microsoft.com/en-us/learn/paths/rust-first-steps/)


## 💻 Cool stuff to have open in a tab while working
_If you have multiple screens, and like a full immersive learning experience - you can keep these open at all times_

* [A big cheatsheet](https://www.cheats.rs/) or [a smaller cheatsheet](https://upsuper.github.io/rust-cheatsheet/)
* A fun [syntax explorer explainer](https://jrvidal.github.io/explaine.rs/)
* [awesome-rust](https://github.com/rust-unofficial/awesome-rust) and [are we there yet](https://wiki.mozilla.org/Areweyet) for when you're reaching out for a library or need inspiration

## 🚀 Releasing

- [a CI/CD template for your project and crates](https://github.com/SpectralOps/rust-ci-release-template) to start with
- [Documenting your crate](https://blog.guillaume-gomez.fr/articles/2020-03-12+Guide+on+how+to+write+documentation+for+a+Rust+crate)


# Extras 
_These links will help bridge the mental model when you're coming from Node.js_

## I'm a Node.js Developer

1. Add [Rust for node developers](https://github.com/Mercateo/rust-for-node-developers) to your schedule, which is a soft intro just to get your bearings.


## Contributing

Please feel free to submit PRs to improve this list. A few pointers:

1. The list must be concise
2. If there are new tracks, feel free to open them by adding a new subtitle to this README and submit PR (i.e. "Rust for game developers, how do I start?")

Happy hacking!
