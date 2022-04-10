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

1. The [Rust Book](https://doc.rust-lang.org/book/). You can read it cover to cover, or skim it. What ever you do, make sure you have a pet project idea to experiment with. You can pick [any of the core utils you like](https://github.com/uutils/coreutils/tree/main/src/uu). The advantage of just re-implementing a core util is that you are probably familiar with one of those, they're just CLI apps and you're not biting more than you can chew, and you do have the source code in that repo for reference.
2. If you like exercises as a learning aid, you can swap "building a small project" while reading the Rust book, with [rustlings](https://github.com/rust-lang/rustlings)
3. Once you finished a first pass at the Rust book, pick a hobby project that's useful for you. Something more than trivial that includes data passing and a few modules (just so you get to experience the borrow checker and data modeling) something in the scope of [bat](https://github.com/sharkdp/bat/tree/master/src). Work on it and go back to the Rust book from time to time (as well as, well - StackOverflow). Repeat, rinse.
4. Asking for feedback is highly encouraged to get better at writing idiomatic, readable and performant Rust. You can ask for feedback in [the Rust Subreddit](https://reddit.com/r/rust) or in [the Rust Programming Language Community Discord Server](https://discord.gg/rust-lang-community).
5. You're now ready for [Rust by example](https://github.com/rust-lang/rust-by-example) and [Rust by practice](https://github.com/sunface/rust-by-practice)
6. When you feel curious about the "why's", pick up [Rust for Rustaceans](https://nostarch.com/rust-rustaceans). This is the point where you're moving from beginner to intermediate Rust developer.
7. Next, [Zero to Production in Rust](https://www.zero2prod.com/) will give you some service-ish, production-ish use cases which will round off your experience

From here, since everyone have their own taste, visit [Rust Books](https://lborb.github.io/book/) from time to time to pick up a resource that you feel can move you forward to the next step.

## 🤾‍♂️ Hold on! I want to just play around before deciding to start

_Some links to give you a feeling of Rust, if you're not ready to make the jump yet, or need some convincing to invest the time_

* Try the [tour of rust](https://tourofrust.com/index.html)
* [A gentle intro to Rust](https://stevedonovan.github.io/rust-gentle-intro/readme.html)


## 💻 Cool stuff to have open in a tab while working

_If you have multiple screens, and like a full immersive learning experience - you can keep these open at all times_

* [A big cheatsheet](https://www.cheats.rs/) or [a smaller cheatsheet](https://upsuper.github.io/rust-cheatsheet/)
* A fun [syntax explorer explainer](https://jrvidal.github.io/explaine.rs/)
* [awesome-rust](https://github.com/rust-unofficial/awesome-rust) and [are we there yet](https://wiki.mozilla.org/Areweyet) for when you're reaching out for a library or need inspiration


# Extras: Node.js Developers

_These links will help bridge the mental model when you're coming from Node.js_

1. Add [Rust for node developers](https://github.com/Mercateo/rust-for-node-developers) to your schedule, which is a soft intro just to get your bearings.


## Contributing

Please feel free to submit PRs to improve this list. A few pointers:

1. The list must be concise
2. If there are new tracks, feel free to open them by adding a new subtitle to this README and submit PR (i.e. "Rust for game developers, how do I start?")

Happy hacking!
